---
layout: default
---


This page is the official demo for the paper "SKQVC: One-Shot Voice Conversion by K-Means Quantization with Self-Supervised Speech Representations."


### Abstract
One-shot voice conversion (VC) is a method that enables the transformation between any two speakers using only a single target speaker utterance. Existing methods often rely on complex architectures and external speaker embeddings derived from pre-trained speaker verification (SV) models to enhance the fidelity in converted speech. Recent works employing K-means quantization (KQ) with self-supervised learning (SSL) features have demonstrated effectiveness in capturing content information. However, they often struggle to preserve speaking variation, including prosodic details and phonetic variation that change within an utterance, particularly when using smaller codebooks. In this work, we propose a simple yet effective one-shot VC model using characteristics of SSL features and speech attributes. Our approach addresses the issue of losing speaking variation, enabling high-fidelity voice conversion trained with only reconstruction-based losses. We demonstrated the performance of our model across six evaluation metrics, and the experiments highlight the benefits of the speaking variation compensation method.


| **Source** | **Target** | **Ours Converted** | **FreeVC** | **YourTTS** | **VQMIVC** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| <audio src="all/MOS/VCTK/src;p227_044&tgt;p300_388/src.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p227_044&tgt;p300_388/tgt.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p227_044&tgt;p300_388/Ours.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p227_044&tgt;p300_388/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p227_044&tgt;p300_388/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p227_044&tgt;p300_388/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/src.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/tgt.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/Ours.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p240_246&tgt;p335_399/VQMIVC.wav" controls preload></audio> |
| --- | --- | --- | --- | --- | --- |
| <audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/src.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/tgt.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/Ours.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p246_092&tgt;p241_354/VQMIVC.wav" controls preload></audio> |
| --- | --- | --- | --- | --- | --- |
| <audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/src.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/tgt.wav" controls preload></audio> | <audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/Ours.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/VCTK/src;p232_410&tgt;p308_187/VQMIVC.wav" controls preload></audio> |
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/src.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/tgt.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/Ours.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p228_268&tgt;p275_061/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/src.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/tgt.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/Ours.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p244_308&tgt;p276_276/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/src.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/tgt.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/Ours.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p274_100&tgt;p244_031/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/src.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/tgt.wav" controls preload></audio> | <audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/Ours.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/VCTK/src;p274_260&tgt;p274_101/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |


### DEMO ( Seen Source and Target, both of them are random sampled, and converted by only one utterance)

| **Source** | **Target** | **Ours Converted** | **FreeVC** | **YourTTS** | **VQMIVC** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| <audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/src.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/tgt.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/Ours.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;1320_122612_000035_000007&tgt;1995_1826_000036_000000/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/src.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/tgt.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/Ours.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;5683_32866_000035_000001&tgt;3729_6852_000078_000003/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/src.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/tgt.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/Ours.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;7021_85628_000034_000000&tgt;4992_41797_000012_000000/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/src.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/tgt.wav" controls preload></audio> | <audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/Ours.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/FreeVC.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/YourTTS.wav" controls preload></audio> |<audio src="all/MOS/LibriTTS/src;8455_210777_000061_000003&tgt;1320_122617_000022_000001/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/src.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/tgt.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/Ours.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;121_127105_000041_000001&tgt;1284_1181_000031_000000/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/src.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/tgt.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/Ours.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;1188_133604_000018_000000&tgt;1580_141083_000031_000000/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/src.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/tgt.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/Ours.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;3575_170457_000024_000016&tgt;4970_29093_000033_000000/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |
| <audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/src.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/tgt.wav" controls preload></audio> | <audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/Ours.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/FreeVC.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/YourTTS.wav" controls preload></audio> |<audio src="all/SMOS/LibriTTS/src;7127_75947_000080_000000&tgt;1995_1837_000020_000000/VQMIVC.wav" controls preload></audio> 
| --- | --- | --- | --- | --- | --- |


<!DOCTYPE html>
<html lang="en-US">


<body data-new-gr-c-s-check-loaded="14.1001.0" data-gr-ext-installed="">
    <section class="page-header">
        <!-- <h1 class="project-name">Demo PAGE</h1> -->
        <!-- <h2 class="project-tagline"></h2> -->
    </section>

    <section class="main-content">
        <table border=0 frame=void rules=none>
            <tr>
                <td>
                    <center><img src='fig/overview.png' width="40%"></center>
                    <br>
                    <center><span><b>Figure 1. Overview of Vec-Tok-VC+</b></span></center>
                </td>
            </tr>
            <tr><br></tr>
            <tr>
                <td>
                    <center><img src='fig/components.png' width="50%"></center>
                    <br>
                    <center><span><b>Figure 2. The details of Vec-Tok-VC+. (a): the residual-enhanced K-Means decoupler. (b): the dual-mode teacher guidance module. (c): the converter and multi-codebook progressive constraint.</b></span> </center>
                </td>
            </tr>

        </table>
        <br><br>





        <h2 id="demos">1. Demo: Intra-lingual Zero-shot Voice Conversion<a name="demos"></a></h2>
        

        <table>
            <thead>
                <tr>
                    <th style="width: 300px; text-align: center;"><strong>Source speech</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Target speaker</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>LM-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>SEF-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Vec-Tok-VC+ (Our proposed)</strong></th>
                </tr>
            </thead>

            <tbody>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/hvd_717_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/00993_single.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/993/hvd_717_1_00993_single.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/993/hvd_717_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/993/hvd_717_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/TIM_305.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/00993_single.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/993/TIM_305_00993_single.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/993/TIM_305.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/993/TIM_305.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/hvd_705_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/TIM_315.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/TIM/hvd_705_1_TIM_315.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/TIM/hvd_705_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/TIM/hvd_705_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/king_033_600492.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/TIM_315.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/TIM/king_033_600492_TIM_315.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/TIM/king_033_600492.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/TIM/king_033_600492.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/404042.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/LY-8.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/LY/404042_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/LY/404042_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/LY/404042.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/0302001002.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/LY-8.wav" controls="" preload="" style="width: 100%;"></audio></td>                   
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/LY/0302001002_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/LY/0302001002_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/LY/0302001002.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/2702010002.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/vo_zhongli_friendship_04.wav" controls="" preload="" style="width: 100%;"></audio></td>              
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/zhongli/2702010002.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/zhongli/2702010002.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/zhongli/2702010002.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/404046.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/vo_zhongli_friendship_04.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/zhongli/404046.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/zhongli/404046.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/zhongli/404046.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

            </tbody>
        </table>



        <h2 id="demos">2. Demo: Cross-lingual Zero-shot Voice Conversion<a name="demos"></a></h2>

        <table>
            <thead>
                <tr>
                    <th style="width: 300px; text-align: center;"><strong>Source speech</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Target speaker</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>LM-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>SEF-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Vec-Tok-VC+ (Our proposed)</strong></th>
                </tr>
            </thead>

            <tbody>


                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/king_033_600486.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/vo_zhongli_friendship_04.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/zhongli/king_033_600486_vo_zhongli_friendship_04.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/zhongli/king_033_600486.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/zhongli/king_033_600486.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/TIM_309.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/vo_zhongli_friendship_04.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/zhongli/TIM_309_vo_zhongli_friendship_04.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/zhongli/TIM_309.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/zhongli/TIM_309.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>
              
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/hvd_701_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/LY-8.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/LY/hvd_701_1_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/LY/hvd_701_1_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/LY/hvd_701_1.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/king_033_600482.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/LY-8.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/LY/king_033_600482_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/LY/king_033_600482_LY.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/LY/king_033_600482.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>


                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/404042.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/00993_single.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/993/404042.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/993/404042_993.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/993/404042.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/0301001005.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/00993_single.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/993/0301001005.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/993/0301001005.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/993/0301001005.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/401092.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/TIM_315.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/TIM/401092.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/TIM/401092.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/TIM/401092.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/0303001004.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/TIM_315.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/LM-VC/TIM/0303001004.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/SEF-VC/TIM/0303001004.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/TIM/0303001004.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>
            </tbody>
        </table>





        <h2 id="demos">3. Demo: Noise-robust Zero-shot Voice Conversion<a name="demos"></a></h2>

        <table>
            <thead>
                <tr>
                    <th style="width: 300px; text-align: center;"><strong>Source speech</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>Target speaker</strong></th>
                    <!-- <th style="width: 300px; text-align: center;"><strong>SEF-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>LM-VC</strong></th> -->
                    <th style="width: 300px; text-align: center;"><strong>Vec-Tok-VC+ (Our proposed)</strong></th>
                </tr>
            </thead>

            <tbody>
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/489.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/db1_002982.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <!-- <td style="width: 300px; text-align: center;"><audio src="" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="" controls="" preload="" style="width: 100%;"></audio></td> -->
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/noise/489.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/619.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/db1_002982.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <!-- <td style="width: 300px; text-align: center;"><audio src="" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="" controls="" preload="" style="width: 100%;"></audio></td> -->
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/noise/619.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>


              
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="demos/src/364.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="demos/target_n/db1_002982.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <!-- <td style="width: 300px; text-align: center;"><audio src="" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="" controls="" preload="" style="width: 100%;"></audio></td> -->
                    <td style="width: 300px; text-align: center;"><audio src="demos/Proposed/noise/364.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>


            </tbody>
        </table>


        <br>
        <br>



        <footer class="site-footer">
            <span class="site-footer-credits">This page was generated by <a href="https://pages.github.com/">GitHubPages</a>.</span>
        </footer>
    </section>
</body>

</html>
