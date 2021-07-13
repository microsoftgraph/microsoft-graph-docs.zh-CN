---
title: workloadAction 资源类型
description: 表示将为特定工作负荷执行的操作。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e6dbbe1458aa6dba37a26af70ee0e64b92a52cf4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402088"
---
# <a name="workloadaction-resource-type"></a>workloadAction 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示将为特定工作负荷执行的操作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionId|String|工作负荷操作的唯一标识符。 必填。 只读。|
|“类别”|workloadActionCategory|工作负荷操作类别。 可取值为：`automated`、`manual`、`unknownFutureValue`。 可选。 只读。|
|说明|String|工作负荷操作的说明。 可选。 只读。|
|displayName|String|工作负荷显示名称的项。 可选。 只读。|
|service|String|与工作负荷操作关联的服务。 可选。 只读。|
|settings|[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) 集合|与工作负荷操作关联的设置集合。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadAction",
  "actionId": "String",
  "category": "String",
  "displayName": "String",
  "description": "String",
  "service": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ]
}
```
