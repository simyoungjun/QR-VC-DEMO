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
                    <th style="width: 300px; text-align: center;"><strong>DDDM-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>kNN-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>SEF-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>SSR-VC</strong></th>
                </tr>
            </thead>

            <tbody>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;61-70968-0000&tgt;2300-131720-0028/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0018&tgt;4446-2275-0016/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0018&tgt;4446-2275-0016/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0018&tgt;4446-2275-0016/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0018&tgt;4446-2275-0016/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0018&tgt;4446-2275-0016/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0018&tgt;4446-2275-0016/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0018&tgt;4446-2275-0016/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0045&tgt;3575-170457-0032/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0045&tgt;3575-170457-0032/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0045&tgt;3575-170457-0032/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0045&tgt;3575-170457-0032/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0045&tgt;3575-170457-0032/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0045&tgt;3575-170457-0032/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0045&tgt;3575-170457-0032/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0056&tgt;8455-210777-0031/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0056&tgt;8455-210777-0031/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0056&tgt;8455-210777-0031/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0056&tgt;8455-210777-0031/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0056&tgt;8455-210777-0031/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0056&tgt;8455-210777-0031/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;672-122797-0056&tgt;8455-210777-0031/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;908-157963-0027&tgt;237-126133-0010/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;908-157963-0027&tgt;237-126133-0010/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;908-157963-0027&tgt;237-126133-0010/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;908-157963-0027&tgt;237-126133-0010/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;908-157963-0027&tgt;237-126133-0010/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;908-157963-0027&tgt;237-126133-0010/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;908-157963-0027&tgt;237-126133-0010/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;8463-294828-0004&tgt;8224-274384-0001/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;8463-294828-0004&tgt;8224-274384-0001/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;8463-294828-0004&tgt;8224-274384-0001/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;8463-294828-0004&tgt;8224-274384-0001/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;8463-294828-0004&tgt;8224-274384-0001/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;8463-294828-0004&tgt;8224-274384-0001/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;8463-294828-0004&tgt;8224-274384-0001/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;7021-85628-0004&tgt;908-157963-0001/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;7021-85628-0004&tgt;908-157963-0001/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;7021-85628-0004&tgt;908-157963-0001/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;7021-85628-0004&tgt;908-157963-0001/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;7021-85628-0004&tgt;908-157963-0001/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;7021-85628-0004&tgt;908-157963-0001/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;7021-85628-0004&tgt;908-157963-0001/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;4970-29095-0031&tgt;1995-1837-0006/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;4970-29095-0031&tgt;1995-1837-0006/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;4970-29095-0031&tgt;1995-1837-0006/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;4970-29095-0031&tgt;1995-1837-0006/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;4970-29095-0031&tgt;1995-1837-0006/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;4970-29095-0031&tgt;1995-1837-0006/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;4970-29095-0031&tgt;1995-1837-0006/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;3729-6852-0037&tgt;1221-135766-0010/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;3729-6852-0037&tgt;1221-135766-0010/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;3729-6852-0037&tgt;1221-135766-0010/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;3729-6852-0037&tgt;1221-135766-0010/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;3729-6852-0037&tgt;1221-135766-0010/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;3729-6852-0037&tgt;1221-135766-0010/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;3729-6852-0037&tgt;1221-135766-0010/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>
                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;2094-142345-0051&tgt;5142-33396-0053/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;2094-142345-0051&tgt;5142-33396-0053/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;2094-142345-0051&tgt;5142-33396-0053/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;2094-142345-0051&tgt;5142-33396-0053/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;2094-142345-0051&tgt;5142-33396-0053/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;2094-142345-0051&tgt;5142-33396-0053/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="MOS/src;2094-142345-0051&tgt;5142-33396-0053/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
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
                    <th style="width: 300px; text-align: center;"><strong>DDDM-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>kNN-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>SEF-VC</strong></th>
                    <th style="width: 300px; text-align: center;"><strong>SSR-VC</strong></th>
                </tr>
            </thead>

            <tbody>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0004&tgt;8455-210777-0004/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0004&tgt;8455-210777-0004/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0004&tgt;8455-210777-0004/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0004&tgt;8455-210777-0004/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0004&tgt;8455-210777-0004/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0004&tgt;8455-210777-0004/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0004&tgt;8455-210777-0004/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0026&tgt;237-134493-0011/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0026&tgt;237-134493-0011/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0026&tgt;237-134493-0011/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0026&tgt;237-134493-0011/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0026&tgt;237-134493-0011/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0026&tgt;237-134493-0011/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;121-127105-0026&tgt;237-134493-0011/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;237-126133-0012&tgt;5142-36377-0020/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;237-126133-0012&tgt;5142-36377-0020/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;237-126133-0012&tgt;5142-36377-0020/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;237-126133-0012&tgt;5142-36377-0020/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;237-126133-0012&tgt;5142-36377-0020/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;237-126133-0012&tgt;5142-36377-0020/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;237-126133-0012&tgt;5142-36377-0020/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0017&tgt;5105-28240-0016/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0017&tgt;5105-28240-0016/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0017&tgt;5105-28240-0016/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0017&tgt;5105-28240-0016/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0017&tgt;5105-28240-0016/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0017&tgt;5105-28240-0016/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0017&tgt;5105-28240-0016/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0013&tgt;4507-16021-0001/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0013&tgt;4507-16021-0001/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0013&tgt;4507-16021-0001/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0013&tgt;4507-16021-0001/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0013&tgt;4507-16021-0001/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0013&tgt;4507-16021-0001/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;8555-284447-0013&tgt;4507-16021-0001/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;5142-33396-0000&tgt;1221-135767-0022/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;5142-33396-0000&tgt;1221-135767-0022/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;5142-33396-0000&tgt;1221-135767-0022/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;5142-33396-0000&tgt;1221-135767-0022/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;5142-33396-0000&tgt;1221-135767-0022/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;5142-33396-0000&tgt;1221-135767-0022/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;5142-33396-0000&tgt;1221-135767-0022/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4970-29093-0019&tgt;5639-40744-0029/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4970-29093-0019&tgt;5639-40744-0029/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4970-29093-0019&tgt;5639-40744-0029/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4970-29093-0019&tgt;5639-40744-0029/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4970-29093-0019&tgt;5639-40744-0029/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4970-29093-0019&tgt;5639-40744-0029/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4970-29093-0019&tgt;5639-40744-0029/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4507-16021-0051&tgt;6930-76324-0009/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4507-16021-0051&tgt;6930-76324-0009/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4507-16021-0051&tgt;6930-76324-0009/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4507-16021-0051&tgt;6930-76324-0009/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4507-16021-0051&tgt;6930-76324-0009/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4507-16021-0051&tgt;6930-76324-0009/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;4507-16021-0051&tgt;6930-76324-0009/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;3729-6852-0022&tgt;7729-102255-0044/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;3729-6852-0022&tgt;7729-102255-0044/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;3729-6852-0022&tgt;7729-102255-0044/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;3729-6852-0022&tgt;7729-102255-0044/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;3729-6852-0022&tgt;7729-102255-0044/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;3729-6852-0022&tgt;7729-102255-0044/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;3729-6852-0022&tgt;7729-102255-0044/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>

                <tr>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;2961-961-0003&tgt;5142-33396-0043/src.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;2961-961-0003&tgt;5142-33396-0043/tgt.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;2961-961-0003&tgt;5142-33396-0043/ours.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;2961-961-0003&tgt;5142-33396-0043/dddmvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;2961-961-0003&tgt;5142-33396-0043/knnvc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;2961-961-0003&tgt;5142-33396-0043/sef-vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                    <td style="width: 300px; text-align: center;"><audio src="SMOS/src;2961-961-0003&tgt;5142-33396-0043/ssr_vc.wav" controls="" preload="" style="width: 100%;"></audio></td>
                </tr>


                

            </tbody>
        </table>


        <br>
        <br>


    </section>
</body>

</html>
