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


<h1>Audio Table</h1>

<table border="1">
    <thead>
        <tr>
            <th></th>
            <th>Audio with noise full</th>
            <th>Audio with noise half</th>
            <th>Audio with /10 noise</th>
            <th>Audio with /20 noise</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Vyhodna</th>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_vyhodna_full.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_vyhodna_half.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_vyhodna_10.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_vyhodna_20.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>Nevyhodna</th>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_nevyhodna_full.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_nevyhodna_half.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_nevyhodna_10.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_nevyhodna_20.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>Difference</th>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel_full.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel_half.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel_10.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel_20.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>Difference/2</th>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel12_full.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel12_half.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel12_10.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="tests_vf_vs_signal/audio_with_noise/testing_audio0_noise_rozdiel12_20.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

## Comparison of DPAI and Janssen reconstruction with the same ODG metric (+-0.4) from PEMO-Q + Janssen reconstruction with "nevyhodna" mask

<h2>Example0</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example0.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example0mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example0mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example0mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example0mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example0.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example0mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example0mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example0mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example0mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example0.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example0mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example0mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example0mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example0mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example0.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example0mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example0mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example0mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example0mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example0.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example0mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example0mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example0mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example0mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example0.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example0mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example0mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example0mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example0mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

<h2>Example1</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example1mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example1mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example1mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example1mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example1mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example1mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example1mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example1mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example1mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example1mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example1mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example1mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example1mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example1mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example1mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example1mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example1mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example1mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example1mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example1mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example1mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example1mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example1mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example1mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

<h2>Example2</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example2mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example2mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example2mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example2mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example2mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example2mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example2mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example2mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example2mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example2mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example2mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example2mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example2mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example2mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example2mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example2mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example2mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example2mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example2mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example2mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example2mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example2mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example2mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example2mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

<h2>Example3</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example3mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example3mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example3mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example3mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example3mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example3mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example3mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example3mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example3mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example3mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example3mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example3mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example3mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example3mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example3mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example3mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example3mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example3mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example3mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example3mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example3mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example3mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example3mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example3mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

<h2>Example4</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example4mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example4mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example4mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example4mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example4mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example4mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example4mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example4mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example4mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example4mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example4mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example4mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example4mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example4mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example4mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example4mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example4mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example4mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example4mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example4mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example4mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example4mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example4mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example4mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

<h2>Example5</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example5mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example5mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example5mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example5mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example5mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example5mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example5mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example5mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example5mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example5mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example5mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example5mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example5mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example5mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example5mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example5mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example5mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example5mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example5mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example5mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example5mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example5mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example5mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example5mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

<h2>Example6</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example6mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example6mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example6mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example6mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example6mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example6mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example6mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example6mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example6mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example6mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example6mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example6mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example6mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example6mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example6mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example6mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example6mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example6mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example6mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example6mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example6mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example6mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example6mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example6mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>

<h2>Example7</h2>
<table border="1">
    <thead>
        <tr>
            <th>Mask</th>
            <th>Original audio</th>
            <th>Corrupted audio</th>
            <th>DPAI</th>
            <th>Janssen approx.</th>
            <th>Janssen "nevyhodna" mask</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>mask1</th>
            <td><audio src="originals/audio_original_example7.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example7mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example7mask1.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example7mask1.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example7mask1.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
        <tr>
            <th>mask2</th>
            <td><audio src="originals/audio_original_example7.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example7mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example7mask2.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example7mask2.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example7mask2.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
      <tr>
            <th>mask3</th>
           <td><audio src="originals/audio_original_example7.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example7mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example7mask3.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example7mask3.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example7mask3.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask4</th>
            <td><audio src="originals/audio_original_example7.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example7mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example7mask4.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example7mask4.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example7mask4.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask5</th>
            <td><audio src="originals/audio_original_example7.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example7mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example7mask5.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example7mask5.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example7mask5.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
       <tr>
            <th>mask6</th>
            <td><audio src="originals/audio_original_example7.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="corrupted/corrupted_audio_example7mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_best_test/audio_example7mask6.wav" controls preload style="width: 200px;"></audio></td>
            <td><audio src="dpai_odg_found/audio_example7mask6.wav" controls preload style="width: 200px;"></audio></td>
           <td><audio src="dpai_odg_nevyh/nevyh_audio_example7mask6.wav" controls preload style="width: 200px;"></audio></td>
        </tr>
    </tbody>
</table>
