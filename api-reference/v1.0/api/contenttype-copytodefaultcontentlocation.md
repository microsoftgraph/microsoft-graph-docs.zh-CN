---
author: swapnil1993
title: contentType：copyToDefaultContentLocation
description: 将文件复制到内容类型中的默认内容位置。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 4ca64f9a29b1471815784d10d0e23ec14c6a08fd
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696477"
---
# <a name="contenttype-copytodefaultcontentlocation"></a>contentType：copyToDefaultContentLocation
命名空间：microsoft.graph


将文件复制到内容类型中的默认 [内容位置][contentType]。 然后，可以通过 POST 操作将该文件添加为默认文件或模板。

## <a name="permissions"></a>权限  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。


|参数|类型|说明|
|-|-|-|
|sourceFile| [itemReference](../resources/itemreference.md) |有关需要复制到默认内容位置的源文件的元数据。 此为必需属性。|
|destinationFileName| string |目标文件名。 |

## <a name="response"></a>响应


如果成功，此调用将返回 `204 No Content` 响应。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "contenttype_copytodefaultcontentlocation"
}
-->
```http
POST https://graph.microsoft.com/v1.0/sites/{siteId}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
   "sourceFile":{
      "sharepointIds":{
         "listId":"e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
         "listItemId":"2"
      }
   },
   "destinationFileName":"newname.txt"
}
```

### <a name="response"></a>响应


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
