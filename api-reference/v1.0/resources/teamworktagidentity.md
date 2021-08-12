---
title: teamworkTagIdentity 资源类型
description: 表示标记中的Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2f507844751b92493eab2c4bb84f2da2f3a04c8afb310b682ac9beb2f025031f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129937"
---
# <a name="teamworktagidentity-resource-type"></a>teamworkTagIdentity 资源类型

命名空间：microsoft.graph

代表 **Microsoft Teams** 中的标记。 标记允许用户快速连接到团队中的部分用户。 有关标记管理的详细信息，请参阅Microsoft Teams[中的管理Microsoft Teams。](/microsoftteams/manage-tags)


继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|继承自 [标识](../resources/identity.md)。 标记的显示名称。|
|id|String|继承自 [标识](../resources/identity.md)。 标记的 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTagIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagIdentity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

