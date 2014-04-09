# Average pocket money calculation without leaking individual information

An organizer can propose this question to the participants, let them come up
with ideas, and point out flaws in the ideas. For example, using a trusted
third party can be expensive and needs full trust of all participants.

One possible solution without a trusted third party: people sit in a circle,
forming a circular linked list. One of them volunteers to be the head of a
list, and writes two large random numbers on a sheet of paper, and passes on
the paper. The next one reads the two numbers, adds his own pocket money amount
to the first number, and increments the 2nd number by 1, writes the new numbers
to another (previously empty) sheet of paper, and passes that paper to the
next. At the end, the head person adds his own pocket money amount and 1, then
subtracts the two (corresponding) random numbers, and reads the results: the
sum and the count of people. Then everybody can divide to get the average.

(Those who don't want to participate just add 0 and 0 when it's their turn, or
they don't join the circle, thus they declare their non-participation openly.)

Then the organizer can mention that asking for the maximum value and asking who
has the maximum for a group size larger than 2 are unsolved problems. And the
known solution for 2 people is very slow and complicated.

What this teaches: privacy is important, algorithms can improve (provide)
privacy, privacy is hard, random numbers are useful, small random numbers are
not as useful, cooperation is necessary.
