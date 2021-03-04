---
author: swapnil1993
title: site： getApplicableContentTypesForList
description: 获取可添加到列表中的网站内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2cda6c5e62fc85db8d512d814064fd977fa36b9e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446710"
---
# <a name="site-getapplicablecontenttypesforlist"></a>site： getApplicableContentTypesForList
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取[][][可添加到列表中的网站 contentType。][contentType]

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All    |
|委派（个人 Microsoft 帐户） | 不支持    |
|Application | Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/getApplicableContentTypesForList
```
## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

若要仅列出自定义内容类型，请使用 `$filter=isBuiltin eq false` 。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="function-parameters"></a>函数参数
在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|参数|类型|说明|
|-|-|-|-|
|listId| String | 需要获取适用内容类型的列表的 GUID。 必需。 |

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回响应 `200 OK` 代码和 [contentType](../resources/contenttype.md) 集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "site_getapplicablecontenttypesforlist"
}
-->
```http
GET https://graph.microsoft.com/beta/sites/{siteId}/getApplicableContentTypesForList(listId='listId')
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contentType)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```

[contentType]: ../resources/contentType.md
[网站]: ../resources/site.md
