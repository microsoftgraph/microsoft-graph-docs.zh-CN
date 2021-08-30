---
author: swapnil1993
title: 列出网站中的 contentTypes
description: 获取网站中的内容类型的集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8ff49f9d4395792e281797440bc6d4fc44570e17
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696525"
---
# <a name="list-contenttypes-in-a-site"></a>列出网站中的 contentTypes
命名空间：microsoft.graph


获取网站 [中的 contentType][contentType] 资源 [的集合][]。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [contentType](../resources/contenttype.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType",
  "isCollection": true
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
