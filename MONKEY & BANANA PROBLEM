public class DLS extends Abstract {

   Node sourceNode;
   Node goalNode;
   int depth = 0;
   int limit = 2;

   public DLS(Node source, Node goalNode){
       super(source, goalNode);
       this.sourceNode = source;
       this.goalNode = goalNode;
   }

   public boolean execute(){
       Stack<node> nodeStack = new Stack<>();
       ArrayList<node> visitedNodes = new ArrayList<>();
       nodeStack.add(sourceNode);

       depth = 0;

       while(!nodeStack.isEmpty()){
           if(depth <= limit) {
               Node current = nodeStack.pop();
               if (current.equals(goalNode)) {
                   System.out.print(visitedNodes);
                   System.out.println("Goal node found");
                   return true;
               } else {
                   visitedNodes.add(current);
                   nodeStack.addAll(current.getChildren());
                   depth++;

               }
           } else {
               System.out.println("Goal Node not found within depth limit");
               return false;
           }
       }


       return false;
   }
}
