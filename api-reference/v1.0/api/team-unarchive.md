---
title: 解档团队
description: 还原存档的团队。 这将恢复用户发送邮件和编辑团队的能力，abiding 受租户和团队设置的支持。 使用存档 API 存档团队。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b891f361acd79a4697b15d54a6f82516124a951c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290572"
---
# <a name="unarchive-team"></a>解档团队

命名空间：microsoft.graph



还原存档的[团队](../resources/team.md)。 这将恢复用户发送邮件和编辑团队的能力，abiding 受租户和团队设置的支持。 使用[存档](team-archive.md)API 存档团队。

Unarchiving 是一种异步操作。 异步操作成功完成后，团队即为 unarchived，这可能会在此 API 的响应之后发生。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | TeamSettings、Group 写全部、所有的 ReadWrite。 All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamSettings （[RSC](https://aka.ms/teams-rsc)）、TeamSettings、All、group、All、All 和 All。 all |

> **注意**：此 API 支持管理员权限。 全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果 unarchiving 成功启动，此方法将返回 `202 Accepted` 响应代码。 该响应还将包含一个 `Location` 标头，其中包含为处理团队的 unarchiving 而创建的[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。 通过向此位置发出 GET 请求，检查 unarchiving 操作的状态。

## <a name="example"></a>示例
#### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```

#### <a name="response"></a>响应
响应示例如下所示。
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
