---
author: swapnil1993
title: 列出 columnDefinitions
description: 列出内容类型的列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5d3c1c4e64323aa772639d977d0d4dfc18603932
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446121"
---
# <a name="list-columndefinitions"></a>列出 columnDefinitions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
获取内容  [类型中的][columnDefinition] [集合][contentType]。

  

## <a name="permissions"></a>Permissions

  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application | Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All  |

  

## <a name="http-request"></a>HTTP 请求

  
<!-- {
  "blockType": "ignored"
}
-->
```http

GET /sites/{site-id}/contentTypes/{contentType-id}/columns
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
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

如果成功，此方法在响应正文中返回响应代码和 `200 OK` [columnDefinition][] 对象集合。

  

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "get_columns_from_contenttype" } -->
 

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.columnDefinition)"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "",
      "displayName": "Title",
      "hidden": false,
      "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
      "indexed": false,
      "name": "Title",
      "readOnly": false,
      "required": false,
      "text": {
        "allowMultipleLines": false,
        "appendChangesToExistingText": false,
        "linesForEditing": 0,
        "maxLength": 255
      }
    },
    {
      "description": "",
      "displayName": "Address",
      "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
      "indexed": false,
      "name": "Address",
      "readOnly": false,
      "required": false,
      "text": {
        "allowMultipleLines": false,
        "appendChangesToExistingText": false,
        "linesForEditing": 0,
        "maxLength": 255
      }
    }
  ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
 
