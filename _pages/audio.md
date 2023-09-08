---
title: "Audio Examples"
layout: single
permalink: /audio
author_profile: false
# classes: wide
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
excerpt: "Experimental results" # "Here you can find the audio files of the different pieces we worked on." - Example of a subtitle
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---
<html>

</html>


Welcome to the audio examples page. Here you'll find the results of our experiments, as well as audio examples of music source separation.




For experiments where our architecture is compared to the [__US__](https://ieeexplore.ieee.org/document/10058592) model by Schulze-Foster _et al._ and the [__U-Net__](https://program.ismir2020.net/poster_5-14.html) model by Petermann _et al._, we show only our two best approaches:
- __VA_NN_2__
- __Warmup__

All the audios presented below are taken from the evaluation datasets: __ChoralSingingDataset__ or __Cantoria__.



<br/>

---
# Source separation results - Joint learning

## BC1song

For these results, we trained the different models on the __BC1Song__ dataset, and evaluated on the __ChoralSingingDataset__ dataset.

> Audio Mix Example
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>


> Separated voices from Wiener filtering
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
          <center> US </center>
        </th>
        <th>
          <center> Unet </center>
        </th>
        <th>
          <center> VA_NN_2 </center>
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
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
      </tr>
     <tr>
        <th> <strong> Alto </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Bass </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
      </tr>
    </tbody>
  </table>
</html>
<br/>

## BCBSQ

For these results, we trained the different models on the __BCBSQ__ dataset, and evaluated on the __ChoralSingingDataset__ dataset.

> Audio Mix Example
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>


> Separated voices from Wiener filtering
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
          <center> US </center>
        </th>
        <th>
          <center> Unet </center>
        </th>
        <th>
          <center> VA_NN_2 </center>
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
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
      </tr>
     <tr>
        <th> <strong> Alto </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Bass </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/Ref_sources/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/VA_NN_1/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BCBQ/W_UP/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
      </tr>
    </tbody>
  </table>
</html>
<br/><br/>

--- 
# Training results on monophonic audios

These results correspond to the evaluation of the __US__ model by Schulze-Foster _et al._ trained on monophonic audios to separate audios with 2 sources (1S &rarr; 2S) and 4 sources (1S &rarr; 4S).  

US<sub>2s</sub> / US<sub>4s</sub> : Reference models trained and evaluated on the same number of sources (2s/4s respectively).

We trained the various models on the __BCBSQ__ dataset, and evaluated them on the __ChoralSingingDataset__ dataset.

## Mono &rarr; 2 Sources

> Audio Mix Example - Alto / Bass
<audio controls>
  <source src="/audio/mono/BCBSQ/mono_to_2sources/mix/mix_el_rossinyol_At_2-06_Bos_207_27.984.wav"/>
</audio>

> Separated voices from Wiener filtering
<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center>Original</center>
        </th>
        <th>
          <center>US<sub>2s</sub></center>
        </th>
        <th>
          <center> 1S &rarr; 2S </center>
        </th>
      </tr>
    </thread>
    <tbody>
      <tr>
        <th> <strong> Alto </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/target_sources/target_sources_el_rossinyol_At_2-06_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/sources_estimates_masking_el_rossinyol_At_2-06_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_At_2-06_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Bass </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/target_sources/target_sources_el_rossinyol_At_2-06_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/sources_estimates_masking_el_rossinyol_At_2-06_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_At_2-06_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/mix_reconstruct_el_rossinyol_At_2-06_Bos_207_27.984.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/mix_reconstruct_el_rossinyol_At_2-06_Bos_207_27.984.wav"/>
          </audio>
        </th>
      </tr>
    </tbody>
  </table>
</html>
<br/>

---

> Audio Mix Example - Soprano / Alto
<audio controls>
  <source src="/audio/mono/BCBSQ/mono_to_2sources/mix/mix_el_rossinyol_Sno_208_At_2-06_27.984.wav"/>
</audio>

> Separated voices from Wiener filtering
<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center>Original</center>
        </th>
        <th>
          <center>US<sub>2s</sub></center>
        </th>
        <th>
          <center> 1S &rarr; 2S </center>
        </th>
      </tr>
    </thread>
    <tbody>
      <tr>
        <th> <strong> Soprano </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/target_sources/target_sources_el_rossinyol_Sno_208_At_2-06_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_27.984_voice_s.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Alto </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/target_sources/target_sources_el_rossinyol_Sno_208_At_2-06_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_27.984_voice_a.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_27.984.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_27.984.wav"/>
          </audio>
        </th>
      </tr>
    </tbody>
  </table>
</html>
<br/>

--- 

> Audio Mix Example - Tenor / Bass
<audio controls>
  <source src="/audio/mono/BCBSQ/mono_to_2sources/mix/mix_el_rossinyol_Tor2-09_Bos_207_27.984.wav"/>
</audio>

> Separated voices from Wiener filtering
<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center>Original</center>
        </th>
        <th>
          <center>US<sub>2s</sub></center>
        </th>
        <th>
          <center> 1S &rarr; 2S </center>
        </th>
      </tr>
    </thread>
    <tbody>
      <tr>
        <th> <strong> Tenor </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/target_sources/target_sources_el_rossinyol_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/sources_estimates_masking_el_rossinyol_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Bass </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/target_sources/target_sources_el_rossinyol_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/sources_estimates_masking_el_rossinyol_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_2s_satb_bcbq_mf0_1/mix_reconstruct_el_rossinyol_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_2sources/unsupervised_1s_bcbq_crepe_10_epo/mix_reconstruct_el_rossinyol_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
      </tr>
    </tbody>
  </table>
</html>
<br/>

## Mono &rarr; 4 Sources

> Audio Mix Example
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>

> Separated voices from Wiener filtering
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
          <center> US<sub>4s</sub> </center>
        </th>
        <th>
          <center> 1S &rarr; 4S </center>
        </th>
      </tr>
    </thread>
    <tbody>
      <tr>
        <th> <strong> Soprano </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_4s_satb_bcbq_mf0_1_again/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_s.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Alto </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_4s_satb_bcbq_mf0_1_again/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_a.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_4s_satb_bcbq_mf0_1_again/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_t.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Bass </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_4s_satb_bcbq_mf0_1_again/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_1s_bcbq_crepe_10_epo/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984_voice_b.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_4s_satb_bcbq_mf0_1_again/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/mono/BCBSQ/mono_to_4sources/unsupervised_1s_bcbq_crepe_10_epo/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
          </audio>
        </th>
      </tr>
    </tbody>
  </table>
</html>

<br/>
<br/>

---
# Generalization on another dataset - Cantoria

For these results, we trained the different models on the __BCBSQ__ dataset, and evaluated them on the __Cantoria__ dataset.


> Audio Mix Example
<audio controls="">
  <source src="/audio/cantoria/mix/mix_CEA_satb_15.984.wav"/>
</audio>


> Separated voices from Wiener filtering
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
          <center> US </center>
        </th>
        <th>
          <center> Unet </center>
        </th>
        <th>
          <center> W-Up </center>
        </th>
      </tr>
    </thread>
    <tbody>
      <tr>
        <th> <strong> Soprano </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/target_sources/target_sources_CEA_satb_15.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/cantoria/BCBSQ/US/sources_estimates_masking_CEA_satb_15.984_voice_s.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/Unet/sources_estimates_masking_CEA_satb_15.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/W-Up/sources_estimates_masking_CEA_satb_15.984_voice_s.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Alto </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/target_sources/target_sources_CEA_satb_15.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/US/sources_estimates_masking_CEA_satb_15.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/Unet/sources_estimates_masking_CEA_satb_15.984_voice_a.wav"/>
          </audio>
        </th>
         <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/W-Up/sources_estimates_masking_CEA_satb_15.984_voice_a.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/target_sources/target_sources_CEA_satb_15.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/US/sources_estimates_masking_CEA_satb_15.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/Unet/sources_estimates_masking_CEA_satb_15.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/W-Up/sources_estimates_masking_CEA_satb_15.984_voice_t.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Bass </strong> </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/target_sources/target_sources_CEA_satb_15.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/US/sources_estimates_masking_CEA_satb_15.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/Unet/sources_estimates_masking_CEA_satb_15.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/W-Up/sources_estimates_masking_CEA_satb_15.984_voice_b.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/US/mix_reconstruct_CEA_satb_15.984.wav"/>
          </audio>
        </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/cantoria/BCBSQ/W-Up/mix_reconstruct_CEA_satb_15.984.wav"/>
          </audio>
        </th>
      </tr>
    </tbody>
  </table>
</html>