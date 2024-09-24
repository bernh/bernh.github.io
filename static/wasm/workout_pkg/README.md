# EBNF of the grammar

    parts = part, { "+", part };
    part = repetition | step;
    repetition = number, "*", "(", parts, ")"; 
    step = time_step | distance_step;
    distance_step = distance, effort;
    time_step = time, ("min" | "s"), effort;

EBNF can be rendered with PlantUML  

Implementation always normalizes to a `1 * (<input>)` which is a bit of a hack
since we basically start parsing with a `repetition` instead of `parts`. 