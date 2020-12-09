---
title: teamsAppInstallation 资源类型
description: '安装在团队中的 teamsApp、聊天或用户的个人作用域。 '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9b34450f29ccb1fb02cf1751c78f312c71fdefc9
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606951"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

安装在[团队](team.md)中的[teamsApp](teamsapp.md) 、[聊天](chat.md)或[用户](user.md)的个人作用域。 作为应用程序一部分的任何 bot 都将成为向其添加应用程序的任何团队、聊天或用户个人范围的一部分。

> [!NOTE]
> `id` **TeamsAppInstallation** 资源的值与 `id` 关联的 **teamsApp** 资源的值不同。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[列出团队中安装的应用程序](../api/team-list-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) 集合 | 列出团队中安装的应用程序。|
|[获取团队中安装的应用程序](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 获取团队中安装的指定应用程序。|
|[将应用添加到团队](../api/team-post-installedapps.md) |无 | 向团队添加 (安装) 应用程序。|
|[从团队中删除应用](../api/team-delete-installedapps.md) | 无 | 删除 (从团队中的应用) 卸载。|
|[升级在团队中安装的应用程序](../api/team-teamsappinstallation-upgrade.md) | 无 | 将团队中安装的应用程序升级到最新版本。|
|[列出为用户安装的应用](../api/userteamwork-list-installedapps.md) | [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合 | 列出在用户的个人范围内安装的应用程序。|
|[获取已安装的用户应用程序](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | 获取在用户的个人范围内安装的指定应用程序。 |
|[为用户添加应用程序](../api/userteamwork-post-installedapps.md) | | 添加 (安装) 用户的个人作用域中的应用程序。|
|[删除用户的应用程序](../api/userteamwork-delete-installedapps.md) | 无 | 删除 (卸载) 用户的个人作用域中的应用程序。|
|[升级为用户安装的应用](../api/userteamwork-teamsappinstallation-upgrade.md) | 无 | 将用户的个人范围内安装的应用程序升级到最新版本。|
|[列出聊天中的应用程序](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) 集合 | 列出聊天中安装的应用程序。|
|[获取聊天中的应用程序](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 获取聊天中安装的指定应用程序。|
|[在聊天中添加应用程序](../api/chat-post-installedapps.md) | | 将 (安装) 应用程序添加到聊天。|
|[从聊天中删除应用程序](../api/chat-delete-installedapps.md) | 无 | 从聊天中删除 (卸载) 应用程序。|
|[升级聊天中的应用程序](../api/chat-teamsappinstallation-upgrade.md) | 无 | 将聊天中安装的应用程序升级到最新版本。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 ID (团队的 ap ID) 。 |

## <a name="relationships"></a>关系

| 关系   | 类型    | Description |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| 已安装的应用程序。 |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| 此版本的应用程序的详细信息。 |

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


