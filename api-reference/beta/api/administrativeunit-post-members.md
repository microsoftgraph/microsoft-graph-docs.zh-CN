---
title: 添加成员
description: 使用此 API 成员 （用户或组） 添加到一个管理单元。
author: lleonard-msft
ms.openlocfilehash: be47dbf06c5f59c0a4aaaea4f8c8b4aa8c3ce902
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339226"
---
# <a name="add-a-member"></a>添加成员

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

使用此 API 成员 （用户或组） 添加到一个管理单元。

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
| Name      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[用户](../resources/user.md)、[组](../resources/group.md)或[directoryObject](../resources/directoryobject.md)要添加的 JSON 表示形式。

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
在请求正文中，提供的 JSON 表示形式`id`您想要添加的[用户](../resources/user.md)或[组](../resources/group.md)对象。

##### <a name="response"></a>响应
下面是一个响应示例。
 
```http
HTTP/1.1 204 No Content
```
