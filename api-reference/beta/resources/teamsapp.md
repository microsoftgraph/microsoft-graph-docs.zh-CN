---
title: teamsApp 资源类型
description: 应用程序中的 Microsoft 团队应用程序目录。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b02af5148e40cddd6079de3479767110a9877e4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841571"
---
# <a name="teamsapp-resource-type"></a>teamsApp 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

应用程序中[的 Microsoft 团队](teams-api-overview.md)应用程序目录。

用户可以看到这些应用程序中 Microsoft 团队存储，并且可以将这些应用程序安装中[团队](team.md)使用[添加到团队的应用程序](../api/teamsappinstallation-add.md)方法。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出已发布的应用程序](../api/teamsapp-list.md) | [teamsApp](teamsapp.md)集合 | 列出来自 Microsoft 团队的应用程序目录的已发布应用程序。|
|[发布应用程序](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | 将应用程序发布到组织的应用程序目录。|
|[更新的已发布的应用程序](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | 更新组织的应用程序目录中的已发布应用程序。|
|[删除已发布的应用程序](../api/teamsapp-delete.md) | 无 | 从组织的应用程序目录中删除的已发布的应用程序。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| ID                  | string   | 目录应用程序的生成应用程序 ID （不同[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的开发人员提供的 ID。 |
| externalId          | string   | 目录中[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)的应用程序开发人员提供的 ID。 |
| displayName                | string   | 目录应用程序[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中应用程序开发人员提供的名称。 |
| distributionMethod  | teamsAppDistributionMethod     | 应用程序分配方法。 |

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod 值

|成员|值|Description|
|:---|:---|:---|
|存储|0| 应用程序都可以通过 Microsoft 团队应用程序商店的所有租户。|
|组织|1|只能在此租户应用程序。|
|sideloaded|2|应用程序是仅供用户/工作组其安装到。|

## <a name="relationships"></a>Relationships

| 关系 | 类型   | Description |
|:---------------|:--------|:----------|
|appDefinitions|[teamsAppDefinition](teamsappdefinition.md)集合| 每个版本的应用程序的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a>另请参阅

- [teamsAppInstallation](teamsappinstallation.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

