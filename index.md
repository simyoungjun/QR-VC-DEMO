---
layout: default
---

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
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
