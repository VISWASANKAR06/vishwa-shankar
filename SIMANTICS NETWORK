% Person: has body = true
:- object(person).

    :- public(has/1).
    has(body).

:- end_object.

% Man: is a Person, default height = 170
:- object(man, extends(person)).

    :- public(height/1).
    height(170).

:- end_object.

% Sport Star: is a Man, default height = 190
:- object(sport_star, extends(man)).

    % override inherited height
    height(190).

:- end_object.

% Mark: is a Sport Star
:- object(mark, extends(sport_star)).

:- end_object.

% Spencer: is another Sport Star, but slim
:- object(spencer, extends(sport_star)).

    % override inherited height
    height(165).

:- end_object.
