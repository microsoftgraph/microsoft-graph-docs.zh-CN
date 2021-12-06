---
title: 更新警报
description: 更新任何集成 **解决方案** 中的可编辑警报属性，使警报状态和分配在解决方案之间保持同步。 此方法更新具有引用警报 ID 记录的任何解决方案。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: ff8eac9c91bf403a1fb5a55ddfe5f7587b1cc77c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007119"
---
# <a name="update-alert"></a>更新警报

命名空间：microsoft.graph

更新任何集成 **解决方案** 中的可编辑警报属性，使警报状态和分配在解决方案之间保持同步。 此方法更新具有引用警报 ID 记录的任何解决方案。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:------------------------------------|
| 委派（工作或学校帐户）     | SecurityEvents.ReadWrite.All        |
| 委派（个人 Microsoft 帐户） | 不支持。                      |
| 应用程序                            | SecurityEvents.ReadWrite.All        |

## <a name="http-request"></a>HTTP 请求

> **注意：** 必须使用此方法 **将警报** ID 作为参数和 vendorInformation 包含 和 `provider` `vendor` 。

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>请求头

| 名称          | 说明              |
|:--------------|:-------------------------|
| Authorization | Bearer {code}。 必需。 |
| Prefer        | return=representation。 可选。   |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段值的 JSON 表示形式。 正文 **必须** 包含具有 有效 和 字段的 **vendorInformation** `provider` `vendor` 属性。 下表列出了可以针对警报进行更新的字段。 请求正文中不包含的现有属性的值不会更改。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性          | 类型                                                                   | 说明 |
|:------------------|:-----------------------------------------------------------------------|:--|
| assignedTo        | String                                                                 | 分配警报的分析员的姓名，用于会审、调查或修正。 |
| closedDateTime    | DateTimeOffset                                                         | 警报关闭的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| comments          | 字符串集合                                                      | 针对客户警报管理的警报 (分析员) 。 此方法只能使用下列值更新 comments 字段 `Closed in IPC` `Closed in MCAS` ：、。 |
| 反馈          | alertFeedback                                                          | 分析师对警报的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。 |
| status            | alertStatus                                                            | 警报生命周期状态 (阶段) 。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。 |
| tags              | String collection                                                      | 可应用于警报并可以作为筛选条件的用户可定义标签 (例如，"HVA"、"SAW) " |
| vendorInformation | [securityVendorInformation](../resources/securityvendorinformation.md) | 包含有关安全产品/服务供应商、提供程序和子提供程序的详细信息的复杂类型（例如，供应商 = Microsoft；提供程序 = Windows Defender ATP；子提供程序 = AppLocker）。 **提供程序和供应商字段是必需的。** |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

如果使用可选请求标头，则该方法在响应正文中返回 响应 `200 OK` 代码和更新的 [alert](../resources/alert.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-request-without-prefer-header"></a>示例 1：不带 Prefer 标头的请求

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-alert-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>响应

下面是成功响应的示例。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>示例 2：具有 Prefer 标头的请求

#### <a name="request"></a>请求

以下示例显示包含请求标头 `Prefer` 的请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-alert-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面是使用可选请求标头 `Prefer: return=representation` 时的响应示例。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

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
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

