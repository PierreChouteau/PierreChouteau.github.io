---
title: "Audio files"
layout: single
permalink: /audio
author_profile: false
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
excerpt: "" # "Here you can find the audio files of the different pieces we worked on." - Example of a subtitle
class: wide
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---
<html>

</html>


# Source separation results

We tried our algorithm in different configurations to evaluate its efficiency. The algorithm takes a multichannel audio with all instrument playing as input, and produces 5 (1 per source) multichannel audios as if the instrument was playing alone in the room. Here we present the most interesting results for the different cases with all audios.

## Technical precision
The piece is written for a quintet: Violins, Flute, Clarinet and Cello. We used 8 microphones for the recording:
- 5 *spot* microphones close to each instrument (named after the instrument)
- 3 linked microphones to capture the global scene (named Left, Center, Right)

All the microphones are used for the separation.

## Test d'un tableau pour les résultats

> Full mix
<audio controls>
  <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav"/>
</audio>

> Separated sources

<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center> Original </center>
        </th>
        <th>
          <center> Ref </center>
        </th>
        <th>
          <center> Unet </center>
        </th>
        <th>
          <center> VA_NN_1 </center>
        </th>
        <th>
          <center> Warmup </center>
        </th>
      </tr>
    </thread>
    <tbody>
      <tr>
        <th> <strong> Soprano </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Alto </strong> </th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
      </tr>
      <tr>
        <th> <strong> Basse </strong> </th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
      </tr>
    </tbody>
  </table>
</html>

## Separation on full mix without prior information

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <center>
    <strong> Original </strong>
    </center>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <center>
    <strong> Separated </strong>
    </center>
  </div>
</div>

</html>

> Violin 1

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
  <source src="/audio/no_effect_audios/separation/micro_Violin1/source_3_micro_Violin1_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Violin 2

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/no_separation/micro_Violin2.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/separation/micro_Violin2/source_4_micro_Violin2_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Flute

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/no_separation/micro_Flute.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/separation/micro_Flute/source_0_micro_Flute_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Clarinet

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/no_separation/micro_Clarinet.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/separation/micro_Clarinet/source_1_micro_Clarinet_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Cello

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/no_separation/micro_Cello.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/no_effect_audios/separation/micro_Cello/source_2_micro_Cello_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>


## Separation on raw audio without prior information
<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <center>
    <strong> Original </strong>
    </center>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <center>
    <strong> Separated </strong>
    </center>
  </div>
</div>

</html>

> Violin 1

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/no_separation/micro_Violin1.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
  <source src="/audio/sto_audios/separation/micro_Violin1/source_3_micro_Violin1_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Violin 2

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/no_separation/micro_Violin2.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/separation/micro_Violin2/source_4_micro_Violin2_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Flute

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/no_separation/micro_Flute.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/separation/micro_Flute/source_0_micro_Flute_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Clarinet

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/no_separation/micro_Clarinet.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/separation/micro_Clarinet/source_1_micro_Clarinet_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Cello

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/no_separation/micro_Cello.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/sto_audios/separation/micro_Cello/source_2_micro_Cello_audio_length_12_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>


## Separation on raw audio with prior information
<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <center>
    <strong> Original </strong>
    </center>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <center>
    <strong> Separated </strong>
    </center>
  </div>
</div>

</html>

> Violin 1

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/no_separation/micro_Violin1.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
  <source src="/audio/prior_dictionnary/separation/micro_Violin1/source_3_micro_Violin1_audio_length_10_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Violin 2

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/no_separation/micro_Violin2.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/separation/micro_Violin2/source_4_micro_Violin2_audio_length_10_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Flute

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/no_separation/micro_Flute.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/separation/micro_Flute/source_0_micro_Flute_audio_length_10_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Clarinet

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/no_separation/micro_Clarinet.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/separation/micro_Clarinet/source_1_micro_Clarinet_audio_length_10_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>

> Cello

<html>

<div id="container">
  <div id="left-column">
    <!-- content for the left column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/no_separation/micro_Cello.wav">
    </audio>
  </div>
  <div id="right-column">
    <!-- content for the right column goes here -->
    <audio controls>
      <source src="/audio/prior_dictionnary/separation/micro_Cello/source_2_micro_Cello_audio_length_10_n_basis_32_n_fft_4096.wav">
    </audio>
  </div>
</div>

</html>
