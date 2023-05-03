Download Link: https://assignmentchef.com/product/solved-cs384-tutorial-6-web-series-renamer-regular-expression
<br>
A sample set of <strong>srt+mp4 </strong>is given to you in separate folders. You need to rename <strong>mp4 + srt files</strong>. You know that in VLC/any media play will auto include the srt if the filename and srt name is same.

There shall be two folders. wrong srt – containing pre-renamed file name

corrected srt – after rename, ensure that new filenames are placed here. You need to ask 3 inputs from the users

<ol>

 <li>Initially make a menu based program that will ask which web series to rename. The sample python code I have already given along with the variables.</li>

 <li>Season Number Padding (take int input): The padding given to the season number. A padding of three digits means if the series have 20 seasons then it will be renamed as season 001, 002, 003…, 019, 020.</li>

 <li>Episode Number Padding (take int input): For example, a padding of two means if the series have</li>

</ol>

30 episodes then it will be renamed as episode 01, 02, …, 30

There are 3 folders that you need to rename:

<ol>

 <li>Breaking Bad</li>

 <li>Game of Thrones</li>

 <li>Lucifer</li>

</ol>

Lets say the user provides these inputs:

<ol>

 <li>Main Title of the <strong>Web Series</strong>: 2</li>

 <li>Season Number Padding (take int input): 1</li>

</ol>

1

<ol start="3">

 <li>Episode Number Padding (take int input): 2</li>

</ol>

<strong>Original</strong>:: ‘Game of Thrones – 8×05 – The Bells.WEB.REPACK.MEMENTO.en.srt” <strong>New</strong>: “Game of Thrones – Season 8 Episode 05 – The Bells.srt”

Also look, there is an interesting case: Look at one of the names:

“Game of Thrones – 8×05 – The Bells.WEB.REPACK.MEMENTO.en.srt”

<strong>Original</strong>:: ‘Game of Thrones – 8×05 – The Bells.WEB.REPACK.MEMENTO.en.srt”

<strong>New</strong>: “Game of Thrones – Season 8 Episode 05 – The Bells.srt”

Here you can see that ”.WEB.REPACK.MEMENTO.en” is the string that is not required. Usually every srts have common strings towards the end that needs to be identified manually and stripped. So in case of Game of Thrones, you need to find out manually such non-useful string and strip them in the final code. A <strong>recommended </strong>approach will be <strong>regex</strong>. Like <strong>splitting </strong>on the <strong>WEB </strong>and other such string (e.g., <strong>720p</strong>). Similar manner do it for mp4 also. So both srt and mp4 will have same name and only the extensions shall differ.

<strong>Task: </strong>Based on the received input, the filename should be <em>seriesname season number (depending on the padding) episode number (depening on the padding) + episode name ()if any)</em>. Following series needs to be renamed (srt+mp4) via the os module.

<ol>

 <li>Breaking Bad</li>

 <li>Game of Thrones</li>

 <li>Lucifer</li>

</ol>

<strong>Spaces should be strictly one between characters and numbers.</strong>