---
title: 更新 apiConnectorConfiguration
description: 通过更新 apiConnectorConfiguration 属性，启用或禁用用户流中的特定步骤的 API 连接器。
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 59630072a82f923938b9e7b3834e039a108491e4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442440"
---
# <a name="update-apiconnectorconfiguration"></a>更新 apiConnectorConfiguration

命名空间：microsoft.graph

更新 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 中的 [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) 属性，以在用户流中启用或禁用 API 连接器。 [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) 的每个关系对应于可配置为调用 API 连接器的用户流中的特定步骤。 一次为特定步骤一个配置 API 连接器，如下所示。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityUserFlow.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|Application|IdentityUserFlow.ReadWrite.All|

工作或学校帐户需要属于以下角色之一：

* 全球管理员
* 外部标识用户流管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供要使用特定步骤的 `id` [identityApiConnector](../resources/identityapiconnector.md) 的 JSON 表示形式。 若要禁用 API 连接器，可以是 {}值。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a>示例 1：注册后 IDP 联合身份验证启用 API 连接器

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应 

下面展示了示例响应。

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a>示例 2：注册后属性集合启用 API 连接器

#### <a name="request"></a>请求 

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a>示例 3：注册后禁用 Post Attribute Collection 的 API 连接器

#### <a name="request"></a>请求 

下面展示了示例请求。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
