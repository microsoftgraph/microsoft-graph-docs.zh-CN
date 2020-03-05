---
title: teamsAppInstallation 资源类型
description: '安装在团队中的 teamsApp、聊天或用户的个人作用域。 '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10a7d5d58a18e23c47d603e7b05c9981ddfeed76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519909"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

安装在[团队](team.md)中的[teamsApp](teamsapp.md) 、[聊天](chat.md)或[用户](user.md)的个人作用域。 作为应用程序一部分的任何 bot 都将成为向其添加应用程序的任何团队、聊天或用户个人范围的一部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出团队中安装的应用程序](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsappinstallation.md) 集合 | 列出在团队中安装的应用程序。|
|[将应用添加到团队](../api/teamsappinstallation-add.md) |无 | 将应用添加（安装）到团队。|
|[从团队中删除应用](../api/teamsappinstallation-delete.md) | 无 | 从团队中删除（卸载）应用程序。|
|[升级在团队中安装的应用程序](../api/teamsappinstallation-upgrade.md) | 无 | 升级到团队中安装的应用程序的最新版本。|
|[列出为用户安装的应用](../api/user-list-teamsappinstallation.md) | [teamsAppInstallation](teamsappinstallation.md) 集合 | 列出在用户的个人范围内安装的应用程序。|
|[为用户添加应用程序](../api/user-add-teamsappinstallation.md) | | 在用户的个人作用域中添加（安装）应用程序。|
|[删除用户的应用程序](../api/user-delete-teamsappinstallation.md) | 无 | 删除（卸载）用户个人作用域中的应用程序。|
|[升级为用户安装的应用](../api/user-upgrade-teamsappinstallation.md) | 无 | 升级到在用户的个人范围内安装的最新版本的应用程序。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一的 ID （而不是团队的 ap ID）。 |

## <a name="relationships"></a>关系

| 关系   | 类型    | 说明 |
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
