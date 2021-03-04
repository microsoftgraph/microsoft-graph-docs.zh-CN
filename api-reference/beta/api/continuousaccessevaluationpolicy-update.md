---
title: 更新 continuousAccessEvaluationPolicy
description: 更新 continuousAccessEvaluationPolicy 对象的属性。
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 80c08c4b711daa2e79600c20ce11f30cd7879af4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437280"
---
# <a name="update-continuousaccessevaluationpolicy"></a>更新 continuousAccessEvaluationPolicy
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）                    |
|:--------------------------------------|:---------------------------------------------------------------|
|委派（工作或学校帐户）     | Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All |

> [!NOTE]
> 此 API 有 [一个与](/graph/known-issues#permissions) 权限相关的已知问题。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

|属性|类型|说明|
|:---|:---|:---|
|groups|字符串集合|评估范围内组标识符的集合。 当集合为空时，所有组都位于范围内。|
|isEnabled|Boolean| `true` 指示是否应该执行连续访问评估;否则 `false` 。 |
|users|字符串集合|评估范围内用户标识符的集合。 当集合为空时，所有用户都位于范围内。|


## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_continuousaccessevaluationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "users": [ "88139f01-1f8d-4c06-ad74-a2544cee9aee" ],
  "groups": [ "9972fb3f-7a40-49f5-85f6-129d9dfbd47a", "ea178055-4713-4d9a-a06c-ff17466b7e77"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
