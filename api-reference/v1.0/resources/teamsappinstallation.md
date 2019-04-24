---
title: teamsAppInstallation 资源类型
description: '在团队中安装的 teamsApp。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c98f1b927c319eb1d81573fd9dc43e1baad86a39
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462352"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[团队](team.md)中安装的[teamsApp](teamsapp.md) 。 作为应用程序的一部分的任何 bot 都将成为向其添加应用程序的任何团队的一部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出应用程序](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsapp.md) | 列出在团队中安装的应用程序。|
|[添加应用程序](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsapp.md) | 将应用添加（安装）到团队。|
|[删除应用程序](../api/teamsappinstallation-delete.md) | 无 | 从团队中删除 (卸载) 应用程序。|
|[升级应用程序](../api/teamsappinstallation-upgrade.md) | 无 | 升级到最新版本的应用程序。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 id (而不是团队 appid)。 |

## <a name="relationships"></a>关系

| 关系   | 类型    | 说明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| 已安装的应用程序。 |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| 此版本的应用程序的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a>另请参阅

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

