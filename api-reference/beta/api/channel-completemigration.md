---
title: channel： completeMigration
description: 通过从频道中删除迁移模式完成外部邮件的迁移。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 144ec67ef6e21e11716bec0e61f53c5e079d96cf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200964"
---
# <a name="channel-completemigration"></a>channel： completeMigration

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过从团队中的频道删除来完成 `migration mode` 邮件迁移过程[](../resources/channel.md)。 `Migration mode` 是一种在数据迁移过程中阻止某些操作（如发送邮件和添加成员）的特殊状态。

完成 **Migration 请求后** ，无法将其他消息导入团队。 在请求返回成功响应后，你可以向团队添加成员。

## <a name="permissions"></a>权限

调用此 API 需要以下权限。 若要了解更多信息，*请参阅*[权限](/graph/permissions-reference)。

|权限类型      | 权限  |
|:--------------------|:---------------------------------------------------------|
| 委派（工作或学校帐户）  | 不支持。|
| 委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Teamwork.Migrate.All|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/completeMigration
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/completeMigration
```

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a>响应

下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 5793eec6-0e5a-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
