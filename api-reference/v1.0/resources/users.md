---
title: 在 Microsoft Graph 中与用户一起工作
description: 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。
localization_priority: Priority
author: krbain
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 74f479ea8d713912fb875a33ac4decca47ce6c61
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353754"
---
# <a name="working-with-users-in-microsoft-graph"></a>在 Microsoft Graph 中与用户一起工作

可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。

通过 Microsoft Graph，你能以两种方式访问 [用户](user.md)

- 通过用户 ID，`/users/{id | userPrincipalName}`
- 通过使用已登录的用户的 `/me` 别名，这与 `/users/{signed-in user's id}` 相同

## <a name="authorization"></a>授权

One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>通用属性

以下内容表示获取或列出用户时返回的属性的默认集。 这些是所有可用属性的子集。 要获取更多用户属性，请使用 `$select` 查询参数。

|属性 |说明 |
|:----------|:-------------|
|id | 用户的唯一标识符。|
|businessPhones | 用户的电话号码。|
|displayName | 用户通讯簿中显示的名称。|
|givenName| 用户的名 |
|jobTitle | 用户的职务。|
|mail| 用户的电子邮件地址。 |
|mobilePhone | 用户的手机号码。|
|officeLocation | 用户的办公地址。|
|preferredLanguage | 用户的语言首选项。|
|surname| 用户的姓。 |
|userPrincipalName| 用户主体名称。 |

有关详细信息及所有属性的列表，请参阅 [user](user.md) 对象。

## <a name="common-operations"></a>通用操作

> **注意：** 某些操作需要其他权限。

| 路径    | 说明 |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | 列出组织中的用户。 |
|[`/users/{id}`](../api/user-get.md) | 通过 ID 获取特定用户。 |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| 获取用户个人资料照片。 |
|[`/users/{id}/manager`](../api/user-list-manager.md) | 获取用户的经理。 |
|[`/users/{id}/messages`](../api/user-list-messages.md)| 列出用户主收件箱中的电子邮件。 |
|[`/users/{id}/events`](../api/user-list-events.md) | 列出用户日历中即将发生的事件。 |
|[`/users/{id}/drive`](../api/drive-get.md)| 获取用户 OneDrive 文件存储。 |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| 列出用户是其成员的所有组。 |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。