## Audio examples

<div class="container">
   <div class="column-1">
     <h6>Original audio signal</h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_original.wav" controls preload style="width: 190px;"></audio>
   </div>
   <div class="column-2">
     <h6>Corrupted audio signal</h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_istft_from_spectrogram.wav" controls preload style="width: 200px;"></audio>
   </div>
   <div class="column-3">
     <h6>Signal with "vyhodna" mask</h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_vyhodna.wav" controls preload style="width: 200px;"></audio>
   </div>
   <div class="column-4">
     <h6>Signal with "nevyhodna" mask</h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_nevyhodna.wav" controls preload style="width: 200px;"></audio>
   </div>
</div>

<div class="container">
   <div class="column-1">
     <h6>Audio1 (mask = diff between "vyhodna" and "nevyhodna")</h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_rozdiel_vyh_nevyh.wav" controls preload style="width: 190px;"></audio>
   </div>
   <div class="column-2">
     <h6>Audio2  (mask = 1/2 * diff between "vyhodna" and "nevyhodna")</h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_rozdiel_vyh_nevyh_div2.wav" controls preload style="width: 200px;"></audio>
   </div>
</div>

<div class="container">
   <div class="column-1">
     <h6>Audio with noise full</h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_rozdiel_vyh_nevyh.wav" controls preload style="width: 190px;"></audio>
      
   </div>
   <div class="column-2">
     <h6>Audio with noise </h6>
     <audio src="tests_vf_vs_signal/audio_without_noise/testing_audio0_rozdiel_vyh_nevyh_div2.wav" controls preload style="width: 200px;"></audio>
   </div>
</div>
