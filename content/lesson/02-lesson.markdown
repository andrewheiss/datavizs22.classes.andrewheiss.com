---
title: "Graphic design"
linktitle: "2: Graphic design"
date: "2020-05-12"
menu:
  lesson:
    parent: Lessons
    weight: 2
type: docs
toc: true
bibliography: "../../static/bib/references.bib"
csl: "../../static/bib/chicago-syllabus-no-bib.csl"
editor_options: 
  chunk_output_type: console
---

## File types

Recall from the [last section of the lecture](/slides/02-slides.html#image-types) that you’ll typically work with one of two image file types: bitmap images and vector images.

Bitmaps store image information as tiny squares, or pixels. Specific files types compress these images in different ways: JPEG files smudge together groups of similarly colored pixels to save repetition, while PNG and GIF files look for fields of the exact same color.

<img src="/slides/img/02/example-bitmap.png" width="30%" />

You use bitmap images for things that go on the internet and when you place images in Word (technically modern versions of Word can handle some types of vector images, but that support isn’t universal yet).

Vector images, on the other hand, do not store image information as pixels. Instead, these use mathematical formulas to draw lines and curves and fill areas with specific colors. This makes them a little more complicated to draw and create, but it also means that you can scale them up or down infinitely—a vector image will look just as crisp on a postage stamp as it would on a billboard.

<img src="/slides/img/02/example-vector.png" width="30%" />

Here are some general guidelines:

-   If an image has lots of colors (like a photograph), you should use a bitmap file type designed for lots of colors, like JPEG. This is the case regardless of where the image will ultimately end up. If you’re putting it on the internet, it needs to be a JPEG. If you’re blowing it up to fit on a billboard, it will still need to be a JPEG (and you have to use a fancy super high quality camera to get a high enough resolution for that kind of expansion)

-   If an image has a few colors and some text and is not a photograph *and* you’re using the image in Word or on the internet, you should use a bitmap file type designed for carefully compressing a few colors, like PNG.

-   If an image has a few colors and some text and is not a photograph *and* you’re planning on using it in multiple sizes (like a logo), or using it in fancier production software like Adobe InDesign (for print) or Adobe After Effects (for video), you should use a vector file type like PDF or SVG.

## Select the best file type

Practice deciding what kind of file type you should use by looking at these images and choosing what you think works the best.

<div class="question">

<img src="/img/lesson/file-types/atlanta-sign.jpg" width="60%" />

<form name="form_1" onsubmit="return validate_form_1()" method="post">
<input type="radio" name="answer_1" id="1_1" value="PNG"><label for="1">PNG</label><br><input type="radio" name="answer_1" id="1_2" value="JPG"><label for="2">JPG</label><br><input type="radio" name="answer_1" id="1_3" value="PDF"><label for="3">PDF</label><br><input type="submit" value="Check answer">
</form>
<p id="result_1">
</p>
<script> function validate_form_1() {var x, text; var x = document.forms["form_1"]["answer_1"].value;if (x == "JPG"){text = 'Correct! This is a photograph, so it should be a JPG. It might seem a little tricky since there are so few colors, but it still needs to be a JPG because the black paint on the brick is actually a range of thousands of different shades of black pixels.';} else {text = 'Not quite—this image has a lot of colors in it…';} document.getElementById('result_1').innerHTML = text; return false;} </script>

</div>

------------------------------------------------------------------------

<div class="question">

<img src="/img/lesson/file-types/gsu-logo.png" width="60%" />

<form name="form_2" onsubmit="return validate_form_2()" method="post">
<input type="radio" name="answer_2" id="2_1" value="PNG"><label for="1">PNG</label><br><input type="radio" name="answer_2" id="2_2" value="JPG"><label for="2">JPG</label><br><input type="radio" name="answer_2" id="2_3" value="PDF"><label for="3">PDF</label><br><input type="submit" value="Check answer">
</form>
<p id="result_2">
</p>
<script> function validate_form_2() {var x, text; var x = document.forms["form_2"]["answer_2"].value;if (x == "PNG"|x == "PDF"){text = 'Correct! This is a logo with a few colors in it, so it’s vector-based. If you use a PDF of the logo, you can rescale it infinitely big or small. If you use a PNG, it will work nicely online.';} else {text = 'Not quite—this image doesn’t have a lot of colors in it…';} document.getElementById('result_2').innerHTML = text; return false;} </script>

</div>

------------------------------------------------------------------------

<div class="question">

<img src="/img/lesson/file-types/pie_chart.png" width="60%" />

<form name="form_3" onsubmit="return validate_form_3()" method="post">
<input type="radio" name="answer_3" id="3_1" value="PNG"><label for="1">PNG</label><br><input type="radio" name="answer_3" id="3_2" value="JPG"><label for="2">JPG</label><br><input type="radio" name="answer_3" id="3_3" value="PDF"><label for="3">PDF</label><br><input type="submit" value="Check answer">
</form>
<p id="result_3">
</p>
<script> function validate_form_3() {var x, text; var x = document.forms["form_3"]["answer_3"].value;if (x == "PNG"|x == "PDF"){text = 'Correct! This is a grpah with a few colors in it, so should be vector-based. If you’re using this in a fancy publication or report, use a PDF. If you’e using Word or HTML, use a PNG.';} else {text = 'Not quite—this image doesn’t have a lot of colors in it…';} document.getElementById('result_3').innerHTML = text; return false;} </script>

</div>

------------------------------------------------------------------------

<div class="question">

<img src="/img/lesson/file-types/solo.jpg" width="60%" />

<form name="form_4" onsubmit="return validate_form_4()" method="post">
<input type="radio" name="answer_4" id="4_1" value="PNG"><label for="1">PNG</label><br><input type="radio" name="answer_4" id="4_2" value="JPG"><label for="2">JPG</label><br><input type="radio" name="answer_4" id="4_3" value="PDF"><label for="3">PDF</label><br><input type="submit" value="Check answer">
</form>
<p id="result_4">
</p>
<script> function validate_form_4() {var x, text; var x = document.forms["form_4"]["answer_4"].value;if (x == "JPG"){text = 'Correct! This has a ton of colors in it and is mostly a photograph. You may have been thrown off by the text in the bottom section, or the stylized shapes of the Millennium Falcon’s windows at the top. Those shapes and the text are both vector-based, but because the majority of the image is a photogrpah, it still needs to be saved as a JPG. To keep the text nice and crisp, it needs to be exported at a high resolution.';} else {text = 'Not quite—this image has a lot of colors in it…';} document.getElementById('result_4').innerHTML = text; return false;} </script>

</div>

------------------------------------------------------------------------

<div class="question">

<img src="/img/lesson/file-types/butterflies.png" width="60%" />

<form name="form_5" onsubmit="return validate_form_5()" method="post">
<input type="radio" name="answer_5" id="5_1" value="PNG"><label for="1">PNG</label><br><input type="radio" name="answer_5" id="5_2" value="JPG"><label for="2">JPG</label><br><input type="radio" name="answer_5" id="5_3" value="PDF"><label for="3">PDF</label><br><input type="submit" value="Check answer">
</form>
<p id="result_5">
</p>
<script> function validate_form_5() {var x, text; var x = document.forms["form_5"]["answer_5"].value;if (x == "PNG"|x == "PDF"){text = 'Correct! Even though this is very colorful, it should be a PNG or PDF, since it’s vector-based and not a photograph. ';} else {text = 'Not quite—this image doesn’t have a lot of colors in it…';} document.getElementById('result_5').innerHTML = text; return false;} </script>

</div>

------------------------------------------------------------------------

<div class="question">

<img src="/img/lesson/file-types/atlanta-night.jpg" width="60%" />

<form name="form_6" onsubmit="return validate_form_6()" method="post">
<input type="radio" name="answer_6" id="6_1" value="PNG"><label for="1">PNG</label><br><input type="radio" name="answer_6" id="6_2" value="JPG"><label for="2">JPG</label><br><input type="radio" name="answer_6" id="6_3" value="PDF"><label for="3">PDF</label><br><input type="submit" value="Check answer">
</form>
<p id="result_6">
</p>
<script> function validate_form_6() {var x, text; var x = document.forms["form_6"]["answer_6"].value;if (x == "JPG"){text = 'Correct! This is a photograph and should be a JPG.';} else {text = 'Not quite—this image has a lot of colors in it…';} document.getElementById('result_6').innerHTML = text; return false;} </script>

</div>
