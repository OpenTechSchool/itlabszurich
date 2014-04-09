= Frog Game

The game is played on a 7x1 grid with the initial state `>>>@<<<`.  Each `<` is
a frog which can step 1 left or jump over a single frog to the left.  Each `<`
is a frog which can step 1 right or jump over a single frog to the right.  The
`@` is an empty cell. The goal is to swap the frogs, i.e. to reach this state:
`<<<@>>>`.

== Solution for 3+3

The 15-step solution for 3+3 frogs is:

    >>>@<<<
    >>@><<<
    >><>@<<
    >><><@<
    >><@<><
    >@<><><
    @><><><
    <>@><><
    <><>@><
    <><><>@
    <><><@>
    <><@<>>
    <@<><>>
    <<@><>>
    <<<>@>>
    <<<@>>>

After some trial and error one learns how he the frogs get stuck:  If there is
a `>><` and no `@` anywhere to the right of it, then the `<` frog gets stuck,
because it has no way to jump over the `>>`, and the `>>` can't be broken up
because they have no destination to jump to.  (By flipping this we get to other
kind of stuck state.)  With pencil and paper one can easily come up with a move
sequence in which we avoid getting stuck, thus eventually the frogs reach the
target state.  Avoiding getting stuck is a bit tricky, because it's not always
immediate:  For example, from `>><>@<<` we can move to `>><@><<` (not being
stuck yet), to which it's possible to move to `>><<>@<` or `>@<>><<`, both of
which are stuck.

== How to animate this game

Organize participants to groups of 6, split each group to 3+3, give some token
to each of the first 3, make them stand in a line, 3+3 facing each other with a
gap between.  Announce that the first group who reaches the target state wins.
Ask them to start moving. There should be at least 1 organizer per group, who
watches them if they are moving according to the rules.  Let them return to the
initial state if they wish, any number of times.  Don't tell them that they are
allowed to plan and draw in advance, but let them if they want to do it.


== Solution for 4+4

FYI The 24-step solution for 4+4 frogs is:

    >>>>@<<<<
    >>>@><<<<
    >>><>@<<<
    >>><><@<<
    >>><@<><<
    >>@<><><<
    >@><><><<
    ><>@><><<
    ><><>@><<
    ><><><>@<
    ><><><><@
    ><><><@<>
    ><><@<><>
    ><@<><><>
    @<><><><>
    <@><><><>
    <<>@><><>
    <<><>@><>
    <<><><>@>
    <<><><@>>
    <<><@<>>>
    <<@<><>>>
    <<<@><>>>
    <<<<>@>>>
    <<<<@>>>>

This looks like too complicated to figure out on the spot, so just do the 3+3.

What this teaches: planning ahead, nominating a boss who tells others what to
do, think out-of-the-box (by asking for a pencil and paper.)
