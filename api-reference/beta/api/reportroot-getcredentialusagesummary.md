---
title: reportRoot： getCredentialUsageSummary
description: 报告组织中使用自助密码重置功能的用户数量的当前状态。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5a059ed68c90a071d0027c059eb2470791be8cca
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65102946"
---
# <a name="reportroot-getcredentialusagesummary"></a>reportRoot： getCredentialUsageSummary

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

报告组织中使用自助密码重置功能的用户数量的当前状态。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Reports.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用                            | Reports.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary(period='{periodValue}')
```

## <a name="function-parameters"></a>函数参数

必须使用以下函数参数来请求响应的时间范围。

| 参数 | 类型 | 说明 |
|:--------- |:---- |:----------- |
| period | 字符串 | 必需。 指定需要使用情况数据的天数。 例如：`/reports/getCredentialUsageSummary(period='D30')`。 支持的句点： `D1`和 `D7``D30`. 句点不区分大小写。 |

## <a name="optional-query-parameters"></a>可选的查询参数

此函数支持可选的 OData 查询参数 **$filter**。 可以对 [credentialUsageSummary](../resources/credentialusagesummary.md) 资源的以下一个或多个属性应用 **$filter**。

| 属性 | 说明和示例 |
|:---- |:----------- |
| 特征 | 指定要 (注册与重置) 的使用情况数据的类型。 例如：`/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`。 支持的筛选器运算符： `eq`. |

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |
| Content-Type | application/json |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和新的 [credentialUsageSummary](../resources/credentialusagesummary.md) 集合对象。

## <a name="examples"></a>示例

以下示例演示如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialusagesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialusagesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialusagesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialusagesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都是从实际调用返回的。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


