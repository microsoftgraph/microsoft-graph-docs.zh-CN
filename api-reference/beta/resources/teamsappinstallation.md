---
title: teamsAppInstallation 资源类型
description: '安装在团队、聊天或用户个人作用域中的 teamsApp。 '
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 66cf31f21a105934181aee5e506cc2215f9ce7a9
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663904"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsApp](teamsapp.md)安装在团队[、](team.md)[聊天](chat.md)或用户的个人[作用域中](user.md)。 作为应用一部分的任何机器人都将成为应用添加到的任何团队、聊天或用户个人范围的一部分。

> [!NOTE]
> **teamsAppInstallation** 资源的 `id` 与关联 **teamsApp** 资源的 `id` 具有不同的值。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出在团队中安装的应用](../api/team-list-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) 集合 | 列出在团队中安装的应用。|
|[在团队中安装应用](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 获取在团队中安装的指定应用。|
|[将应用添加到团队](../api/team-post-installedapps.md) |无 | 添加 (将) 安装到团队。|
|[升级团队中安装的应用](../api/team-teamsappinstallation-upgrade.md) | 无 | 将团队中安装的应用升级到最新版本。|
|[从团队中删除应用](../api/team-delete-installedapps.md) | 无 | 从 (中删除) 卸载应用。|
|[列出为用户安装的应用](../api/userteamwork-list-installedapps.md) | [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合 | 列出在用户的个人范围内安装的应用。|
|[为用户安装应用](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | 获取在用户的个人范围内安装的指定应用。 |
|[为用户添加应用](../api/userteamwork-post-installedapps.md) | | 添加 (在) 范围内安装应用。|
|[升级为用户安装的应用](../api/userteamwork-teamsappinstallation-upgrade.md) | 无 | 将用户个人范围内安装的应用升级到最新版本。|
|[为用户删除应用](../api/userteamwork-delete-installedapps.md) | 无 | 删除 (用户) 范围内应用的卸载权限。|
|[列出聊天中的应用](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) 集合 | 列出聊天中安装的应用。|
|[在聊天中安装应用](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 获取在聊天中安装的指定应用。|
|[在聊天中添加应用](../api/chat-post-installedapps.md) | | 添加 (将) 安装到聊天中。|
|[升级聊天中的应用](../api/chat-teamsappinstallation-upgrade.md) | 无 | 将聊天中安装的应用升级到最新版本。|
|[从聊天中删除应用](../api/chat-delete-installedapps.md) | 无 | 从 (卸载) 应用。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 ID (不是团队的 ap ID) 。 |

## <a name="relationships"></a>关系

| 关系   | 类型    | 说明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| 安装的应用。 |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| 此版本的应用的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a>另请参阅

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)
- [userScopeTeamsAppInstallation](../resources/userscopeteamsappinstallation.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


