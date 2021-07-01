---
title: teamworkTagIdentity 资源类型
description: 表示标记中的Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b9ea11746a98fba8bb209112c1cb6b1ed63fc954
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211080"
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

