# Template for _model card_

This is a template for a [model card for model reporting](https://arxiv.org/abs/1810.03993).

The template is [here](./model-card-template.md).

## What is a model card?

[Model cards for model reporting](https://arxiv.org/abs/1810.03993) were created to increase
transparency of models.

The problem it is trying to solve:

> Currently, there are no standardized documentation procedures to communicate the performance
> characteristics of trained machine learning (ML) and artificial intelligence (AI) models.
> This lack of documentation is especially problematic when models are used in applications that
> have serious impacts on people’s lives such as in health care, employment, education and law
> enforcement.

## Why use a markdown file for the datasheet?

The short explanation: using a markdown file allows us to easily compare (diff) one version
of the model card with another version. 

The longer explanation:

Models should be under version control, in the same way we put the code under version
control. Once under version control, we can compare one version against the other.

It is easier to follow the changes in a model when its model card is distributed together
with the model. If the model is under source control, so should be its model card.

Whenever there is a new version of the model, we also need to update its description.
In other words, we need to update its model card.

The model card distributed with a version should be in a format that is easy to compare with
previous version, to allow us to quickly see what has been changed. Markdown is simple, text
format, making it ideal for that.

## Examples of model cards

- [GPT-2](https://github.com/openai/gpt-2/blob/master/model_card.md)
- Google's interactive model cards for [face detection](https://modelcards.withgoogle.com/face-detection)
  and [object detection](https://modelcards.withgoogle.com/object-detection)


