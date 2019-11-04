---
title: 列出 accessPackageResources
description: 检索 accesspackageresource 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebb1d6ce33c2f10da19162d40f097c1043af62e8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935278"
---
# <a name="list-accesspackageresources"></a>列出 accessPackageResources

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[accessPackageCatalog](../resources/accesspackagecatalog.md)中的[accessPackageResource](../resources/accesspackageresource.md)对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     |  EntitlementManagement |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。 必填。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageResource](../resources/accesspackageresource.md)对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
