---
title: 添加成员
description: 使用此 API 将成员 (用户或组) 添加到管理单元。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b7db48bdc6b608efa051493cbd27cee25f2d1263
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322782"
---
# <a name="add-a-member"></a>添加成员

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 将成员 (用户或组) 添加到管理单元。

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中, 提供要添加的[用户](../resources/user.md)、[组](../resources/group.md)或[directoryObject](../resources/directoryobject.md)的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
在请求正文中, 提供要添加的[用户](../resources/user.md)或`id` [组](../resources/group.md)对象的 JSON 表示形式。

##### <a name="response"></a>响应
下面是一个响应示例。
 
```http
HTTP/1.1 204 No Content
```
