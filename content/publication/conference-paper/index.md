---
title: Repeated Knowledge Distillation with Confidence Masking to Mitigate
  Membership Inference Attacks
authors:
  - Federico Mazzone
  - Leander van den Heuvel
  - Maximilian Huber
  - Cristian Verdecchia
  - Maarten Everts
  - Florian Hahn
  - Andreas Peter
author_notes:
  - First Author
  - Second autor
publication_short: In AISEC
abstract: Machine learning models are often trained on sensitive data, such as
  medical records or bank transactions, posing high privacy risks. In fact,
  membership inference attacks can use the model parameters or predictions to
  determine whether a given data point was part of the training set. One of the
  most promising mitigations in literature is Knowledge Distillation (KD). This
  mitigation consists of first training a teacher model on the sensitive private
  dataset, and then transferring the teacher knowledge to a student model, by
  the mean of a surrogate dataset. The student model is then deployed in place
  of the teacher model. Unfortunately, KD on its own does not provide users much
  flexibility, meant as the possibility to arbitrarily decide how much utility
  to sacrifice to get membership-privacy. To address this problem, we propose a
  novel approach that combines KD with confidence score masking. Concretely, we
  repeat the distillation procedure multiple times in series and, during each
  distillation, perturb the teacher predictions using confidence masking
  techniques. We show that our solution provides more flexibility than standard
  KD, as it allows users to tune the number of distillation rounds and the
  strength of the masking function. We implement our approach in a tool, RepKD,
  and assess our mitigation against white- and black-box attacks on multiple
  models and datasets. Even when the surrogate dataset is different from the
  private one (which we believe to be a more realistic setting than is commonly
  found in literature), our mitigation is able to make the black-box attack
  completely ineffective and significantly reduce the accuracy of the white-box
  attack at the cost of only 0.6% test accuracy loss.
tags:
  - Membership
  - inference
  - attacks
  - ai
  - security
projects: []
slides: ""
url_pdf: ""
publication_types:
  - "3"
image:
  preview_only: false
summary: Migitate Membership attacks using repeated knowledge distillation.
url_dataset: ""
url_project: https://aisec.cc
url_source: https://dl.acm.org/doi/10.1145/3560830.3563721
url_video: ""
publication: In ACM Workshop on Artificial Intelligence and Security
featured: true
date: 2022-11-15T00:00:00Z
url_slides: ""
publishDate: 2022-11-15T12:00:00Z
url_poster: ""
url_code: ""
doi: ""
---

{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/).
