---
description: didnt realize this was a real word until years later
---

# API Page

{% swagger baseUrl="https://api.cakes.com" path="/v1/cakes/:id" method="post" summary="Get Cakes" %}
{% swagger-description %}
This endpoint allows you to get free cakes.
{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="boolean" %}
ID of the cake to get, for free of course.
{% endswagger-parameter %}

{% swagger-parameter in="header" name="Authentication" type="boolean" %}
Authentication token to track down who is emptying our stocks.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="recipe" type="boolean" %}
The API will do its best to find a cake matching the provided recipe.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="gluten" type="boolean" %}
Whether the cake should be gluten-free or not.
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```javascript
{
    "name": "Cake's name",
    "recipe": "Cake's recipe name",
    "cake": "Binary cake"
}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```javascript
{
    "message": "Ain't no cake like that."
}
```
{% endswagger-response %}
{% endswagger %}

{% tabs %}
{% tab title="First Tab" %}

{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

{% swagger method="get" path="" baseUrl="test" summary="test" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" %}

{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}
