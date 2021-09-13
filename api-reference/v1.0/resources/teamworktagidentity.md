---
title: teamworkTagIdentity 资源类型
description: 表示标记中的Microsoft Teams。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7cd605a42f0f0c7f697c7b291fe30645bdf4403b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128170"
---
# <a name="teamworktagidentity-resource-type"></a>teamworkTagIdentity 资源类型

命名空间：microsoft.graph

代表 **Microsoft Teams** 中的标记。 标记允许用户快速连接到团队中的部分用户。 有关标记管理的详细信息，请参阅 Microsoft Teams[中的管理Microsoft Teams。](/microsoftteams/manage-tags)


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

