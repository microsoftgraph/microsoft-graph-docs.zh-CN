---
author: swapnil1993
title: 更新 columnDefinition
description: 更新网站、列表或内容类型列。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 1c7d7fda5676f88aa0d1c546417f05fe5983c538
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080133"
---
# <a name="update-columndefinition"></a>更新 columnDefinition
命名空间：microsoft.graph


更新 [网站][]、 [列表][]或 [内容类型][contentType] [column][columnDefinition] 。
  

## <a name="permissions"></a>权限  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/columns/{column-id}
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|


## <a name="request-body"></a>请求正文

在请求正文中，提供要更新的 [columnDefinition][] 资源的这些属性的 JSON 表示形式。 为了获得最佳性能，请勿加入尚未更改的现有值。

对于 site **或** list 中的 **列**，可以更新 **columnDefinition** 的任何属性，而不是 **id** 属性。

对于 **contentType 中的列**，只能更新 **必需属性或****隐藏** 属性。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [columnDefinition][] 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
Content-Type: application/json

{
  "required": true,
  "hidden": false,
  "propagateChanges": false     
}
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Custom Column",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Custom Column",
  "readOnly": false,
  "required": true,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
[list]: ../resources/list.md
[site]: ../resources/site.md

