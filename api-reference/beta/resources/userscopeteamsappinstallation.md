---
title: userScopeTeamsAppInstallation 资源类型
description: 代表在用户的个人作用域中安装的 teamsApp。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 19ca16e4d6a3171cc622440ee79dce3d93e8dd84
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564194"
---
# <a name="userscopeteamsappinstallation-resource-type"></a>userScopeTeamsAppInstallation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表在[用户](user.md)的个人作用域中安装的[teamsApp](teamsapp.md) 。 作为应用程序一部分的任何 bot 都将成为应用程序添加到的用户个人范围的一部分。
此类型继承自 [teamsAppInstallation](teamsappinstallation.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出为用户安装的应用](../api/userteamwork-list-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合 | 列出在用户的个人范围内安装的应用程序。 |
|[获取已安装的用户应用程序](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | 列出在用户的个人范围内安装的指定应用程序。 |
|[为用户添加应用程序](../api/userteamwork-add-installedapps.md) | 无 | 添加 (安装) 用户的个人作用域中的应用程序。 |
|[删除用户的应用程序](../api/userteamwork-delete-installedapps.md) | 无 | 删除) 用户的个人作用域中的应用程序 (卸载。 |
|[升级为用户安装的应用](../api/userteamwork-upgrade-installedapps.md) | 无 | 升级到在用户的个人范围内安装的最新版本的应用程序。|
|[在用户和应用之间获取聊天](../api/userscopeteamsappinstallation-get-chat.md) | [聊天](chat.md) | 列出用户与应用之间的一对一聊天。 |

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 ID (团队应用程序 ID) 。 |

## <a name="relationships"></a>关系

| 关系   | 类型    | 说明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| 已安装的应用程序。 |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| 此版本的应用程序的详细信息。 |
|聊天 |[聊天](chat.md) | 用户和团队应用程序之间的聊天。 | 

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userScopeTeamsAppInstallation",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userScopeTeamsAppInstallation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

