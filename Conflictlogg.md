                               <<<Deltagare: Patrik Tjäder, Andreas Sellmander, Christoffer Ohlsson, Ulf Larsson >>>



Merge-konflikten uppstod när flera personer arbetade i samma dokument (Topp 5) i olika brancher.
Filen innehöll varje deltagares “Top 5 spel”-lista, där varje person skrev sin del direkt under den föregående.
Patrik skapade dokumentet  Därefter skapade vi fyra brancher där varje person fyllde i sin egen del.
Konflikten uppstod när en av de andra brancherna mergeades — den innehöll bara radbrytningar (“enter”) under Patriks lista,
vilket Git tolkade som en ändring i samma område av filen. Eftersom Git inte kunde avgöra om Patriks text eller den andras tomma rader skulle behållas,
markerades det som en merge-konflikt. Konflikten löstes genom att semi manuellt (via merge editor) redigera filen och ta bort behålla alla fyra listorna i rätt ordning.
Därefter sparades filen, stageades (git add), och committades som en löst konflikt.