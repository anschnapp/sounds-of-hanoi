# sounds-of-hanoi
Experimental sonic pi sound scripts based on algorithms (starting with tower of hanoi)

## current sounds

### sounds of hanoi
It's a simple recursive algorithm which solves a tower of hanoi problem.
The sound is about the movement which happens while the problem is being solved.

There are different sounds for movements from left to middle, middle to right and so on.

In addition there is a special sound which appears when one hanoi problem (so also the recursive sub problems) has solved.
The intensity of this sound is higher if a bigger tower was moved, so the loudest sound of this type is at the end when the hole problem was solved.

You could easily play around and test for bigger towers or change the sound effects.

There is also a mp3 file available so you could hear it (without extra installing sonic pi just to for hearing)
(of course this is only one recorded version of it, currently it's the one of tag version 1.0.0)

### sounds of quicksort
It's a simple recursive algorithm of quicksort.

The sounds are here represented by numbers which are natively used as higher and lower beep tones in sonic pi.
The range from 40 to 115 is used here but also many subtones between them.
Without changing the parameter are list of 300 items between this range is created (0.25 steps simple increasing)

This list is then randomized and played. The beauty of playing the random list is to give a hint how random values sounds.
Then there is a 2 second break.

After this step the quicksort starts. Every number which is compared (for moving to low or high set) will play it's tone.

You could hear that first it sounds also quite random. Then at some point you hear the fine sorting on the low tones.
Then it goes back to some in between lists for the middle tones. And so on until it ends with fine tuning the high tones (sorry for that it's not so nice for the ears ;))
After quick search has finished there is also a 2 second break.

After the hole algorithm has finished you will hear the sorted version of the list.

You could easily play around and change parameters. To maybe hear longer lists, or even the worst case, a pre sorted list ;)!

There is also a mp3 file available so you could hear it (without extra installing sonic pi just to for hearing)
(of course this is only one recorded version of it, currently it's the one of tag version 1.0.0)

### sounds of bubble sort
The sound here represents all comparisons done while the bubble sort algorithm is executed (similar to the quicksort variant).

Also here you would first hear the random list of tones. Then a 2 seconds delay. Then the actual sound of the algorithm. Again a 2 second delay and then the sorted list.
The frequency bandwidth of tones is the same here as for quicksort (40 to 115).
But this time only 100 items are used because this algorithm gets incredible slow if we fit it with 300 or 400 like we do in the quicksort example.
You could hear that it's a smaller dataset in the list when you hear the random and or the sorted list, because the length of playing it is proportional to the items of the list.

Also here i have put a sound file close to the source code. (just for getting an idea without the need of executing it on sonic pi)
