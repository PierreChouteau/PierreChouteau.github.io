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

We tried our algorithm in different configurations to evaluate its efficiency. The algorithm takes a multichannel audio with all instrument playing as input, and produces 5 (1 per source) multichannel audios as if the instrument was playing alone in the room. Here we present the most interesting results for the different cases with all audios.

## Préçision technique

Nous avons expérimenté plusieurs méthodes d'entrainement pour atteindre notre objectif. Nous présentons ici les deux méthodes les plus intéressantes.
- VA_NN_1: Cette méthode consiste à entrainer le modèle de séparation en bloquant la partie __estimation de fréquences fondamentales__.  <!-- Expliquer plus que ça -->
- Warmup: Cette méthode consiste à entrainer le modèle de séparation en échauffement les différente partie séparément puis en poursuivant l'entrainement globale par la suite. <!-- Expliquer plus que ça -->

Nous comparons nos résultats au [modèle de référence](https://github.com/schufo/umss) que nous avons modifié, et à l'architecture [Unet](https://program.ismir2020.net/poster_5-14.html) de Petermann et al.

## BC1song

Pour ces résultas, nous avons entrainé les différents modèles sur la base de données __BC1Song__, et évalué sur la base de données __ChoralSingingDataset__.

> Exemple de mélange audio
<audio controls>
  <source src="/audio/Apprentissage_Conjoint/Melange/melange_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984.wav"/>
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
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_s.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_s.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_s.wav"/>
          </audio>
        </th>
      </tr>
     <tr>
        <th> <strong> Alto </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_a.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_a.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_a.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_t.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_t.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_t.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Basse </strong> </th>
        <th>
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/Apprentissage_Conjoint/Original_sources/target_sources_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_b.wav" type="audio/wav">
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Unet_Sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_b.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_b.wav"/>
          </audio>
        </th>
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/Ref_sources/sources_estimates_masking_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984_voice_b.wav"/>
          </audio>
        </th>
        <th></th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/VA_NN_1/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984.wav"/>
          </audio>
        </th>
        <th>
          <audio controls="">
            <source src="/audio/Apprentissage_Conjoint/BC1song/W_UP/mix_reconstruct_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984.wav"/>
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
  <source src="/audio/Apprentissage_Conjoint/Melange/melange_el_rossinyol_Sno_208_At_2-06_Tor2-09_Bos_207_7.984.wav"/>
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
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav" type="audio/wav">
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

# Résultats de l'entrainement sur des audios monophoniques

## Mono &rarr; 2 Sources

<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center> Ref </center>
        </th>
        <th>
          <center> 1S &rarr; 2S </center>
        </th>
        <th>
          <center> Ref </center>
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
          <audio class="px-1" controls="" controlslist="nodownload">
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav" type="audio/wav">
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
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
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
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
      </tr>
    </tbody>
  </table>
</html>

## Mono &rarr; 4 Sources

<html>
  <table>
    <thread>
      <tr>
        <th>
          <!-- <center> Voice </center> -->
        </th>
        <th>
          <center> Ref </center>
        </th>
        <th>
          <center> 1S &rarr; 4S </center>
        </th>
        <th>
          <center> Ref </center>
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
            <source src="/audio/no_effect_audios/no_separation/micro_Violin1.wav" type="audio/wav">
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
      </tr>
      <tr>
        <th> <strong> Tenor </strong> </th>
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
      </tr>
      <tr>
        <th> <strong> Re-synthesized mix </strong> </th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
        <th>Test</th>
      </tr>
    </tbody>
  </table>
</html>

# Généralisation sur un autre dataset - Cantoria

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