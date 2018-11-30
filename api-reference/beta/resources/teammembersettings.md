---
title: teamMemberSettings 资源类型
description: 例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。
ms.openlocfilehash: fa673e050ab3362ae7b132f30cfc4caf16d96dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041890"
---
# <a name="teammembersettings-resource-type"></a>teamMemberSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加[团队](team.md)中。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|布尔|如果设置为 true，则成员可以添加和更新通道。|
|allowDeleteChannels|布尔|如果设置为 true，则成员可以删除通道。|
|allowAddRemoveApps|布尔|如果设置为 true，则成员可以添加和删除应用程序。|
|allowCreateUpdateRemoveTabs|布尔|如果设置为 true，则成员可以添加、 更新和删除选项卡。 |
|allowCreateUpdateRemoveConnectors|布尔|如果设置为 true，则成员可以添加、 更新和删除连接器。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
