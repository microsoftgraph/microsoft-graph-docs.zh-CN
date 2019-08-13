---
title: 更新警报
description: 在任何集成的解决方案中更新可编辑的 alert 属性, 以保持各个解决方案之间同步警报状态和分配。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 93a395f78baeec0a6609ea7dee0b9cfbc3e3224b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318815"
---
# <a name="update-alert"></a>更新警报

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在任何集成的解决方案中更新可编辑的**alert**属性, 以保持各个解决方案之间同步警报状态和分配。 此方法更新任何包含所引用警报 ID 的记录的解决方案。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |   SecurityEvents.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

> **注意:** 您必须将**警报**ID 作为参数和 vendorInformation (包含`provider`和`vendor`使用此方法) 包括在内。
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}。 必需。|
|Prefer | return = 表示形式 |

## <a name="request-body"></a>请求正文

在请求正文中, 提供应更新的相关字段的值的 JSON 表示形式。 正文**必须**包含具有有效`vendorInformation` `provider`和`vendor`字段的属性。 下表列出了可以为警报更新的字段。 未包含在请求正文中的现有属性的值不会更改。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|assignedTo|String|为会审、调查或修正分配了警报的分析师的名称。|
|closedDateTime|DateTimeOffset|警报关闭的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|comments|字符串集合|通知的分析师注释 (针对客户通知管理)。|
|反馈|alertFeedback 枚举|分析师对警报的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。|
|status|alertStatus 枚举|警报生命周期状态 (阶段)。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。|
|tags|String collection|可应用于警报并可用作筛选条件的用户定义的标签 (例如, "HVA"、"锯")。|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|包含有关安全产品/服务供应商、提供程序和子提供程序的详细信息的复杂类型（例如，供应商 = Microsoft；提供程序 = Windows Defender ATP；子提供程序 = AppLocker）。 **提供程序和供应商字段是必需的。**|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

如果使用可选的请求标头, 则该方法将`200 OK`在响应正文中返回响应代码和更新的[alert](../resources/alert.md)对象。

## <a name="examples"></a>示例

### <a name="example-1-request-without-prefer-header"></a>示例 1: 不带首选标头的请求

#### <a name="request"></a>请求

以下是不带`Prefer`标头的请求示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>响应

下面是成功响应的示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>示例 2: 具有首选标头的请求

#### <a name="request"></a>请求

下面的示例演示包含`Prefer`请求标头的请求。

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

#### <a name="response"></a>响应

以下是使用可选`Prefer: return=representation`请求标头时响应的示例。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
