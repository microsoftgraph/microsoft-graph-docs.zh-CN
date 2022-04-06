---
author: JeremyKelley
title: 将项目添加到捆绑包
description: 将项目添加到 driveItems 捆绑包
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ed5ded16b1577a4931b28d24ac22a785eaed2d2a
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561581"
---
# <a name="add-item-to-a-bundle"></a>将项目添加到捆绑包

命名空间：microsoft.graph

将驱动器中的其他 [driveItem][] 添加到 [捆绑包][]。

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。                             |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All   |
|应用程序          | 不支持。                                           |

## <a name="http-request"></a>HTTP 请求

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明  |
|:------------- |:------------ |
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文

请求正文包括应添加到捆绑包的子集合中的项目的标识符。

## <a name="response"></a>响应

如果成功，响应为 `204 No Content`。

有关错误响应的信息，请参阅 [错误响应][error-response]。

## <a name="example"></a>示例

### <a name="request"></a>请求

此请求将现有项添加到指定的捆绑包。

<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```

### <a name="response"></a>响应

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section&quot;: &quot;documentation"
} -->


