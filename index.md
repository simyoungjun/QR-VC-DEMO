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

        /* 🔧 [추가] 테이블 가로 스크롤과 오디오 셀 간격 */
        .table-scroll-wrapper {
            overflow-x: auto;
            white-space: nowrap;
            padding-bottom: 1em;
        }

        .audio-table {
            border-collapse: collapse;
            width: max-content;
            min-width: 100%;
        }

        .audio-table th,
        .audio-table td {
            padding: 16px; /* 🔧 간격 넓히기 */
            text-align: center;
            width: 300px;
        }

        .audio-table audio {
            width: 100%;
        }
        
    </style>
</head>


<body data-new-gr-c-s-check-loaded="14.1001.0" data-gr-ext-installed="">


    <section class="main-content">
       
        <br><br>
        <h2 id="abstract">Abstract<a name="abstract"></a></h2>
        <p>Zero-shot voice conversion is a technique that alters the speaker identity of an input speech to match a target speaker using only a single reference utterance, without requiring additional training. Recent approaches extensively utilize self-supervised learning features with K-means quantization to extract high-quality content representations while removing speaker identity. However, this quantization process also eliminates fine-grained phonetic and prosodic variations, degrading intelligibility and prosody preservation. While prior works have primarily focused on quantized representations, quantization residuals remain underutilized and deserve further exploration. In this paper, we introduce a novel approach that fully utilizes quantization residuals by leveraging temporal properties of speech components. This facilitates the disentanglement of speaker identity and the recovery of phonetic and prosodic details lost during quantization. By applying only K-means quantization and linear projections, our method achieves simple yet effective disentanglement, without requiring complex architectures or explicit supervision. This allows for high-fidelity voice conversion trained solely with reconstruction losses. Experiments show that the proposed model outperforms existing methods across both subjective and objective metrics. It achieves superior intelligibility and speaker similarity, along with improved prosody preservation, highlighting the impact of our Linear Disentangler module.</p>
        <br><br>

       
        <br><br>



        <h2 id="demos">DEMO: Comparison with baseline models on LibriTTS test dataset<a name="demos"></a></h2>

        
        
        <div class="table-scroll-wrapper">
            <table class="audio-table">
                <thead>
                    <tr>
                            <th><strong>Source</strong></th>
                            <th><strong>Target</strong></th>
                            <th><strong>Our Converted</strong></th>
                            <th><strong>DDDM-VC</strong></th>
                            <th><strong>Phoneme Hallucinator</strong></th>
                            <th><strong>kNN-VC</strong></th>
                            <th><strong>SEF-VC</strong></th>
                            <th><strong>SSR-VC</strong></th>
                    </tr>
                </thead>
    
                <tbody>

                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;237-126133-0012&tgt;5142-36377-0020/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>

                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;672-122797-0056&tgt;8455-210777-0031/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>

                    <tr>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 500px; text-align: center;"><audio src="sample/src;61-70968-0000&tgt;2300-131720-0028/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;121-127105-0004&tgt;8455-210777-0004/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
                    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;908-157963-0027&tgt;237-126133-0010/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2094-142345-0051&tgt;5142-33396-0053/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;2961-961-0003&tgt;5142-33396-0043/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;3729-6852-0037&tgt;1221-135766-0010/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;4507-16021-0051&tgt;6930-76324-0009/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;5142-33396-0000&tgt;1221-135767-0022/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                    <tr>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/phoneme_hallucinator_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/knnvc_vol07.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                        <td style="width: 300px; text-align: center;"><audio src="sample/src;8555-284447-0017&tgt;5105-28240-0016/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    </tr>
    
                </tbody>
            </table>
        </div>


        <br>
        <br>


    </section>
</body>

</html>
