---
title: 在 Microsoft Graph 中与用户一起工作
description: 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。
ms.localizationpriority: high
author: jpettere
ms.prod: users
doc_type: conceptualPageType
ms.openlocfilehash: 2f36771ccc92bfec6fd4aeb723891a3a712c6269
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65059969"
---
# <a name="working-with-users-in-microsoft-graph"></a>在 Microsoft Graph 中与用户一起工作

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以使用 Microsoft Graph 基于用户、他们与其他用户和组的关系以及他们访问的资源（例如其邮件、日历、文件、管理角色、组成员身份）构建引人注目的应用体验。

通过 Microsoft Graph，你能以两种方式访问用户：

- 通过用户 ID，`/users/{id}`
- 通过使用已登录的用户的 `/me` 别名，这与 `/users/{signed-in user's id}` 相同

Azure AD 中有两种类型的用户 - 成员用户和来宾用户。 来宾用户通过兑换其邀请加入组织。 来宾用户可以转换为成员，享受成员的所有特权。

## <a name="authorization"></a>授权

需要以下 [权限](/graph/permissions-reference) 之一才能访问用户操作。用户可将前三个权限授予应用程序。其余权限只能由管理员授予应用。

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- User.ManageIdentities.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>组织中来宾用户的用户和组搜索限制

用户和组搜索功能允许应用对 `/users` 或 `/groups` 资源集(例如 `https://graph.microsoft.com/v1.0/users`)执行查询，以搜索组织目录中的任何用户或组。管理员和成员用户都具有此功能；但来宾用户没有。

如果登录用户是来宾用户，应用程序可以读取特定用户或组的配置文件（例如，`https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`），具体视应用程序获得的授权而定；不过，不能对可能返回多个资源的 `/users` 或 `/groups` 资源集执行查询。

借助授予的适当权限，应用程序可以读取用户或组的配置文件，具体是通过导航属性中的链接获取；例如，`/users/{id}/directReports` 或 `/groups/{id}/members`。

有关来宾用户搜索限制的详细信息，请参阅[比较成员用户和来宾用户的默认权限](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions)。

## <a name="common-properties"></a>通用属性

| 属性 | 说明 |
|----------|-------------|
| displayName | 用户通讯簿中显示的名称。|
|givenName| 用户的名。 |
|surname| 用户的姓。 |
|mail| 用户的电子邮件地址。 |
|photo| 用户的个人资料照片。 |

有关详细信息及所有属性的列表，请参阅 [user](user.md) 对象。

## <a name="common-operations"></a>通用操作

>**注意：** 某些操作需要其他权限。

| 路径    | 说明 |
|---------|-------------|
|[`/users`](../api/user-list.md) | 列出组织中的用户。 |
|[`/users/{id}`](../api/user-get.md) | 通过 ID 获取特定用户。 |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| 获取用户个人资料照片。 |
|[`/users/{id}/manager`](../api/user-list-manager.md) | 获取用户的经理。 |
|[`/users/{id}/messages`](../api/user-list-messages.md)| 列出用户主收件箱中的电子邮件。 |
|[`/users/{id}/events`](../api/user-list-events.md) | 列出用户日历中即将发生的事件。 |
|[`/users/{id}/drive`](../api/drive-get.md)| 获取用户 OneDrive 文件存储。 |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| 列出用户是其成员的所有组。 |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| 列出用户所属的 Microsoft Teams。 |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。