---
title: 获取成员
description: 使用此 API 可在管理单元中) 用户或组 (获取特定成员。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6cf700fad752071603586d29cc892a28763616a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020236"
---
# <a name="get-a-member"></a>获取成员

命名空间：microsoft.graph

使用此 API 可在管理单元中) 用户或组 (获取特定成员。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、all、、all、all 和的所有子目录。    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AdministrativeUnit、AdministrativeUnit、all、all、all、All 和所有的 |

## <a name="http-request"></a>HTTP 请求

```http
GET /directory/administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [user](../resources/user.md) 或 [group](../resources/group.md) 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

```http
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a>响应
下面是 respone 的一个示例。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```
