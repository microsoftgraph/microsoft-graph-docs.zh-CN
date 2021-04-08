---
author: swapnil1993
ms.date: 08/30/2020
title: 在网站创建 columnDefinition
description: 创建网站栏。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 1404707dc2a98b4ac60e663fd25d595c977148f7
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638836"
---
# <a name="create-columndefinition-for-a-site"></a>为网站创建 columnDefinition
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
为网站创建 [列][site] by specifying a [columnDefinition][columnDefinition] 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/concepts/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/columns
```

## <a name="request-body"></a>请求正文

在请求正文中，提供要添加的 [columnDefinition 资源的][] JSON 表示形式。  

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [columnDefinition][] 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/columns
Content-Type: application/json

{
   "description":"test",
   "enforceUniqueValues":false,
   "hidden":false,
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "description":"test",
   "displayName":"Title",
   "enforceUniqueValues":false,
   "hidden":false,
   "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
  

