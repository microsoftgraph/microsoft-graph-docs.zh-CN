---
title: 更新警报
description: 更新在任何集成的解决方案，以使警报状态和分配保持同步跨解决方案可编辑的警报属性。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b1fec6bfca2ce116bc35c4a7c8a115418b15012
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967324"
---
# <a name="update-alert"></a>更新警报

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新在任何集成的解决方案，以使警报状态和分配保持同步跨解决方案的可编辑**通知**属性。 此方法将更新的任何解决方案都有一个记录引用的警报 id。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |   SecurityEvents.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

> **注意：** 您必须为参数和 vendorInformation 包含包括的**警报**ID`provider`和`vendor`使用此方法。
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>请求标头

| Name       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}。必需。|
|Prefer | 返回 = 表示形式 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。 **必须**正文包含`vendorInformation`属性与有效`provider`和`vendor`字段。 下表列出了可更新的通知的字段。 不包含在请求正文中的现有属性的值不会更改。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|assignedTo|String|分析师通知的名称分配给进行会审、 调查或修复。|
|closedDateTime|DateTimeOffset|通知关闭的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|comments|String 集合|分析师评论的警报 （客户警报管理）。|
|反馈|alertFeedback 枚举|分析师通知上的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。|
|status|alertStatus 枚举|警报生命周期状态 （阶段）。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。|
|tags|String 集合|可以应用于通知和可以充当筛选条件 (例如，"HVA"，"看到) 的用户可定义标签。|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|包含有关安全产品/服务供应商、 提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。 **提供程序和供应商字段是必需的。**|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

如果使用可选请求标头，则该方法返回`200 OK`响应代码和响应正文中的更新的[通知](../resources/alert.md)对象。

## <a name="examples"></a>示例

### <a name="example-1-request-without-prefer-header"></a>示例 1： 请求，但没有更愿意头

#### <a name="request"></a>请求

以下是没有的请求的示例`Prefer`标头。
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

### <a name="example-2-request-with-prefer-header"></a>示例 2： 使用更愿意标头的请求

#### <a name="request"></a>请求

下面的示例演示包含的请求，`Prefer`请求标头。

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

下面是响应的示例时可选`Prefer: return=representation`使用请求标头。

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
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
