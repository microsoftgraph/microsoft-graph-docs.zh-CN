---
title: 通道： completeMigration
description: 通过从通道中删除迁移模式来完成外部邮件的迁移。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35991987816f65b7a52a80857b00621572fbb793
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796547"
---
# <a name="channel-completemigration"></a>通道： completeMigration

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 `migration mode` 从团队中的 [通道](../resources/channel.md) 中删除来完成邮件迁移过程。 `Migration mode` 是一种特殊状态，可防止在数据迁移过程中执行某些操作（如发送邮件和添加成员）。

发出 **completeMigration** 请求后，不能将其他邮件导入到团队中。 在请求返回成功的响应之后，您可以向团队添加成员。

## <a name="permissions"></a>权限

若要调用此 API，需要以下权限。 若要了解详细信息， *请参阅*[权限](/graph/permissions-reference)。

|权限类型      | 权限  |
|:--------------------|:---------------------------------------------------------|
| 委派（工作或学校帐户）  | 不支持。|
| 委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Teamwork.Migrate.All|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/channels/{channelId}/completeMigration
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
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/completeMigration
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
