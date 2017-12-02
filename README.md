<h1>APOPHENIA</h1>

This Pure Data project was developed for an assignment in Sound Synthesis for Digital Media. It is inspired by the works of Terry Riley and the ideaof texture perceived from repetition of movement and sound.

<h2>Project Structure</h2>

The project is structured to ensure the easiest playing possible. As such, several abstractions were used along with the graph-on-parent technique. The main patch is named <strong>Apophenia-master.pd</strong>, this is the one used to play. The remaining patches constitute the building blocks. This is the file list of the project:
<ul>
    <li> aArrays.pd </li>
    <li> aDelay.pd </li>
    <li> Apophenia.pd </li>
    <li> Apophenia-master.pd </li>
    <li> aSample.pd </li>
    <li> aVol.pd </li>
    <li> aVolMaster.pd </li>
</ul>

<h2>Main Patch Composition</h2>

The <strong>first block</strong>, present in green, is related to the imported sample. here it is possible to see the array which holds the sample, define the left and right sample limits, the playback speed and preview where the reading needle is.

The <strong>second block</strong>, in orange, is the volume control of the sample.

The <strong>third block</strong>, in light blue, holds the delay controls and a low pass filter that only affects the delay line. Here you can control the delay time, feedback amount, delay level and lowpass frequency.

The <strong>fourth block</strong>, in violet, shows the elements that control the [freeverb~] reverb external. This control block was extracted from the patch <a href="patchstorage.com/freeverbcontrol">freeverbcontrol</a> present in the patchstorage website.

The <strong>fifth block</strong>, in red, is the master volume for the entire patch. It has a toggle to turn on and off the dsp, and has a lowpass filter that affects all the input sounds.

<h2>Aknowledgments:</h2>
<a href="https://linkedin.com/in/joaogomesreis">João Reis</a>, Nuno Loureiro, <a href="http://ruipenha.pt/">Rui Penha</a>

<h2>References:</h2>
<a href="https://forum.pdpatchrepo.info/topic/10666/delay-with-tap-tempo-sync">Delay With Tap Tempo Sync</a>
<br> <a href="https://daniel-murray.github.io/blog/2013/01/21/abstractions-and-user-interfaces-in-pure-data/">Abstractions and User Interfaces in Pure Data</a>
<br> <a href="http://www.pd-tutorial.com/english/ch03s04.html">Pd tutorial — 3.4 Sampling</a>
<br> <a href="https://patchstorage.com/platform/pd-vanilla/">Patchstorage Pd-vanilla</a>
<br> <a href="https://www.youtube.com/watch?v=nTTZZyD4xlE">PURE DATA: 06 Conditional Logic with Spigot & Moses</a>
