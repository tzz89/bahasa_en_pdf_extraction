## Fast PDF sentence pair extraction for translation
In this repository, I have created a rule based extraction to extract bilingual sentence pairs from annual reports for finetuning a domain specific translation task. The idea is that I will use rule based extraction to extract sentence pairs in a csv format and at the same time create images with matching bboxes over the sentence pair. I will then visually inspect the pairs and remove the faulty extraction. The end result is a positive one as I was able to generate 40k sentence pairs for training in 2 days

## Algorithm used
Non- recursive X-Y cut. It turns out that if we cut the image horizontal 1 time and then vertically 1 time. It gives pretty good result

## Sample output
Click on picture to get higher resolution images
### Good Extractions
<p align="left">
<img src="assets\sample_1.jpg" height="270px" width="270px">
<img src="assets\sample_2.jpg" height="270px" width="270px">
<img src="assets\sample_3.jpg" height="270px" width="270px">
<img src="assets\sample_4.jpg" height="270px" width="270px">
<img src="assets\sample_5.jpg" height="270px" width="270px">
<img src="assets\sample_6.jpg" height="270px" width="270px">
<p>

### Faulty Extractions
<p align="left">
<img src="assets\sample_7.jpg" height="270px" width="270px">
<img src="assets\sample_8.jpg" height="270px" width="270px">
<p>


