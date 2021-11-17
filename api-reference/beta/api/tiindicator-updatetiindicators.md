---
title: tiIndicator：updateTiIndicators
description: 在一个请求 (TI) 指示器（而不是多个请求）中更新多个威胁情报。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: e90fd3b95e302956a250f2acf08ff18daa0298ca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989434"
---
# <a name="tiindicator-updatetiindicators"></a>tiIndicator：updateTiIndicators

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在一个请求 (TI) 指示器（而不是多个请求）中更新多个威胁情报。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型   | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | ThreatIndicators.ReadWrite.OwnedBy |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。 有关可更新的属性的详细信息，请参阅[更新 tiIndicator。](tiindicator-update.md) 每个 tiIndicator 的必填字段为 `id` `expirationDateTime` `targetProduct` ：、、。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|值|tiIndicator 集合| 要 **更新的 tiIndicator** 集合。 每个实体必须具有 **id** 和其他可编辑属性以进行更新。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tiIndicator](../resources/tiindicator.md) 对象集合。  如果出现错误，此方法将返回 响应 `206 Partial Content` 代码。  有关详细信息 [，](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) 请参阅错误。

## <a name="examples"></a>示例

以下示例演示如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators",
  "isCollection":true
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
  ]
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-updatetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/tiindicator-updatetiindicators-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> [!NOTE]
> 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


