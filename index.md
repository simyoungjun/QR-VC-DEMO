---
layout: default
---



<html lang="en-US">
<head>
    <style>
        .main-content {
            max-width: 1800px; /* 원하는 최대 너비 */
            margin: 0 auto; /* 중앙 정렬 */
            padding: 0 20px; /* 좌우 패딩 */
        }
    </style>
</head>


<body data-new-gr-c-s-check-loaded="14.1001.0" data-gr-ext-installed="">


    <section class="main-content">
       
        <br><br>
        <h2 id="abstract">Abstract<a name="abstract"></a></h2>
        <p>One-shot voice conversion (VC) modifies the speaker identity of a source speech to match a target using only a single reference utterance, without requiring retraining. Recent approaches extensively utilize self-supervised learning (SSL) features with K-means quantization (KQ) to extract high-quality content representations by exploiting their structural properties. However, quantization removes fine-grained phonetic and prosodic variations as well as speaker identity, degrading intelligibility and prosody preservation. Despite this limitation, existing methods have not explored the potential of quantization residuals. This work introduces a novel approach that fully utilizes quantization residuals to disentangle speaker identity while restoring phonetic and prosodic details lost during quantization. By applying only K-means quantization and linear transformations, our method achieves effective disentanglement within a unified framework. This enables high-fidelity voice conversion while relying solely on reconstruction losses. As a result, it eliminates the need for explicit supervision and complex, non-linear deep networks in disentanglement structure. Experiments demonstrate that the proposed model outperforms existing methods while maintaining a simple linear disentanglement structure. It achieves the superior intelligibility and speaker similarity while better preserving prosody, highlighting the potential of quantization residuals in one-shot VC.</p>
        <br><br>

       
        <br><br>





        <h2 id="demos">DEMO 1. Seen-to-seen scenarios with VCTK test set<a name="demos"></a></h2>
        

        <table>
            <thead>
                <tr>
                    <th style="width: 300px; text-align: center;"><strong>Source</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Target</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Our Converted</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>FreeVC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>YourTTS</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>VQMIVC</strong></th>
                </tr>
            </thead>

            <tbody>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

            </tbody>
        </table>



        <h2 id="demos">DEMO 2. Unseen-to-unseen scenarios with LibriTTS test set<a name="demos"></a></h2>

        <table>
            <thead>
                <tr>
                    <th style="width: 300px; text-align: center;"><strong>Source</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Target</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Our Converted</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>FreeVC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>YourTTS</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>VQMIVC</strong></th>
                </tr>
            </thead>

            <tbody>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/Ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/FreeVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/YourTTS.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/VQMIVC.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>


                

            </tbody>
        </table>


        <br>
        <br>


    </section>
</body>

</html>
