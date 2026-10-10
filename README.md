# team list

`TEAM.md` is a shared list everybody appends to. Two branches editing the same
place in it is how you get a merge conflict — which is the point of this one.

**What a merge conflict is:** Git can combine two branches by itself as long as
they touched different lines. When both changed the same lines, Git won't guess
which one is right. It stops, writes both versions into the file, and leaves the
choice to you. Between `<<<<<<<` and `=======` is your side, between `=======` and
`>>>>>>>` is the incoming side, so `=======` is just the line separating the two
versions. You resolve it by editing the block down to what you want, deleting
all three marker lines, and committing.
