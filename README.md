[<img src='https://s3.amazonaws.com/drivendata-public-assets/logo-white-blue.png' height='70'>](https://www.drivendata.org/)
<br><br>
<img src='https://s3.amazonaws.com/drivendata-public-assets/fb-isc-koala-banner.jpg' height='200' alt='Example of original and manipulated image pair from the Challenge.'>

# Image Similarity Challenge

## Goal of the Competition
Competitors built models to help detect whether a given query image is derived from any of the images in a large reference set.

Content tracing is a crucial component on all social media platforms today, used for such tasks as flagging misinformation and manipulative advertising, preventing uploads of graphic violence, and enforcing copyright protections. But when dealing with the billions of new images generated every day on sites like Facebook, manual content moderation just doesn't scale. They depend on algorithms to help automatically flag or remove bad content.

This competition allowed participants to test their skills in building a key part of that content tracing system, and in so doing contribute to making social media more trustworthy and safe for the people who use it.

<p align="center">
<img src='https://drivendata-public-assets.s3.amazonaws.com/fb-isc-deudeuche.jpg' height='250' align='center' alt='Example of manipulations of a source image.'> 
</p>

<p class="small" align="center"><i>A reference image is manipulated to produce new images. <br>In this challenge competitors built models to detect whether a given query image is derived from a reference set.</i></p>

***

There are two tracks to this challenge:

* For the [Matching Track](https://www.drivendata.org/competitions/84/competition-image-similarity-1-final/), competitors created models that directly detect whether a query image is derived from one of the images in a large corpus of reference images.
* For the [Descriptor Track](https://www.drivendata.org/competitions/85/competition-image-similarity-2-final/), competitors generated useful vector representations of images (up to 256 dimensions). These descriptors are compared with Euclidean distance to detect whether a query image is derived from one of the images in a large corpus of reference images.


## Winning Submissions

See below for links to winning submissions' arXiv papers and code.

### Matching Track

Place | Team or User | Code	| Paper | Score | Summary of Model
--- | --- | --- | --- | --- | ---
1   | VisionForce | [GitHub repository](https://github.com/WangWenhao0716/ISC-Track1-Submission) | [D2LV: A Data-Driven and Local-Verification Approach for Image Copy Detection](https://arxiv.org/abs/2111.07090) | 0.8329 | A "data-driven and local-verification (D^2LV)" approach using pre-training on a set of basic and advanced image augmentations, and a global-local and local-global matching strategy for testing.
2   | separate | [GitHub repository](https://github.com/seungkee/2nd-place-solution-to-Facebook-Image-Similarity-Matching-Track) | [2nd Place Solution to Facebook AI Image Similarity Challenge Matching Track](https://arxiv.org/abs/2111.09113) | 0.8291 | A Vision Transformer approach that uses concatenated query and reference images to learn the relationship between query and reference images directly.
3   | imgFp | [GitHub repository](https://github.com/sun-xl/ISC2021) | [3rd Place: A Global and Local Dual Retrieval Solution to Facebook AI Image Similarity Challenge](https://arxiv.org/abs/2112.02373) | 0.7682 | A global+local recall approach with EsViT for global recall and SIFT point features for local recall.

### Descriptor Track

Place | Team or User | Code	| Paper | Score | Summary of Model
--- | --- | ---  | --- | ---  | ---
1   | lyakaap | [GitHub repository](https://github.com/lyakaap/fbisc) | Coming soon...  | 0.6354 | Uses an EfficientNet backbone trained with contrastive loss and cross-batch memory, and a training neighbor subtraction step in post-processing.   
2   | S-square | [GitHub repository](https://github.com/socom20/facebook-image-similarity-challenge-2021) | Coming soon...  | 0.5905 | Ensembles EfficientNet and NFNet backbones using an ArcFace loss function, and applies a sample normalization step in post-processing.
3   | VisionForce | [GitHub repository](https://github.com/WangWenhao0716/ISC-Track2-Submission) | [Bag of Tricks and A Strong baseline for Image Copy Detection](https://arxiv.org/abs/2111.08004) | 0.5788 | Uses a pretrained Barlow Twins model, yolov5 model to detect overlays, and a descriptor stretching step in post-processing.
