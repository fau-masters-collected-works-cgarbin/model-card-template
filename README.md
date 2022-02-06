# Template for _model card_

This is a template for a [model card for model reporting](https://arxiv.org/abs/1810.03993).

The template is [here](./model-card-template.md).

## What is a model card?

[Model cards for model reporting](https://arxiv.org/abs/1810.03993) was created to increase
transparency of models.

> [Model cards are] short documents accompanying trained machine learning models that provide
> benchmarked evaluation in a variety of conditions, such as across different cultural, demographic,
> or phenotypic groups ... and intersectional groups ... that are relevant to the intended application
> domains. Model cards also disclose the context in which models are intended to be used, details of
> the performance evaluation procedures, and other relevant information.}

The problem it is trying to solve:

> Currently, there are no standardized documentation procedures to communicate the performance
> characteristics of trained machine learning (ML) and artificial intelligence (AI) models.
> This lack of documentation is especially problematic when models are used in applications that
> have serious impacts on people’s lives such as in health care, employment, education and law
> enforcement.

One of the main concerns of model cards is _ethics_. As such, it emphasizes metrics across intersectional groups.
That is, performance not only in the obvious, larger groups, such as male vs. female, but also in
combinations of those groups, "male, Fitzpatrick skin type I" vs. "male, Fitzpatrick skin type V", or
"female, ages 18-34" vs. "female, ages 35-50". Disaggregating the measures of a model before putting it
in production can prevent embarrassing and potentially harmful errors, such as the very public shaming
of Microsoft and IBM in the [Gender Shades paper](http://proceedings.mlr.press/v81/buolamwini18a/buolamwini18a.pdf)
and accompanying [MIT Media Lab's website](http://gendershades.org/).

## Why use a markdown file for the model card?

The short explanation: using a markdown file allows us to compare (diff) easily one version
of the model card with another version. 

The longer explanation:

Models should be under version control, in the same way we put the code under version
control. Once under version control, we can compare one version against the other.

It is easier to follow the changes in a model when its model card is distributed together
with the model. If the model is under source control, so should be its model card.

Whenever there is a new version of the model, we also need to update its description.
In other words, we need to update its model card.

The model card distributed with a version should be in a format that is easy to compare with
previous versions, to allow us to quickly see what has been changed. Markdown is a simple, text
format, making it ideal for that.

## Examples of model cards

- [CheXNet](https://github.com/fau-masters-collected-works-cgarbin/chexnet-model-card)
- Google's interactive model cards for [face detection](https://modelcards.withgoogle.com/face-detection)
  and [object detection](https://modelcards.withgoogle.com/object-detection)
- NVIDIA's [DashCamNet](https://catalog.ngc.nvidia.com/orgs/nvidia/models/tlt_dashcamnet)
- OpenAI's [GPT-3](https://github.com/openai/gpt-3/blob/master/model-card.md) and [CLIP](https://github.com/openai/CLIP/blob/main/model-card.md)

