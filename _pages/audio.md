---
title: "Exemples Audio"
layout: single
permalink: /audio
author_profile: false
# classes: wide
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
excerpt: "Comparaison de différents modèles de séparation" # "Here you can find the audio files of the different pieces we worked on." - Example of a subtitle
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---
<html>

</html>


# Résultats de la séparation de sources - Apprentissage Conjoint


## Préçision technique

Nous avons expérimenté plusieurs méthodes d'entrainement pour atteindre notre objectif. Nous présentons ici les deux méthodes les plus intéressantes.
- VA_NN_1: Cette méthode consiste à entrainer le modèle de séparation en bloquant la partie __estimation de fréquences fondamentales__.  <!-- Expliquer plus que ça -->
- Warmup: Cette méthode consiste à entrainer le modèle de séparation en échauffant les différente partie séparément puis en poursuivant l'entrainement globale par la suite. <!-- Expliquer plus que ça -->

Nous comparons nos résultats au [modèle de référence](https://github.com/schufo/umss) (*US*) que nous avons modifié, et à l'architecture [*U-Net*](https://program.ismir2020.net/poster_5-14.html) de Petermann et al.

## BC1song

Pour ces résultas, nous avons entrainé les différents modèles sur la base de données __BC1Song__, et évalué sur la base de données __ChoralSingingDataset__.

> Exemple de mélange audio
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>


> Voix séparées
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

## BCBQ

Pour ces résultas, nous avons entrainé les différents modèles sur la base de données __BCBQ__, et évalué sur la base de données __ChoralSingingDataset__.

> Exemple de mélange audio
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>


> Voix séparées
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

# Résultats de l'entrainement sur des audios monophoniques

Ces résultats correspondent à l'entrainement du modèle de séparation sur des audios monophoniques. Nous avons entrainé les différents modèles sur la base de données __BCBQ__, et évalué sur la base de données __ChoralSingingDataset__.

## Mono &rarr; 2 Sources

> Exemple de mélange audio
<audio controls>
  <source src="/audio/mono/BCBSQ/mono_to_2sources/mix/mix_el_rossinyol_At_2-06_Bos_207_27.984.wav"/>
</audio>

> Voix séparées

<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center> US </center>
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

## Mono &rarr; 4 Sources

> Exemple de mélange audio
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/mix_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_27.984.wav"/>
</audio>

> Voix séparées
<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center> US </center>
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

# Généralisation sur un autre dataset - Cantoria

Pour ces résultats, nous avons entrainé les différents modèles sur la base de données __BCBQ__, et évalué sur la base de données __Cantoria__.


> Exemple de mélange audio
<audio controls="">
  <source src="/audio/cantoria/mix/mix_CEA_satb_15.984.wav"/>
</audio>


> Voix séparées
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