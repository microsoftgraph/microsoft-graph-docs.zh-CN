---
title: 列出警报
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 6036514c2aeabe287fd019ce69157d4b7897af60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860205"
---
# <a name="list-alerts"></a>列出警报

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检索[通知](../resources/alert.md)对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  SecurityEvents.Read.All SecurityEvents.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | SecurityEvents.Read.All SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下[OData 查询参数](/graph/query-parameters)以帮助自定义响应：

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`将返回从每个安全 API 提供程序的聚合的顶级结果。  

若要返回替代属性集，请使用 OData`$select`查询参数指定的所需的**通知**属性集。  例如，若要返回**assignedTo**、**类别**和**严重性**属性，请添加以下到您的查询： `$select=assignedTo,category,severity`。

> **注意：**`$top`的限制为 1000年警报和组合`$top`  +  `$skip`不能超过 6000 通知。 例如，`/security/alerts?$top=10&$skip=5990`会返回`200 OK`响应代码，但`/security/alerts?$top=10&$skip=5991`将返回`400 Bad Request`响应代码。  有关详细信息，请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。 在请求正文将被忽略。

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和响应正文中的**通知**对象的集合。 如果从提供程序返回状态代码之外的 2xx 或 404 或提供程序超时，如果响应将`206 Partial Content`与警告标头中的提供程序的响应状态代码。 有关详细信息，请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
