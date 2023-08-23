---
title: "Exemples Audio"
layout: single
permalink: /audio
author_profile: false
# classes: wide
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
excerpt: "Résultats d'expériences" # "Here you can find the audio files of the different pieces we worked on." - Example of a subtitle
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---
<html>

</html>


<!-- Pour ce projet, nous avons proposé un modèle d'apprentissage profond non supervisé pour de la séparation de sources musicales. Celui-ci est basé sur le modèle de séparation de sources __US__ de [Schulze-Foster et al.](https://ieeexplore.ieee.org/document/10058592), mais contrairement à ce dernier, il n'utilise aucune connaissance *a priori* sur les fréquences fondamentales des sources.

Notre approche se base sur des modèles pré-entrainés, pour intégrer l'estimation des fréquences fondamentales à l'intérieur du modèle __US__, et nous avons expérimenté plusieurs méthodes d'entrainement pour atteindre notre objectif. 

Nous présentons ici les résultats des deux méthodes les plus intéressantes : 
- VA_NN_2
- Warmup

Les détails d'implémentation et de fonctionnement sont disponible dans le __rapport__.


Nous comparons nos résultats au modèle __US__ de Schulze-Foster et al., et à l'architecture [__U-Net__](https://program.ismir2020.net/poster_5-14.html) de Petermann et al. -->


Bienvenue sur la page des exemples audio. Vous trouverez ici les résultats de nos expériences, ainsi que des exemples audio de séparation de sources musicales.

Pour les expériences où notre architecture est comparée aux modèles [__US__](https://ieeexplore.ieee.org/document/10058592) de Schulze-Foster et al. et [__U-Net__](https://program.ismir2020.net/poster_5-14.html) de Petermann et al., nous ne montrons que nos deux meilleurs approches: 
- __VA_NN_2__
- __Warmup__.



<br/>

---
# Résultats de la séparation de sources - Apprentissage Conjoint

## BC1song

Pour ces résultas, nous avons entrainé les différents modèles sur la base de données __BC1Song__, et évalué sur la base de données __ChoralSingingDataset__.

> Exemple de mélange audio
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>


> Voix séparées issues du filtrage de Wiener
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
        <th> <strong> Basse </strong> </th>
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
        <th> <strong> Mélange re-synthétisé </strong> </th>
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

Pour ces résultas, nous avons entrainé les différents modèles sur la base de données __BCBSQ__, et évalué sur la base de données __ChoralSingingDataset__.

> Exemple de mélange audio
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>


> Voix séparées issues du filtrage de Wiener
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
        <th> <strong> Basse </strong> </th>
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
        <th> <strong> Mélange re-synthétisé </strong> </th>
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
# Résultats de l'entrainement sur des audios monophoniques

Ces résultats correspondent à l'entrainement du modèle de séparation sur des audios monophoniques. Nous avons entrainé les différents modèles sur la base de données __BCBQ__, et évalué sur la base de données __ChoralSingingDataset__.

## Mono &rarr; 2 Sources

> Exemple de mélange audio - Alto / Basse
<audio controls>
  <source src="/audio/mono/BCBSQ/mono_to_2sources/mix/mix_el_rossinyol_At_2-06_Bos_207_27.984.wav"/>
</audio>

> Voix séparées issues du filtrage de Wiener
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
        <th> <strong> Basse </strong> </th>
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
        <th> <strong> Mélange re-synthétisé </strong> </th>
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

> Exemple de mélange audio - Soprano / Alto
<audio controls>
  <source src="/audio/mono/BCBSQ/mono_to_2sources/mix/mix_el_rossinyol_Sno_208_At_2-06_27.984.wav"/>
</audio>

> Voix séparées issues du filtrage de Wiener
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
        <th> <strong> Mélange re-synthétisé </strong> </th>
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

> Exemple de mélange audio - Tenor / Basse
<audio controls>
  <source src="/audio/mono/BCBSQ/mono_to_2sources/mix/mix_el_rossinyol_Tor2-09_Bos_207_27.984.wav"/>
</audio>

> Voix séparées issues du filtrage de Wiener
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
        <th> <strong> Basse </strong> </th>
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
        <th> <strong> Mélange re-synthétisé </strong> </th>
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

> Exemple de mélange audio
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>

> Voix séparées issues du filtrage de Wiener
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
        <th> <strong> Basse </strong> </th>
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
        <th> <strong> Mélange re-synthétisé </strong> </th>
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
# Généralisation sur un autre base de données - Cantoria

Pour ces résultats, nous avons entrainé les différents modèles sur la base de données __BCBSQ__, et évalué sur la base de données __Cantoria__.


> Exemple de mélange audio
<audio controls="">
  <source src="/audio/cantoria/mix/mix_CEA_satb_15.984.wav"/>
</audio>


> Voix séparées issues du filtrage de Wiener
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
        <th> <strong> Basse </strong> </th>
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
        <th> <strong> Mélange re-synthétisé </strong> </th>
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