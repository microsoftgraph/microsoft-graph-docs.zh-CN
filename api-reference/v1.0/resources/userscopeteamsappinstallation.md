---
title: userScopeTeamsAppInstallation 资源类型
description: 表示安装在用户个人作用域中的 teamsApp。
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e0ebe4544d419c7cdf4ea72c79b2e76fc231d004
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136255"
---
# <a name="userscopeteamsappinstallation-resource-type"></a>userScopeTeamsAppInstallation 资源类型

命名空间：microsoft.graph

表示[安装在](teamsapp.md)用户的个人作用域中的[teamsApp。](user.md) 作为应用一部分的任何机器人都将成为应用添加到的用户个人作用域的一部分。
此类型继承自 [teamsAppInstallation](teamsappinstallation.md)。

> [!NOTE]
> **teamsAppInstallation** 资源的 `id` 与关联 **teamsApp** 资源的 `id` 具有不同的值。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出为用户安装的应用](../api/userteamwork-list-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合 | 列出在用户的个人范围内安装的应用。 |
|[获取为用户安装的应用](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | 列出在用户的个人范围内安装的指定应用。 |
|[为用户添加应用](../api/userteamwork-post-installedapps.md) | 无 | 添加 (在) 个人范围内安装应用。 |
|[为用户删除应用](../api/userteamwork-delete-installedapps.md) | 无 | 删除 () 用户的个人范围内卸载应用。 |
|[升级为用户安装的应用](../api/userteamwork-teamsappinstallation-upgrade.md) | 无 | 升级到安装在用户个人作用域中的应用的最新版本。|
|[获取用户和应用之间的聊天](../api/userscopeteamsappinstallation-get-chat.md) | [聊天](chat.md) | 列出用户与应用之间的一对一聊天。 |

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 ID (应用Teams ID) 。 |

## <a name="relationships"></a>关系

| 关系   | 类型    | 说明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| 安装的应用。 |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| 此版本的应用的详细信息。 |
|聊天 |[聊天](chat.md) | 用户与应用之间的Teams。 | 

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

