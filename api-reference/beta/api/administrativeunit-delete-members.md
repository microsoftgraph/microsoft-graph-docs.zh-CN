---
title: 删除成员
description: 使用此 API 可从管理单元中删除成员（用户或组）。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3774df54f73c7e08456b3412a65378cfb51cefcf
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123340"
---
# <a name="remove-a-member"></a>删除成员

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 可从管理单元中删除成员（用户或组）。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit、Directory.accessasuser.all 和所有    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | AdministrativeUnit.ReadWrite.All |

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
##### <a name="request"></a>请求
下面是一个请求示例。 在下面的示例中，id1 表示目标管理单元的标识符，id2 表示要从目标管理单元中删除的成员用户或组的唯一标识符。 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a>响应
下面是一个响应示例。
 
```http
HTTP/1.1 204 No Content
```
