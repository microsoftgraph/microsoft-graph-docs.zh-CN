---
title: 列出警报
description: 检索警报对象的列表。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: d50c3244ae2c0e9f158dc38923136ef3e8656f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459211"
---
# <a name="list-alerts"></a>列出警报

检索[警报](../resources/alert.md)对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  securityevents.readwrite.all、securityevents.readwrite.all 和所有  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | securityevents.readwrite.all、securityevents.readwrite.all 和所有 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>可选查询参数

此方法支持以下[OData 查询参数](/graph/query-parameters)来帮助自定义响应:

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`将返回每个安全 API 提供程序的聚合顶级结果。  

若要返回其他属性集, 请使用 OData `$select`查询参数指定所需的一组**警报**属性。  例如, 若要返回 "**分配给**"、"**类别**" 和 "**严重性**" 属性, 请将`$select=assignedTo,category,severity`以下内容添加到您的查询中:。

> **注意:**`$top`的警报限制为1000个, 并且组合`$top`  +  `$skip`不能超过6000个警报。 例如, `/security/alerts?$top=10&$skip=5990`将返回`200 OK`响应代码, 但`/security/alerts?$top=10&$skip=5991`将返回`400 Bad Request`响应代码。  有关详细信息, 请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。

## <a name="request-headers"></a>请求头

| 名称      |说明|
|:----------|:----------|
| Authorization  | 持有者 {代码}。 必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。 请求正文将被忽略。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和**alert**对象集合。 如果从提供程序返回的状态代码或者提供程序超时, 则响应将是一个`206 Partial Content`状态代码, 提供程序的响应在警告标头中。 有关详细信息, 请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
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
