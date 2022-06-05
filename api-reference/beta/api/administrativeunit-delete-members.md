---
title: 删除成员
description: 使用此 API 从管理单元中删除成员 (用户、组或设备) 。
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 199e0ba76a61b8279dcd79acb59ef14d9001a35d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898166"
---
# <a name="remove-a-member"></a>删除成员

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 从管理单元中删除成员 (用户、组或设备) 。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | AdministrativeUnit.ReadWrite.All |

若要从管理单元中删除成员，必须为调用主体分配以下 [Azure AD 角色](/azure/active-directory/roles/permissions-reference)之一：

* 特权角色管理员
* 全局管理员

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。 在下面的示例中， `{id1}` 表示目标管理单元的标识符，并 `{id2}` 表示要从目标管理单元中删除的成员用户、组或设备的唯一标识符。 

```msgraph-interactive
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

### <a name="response"></a>响应
下面展示了示例响应。
 
```http
HTTP/1.1 204 No Content
```


