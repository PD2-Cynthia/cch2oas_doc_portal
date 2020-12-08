# 取得會員訊息未讀數

{% api-method method="post" host="http://domain name/cch2oas" path="/portal/message/unread" %}
{% api-method-summary %}
 取得訊息未讀數
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="lang" type="string" required=true %}
zh\_CN
{% endapi-method-parameter %}

{% api-method-parameter name="role" type="string" required=true %}
Portal
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="portalVendorId" type="string" required=true %}
PortalVENDORID使用AES加密後\(AES/ECB/PKCS5Padding\)，再用Base64加密傳出
{% endapi-method-parameter %}

{% api-method-parameter name="portalKey" type="string" required=true %}
PortalVENDORKey使用AES加密後\(AES/ECB/PKCS5Padding\)，再用Base64加密傳出
{% endapi-method-parameter %}

{% api-method-parameter name="portalUserAccount" type="string" required=true %}
portal登入賬號
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "code": 200,
    "exceptionCode": 0,
    "message": "取得资料成功",
    "token": null,
    "data": {
        "unreadCount": 2
    },
    "resourceKey": "api.response.code.getSuccess",
    "isOK": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



