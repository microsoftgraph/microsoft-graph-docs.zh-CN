---
title: roleDefinition 资源类型
description: 表示角色定义的详细信息。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 6d2a34d8e6130a894341bcbbb735910c9357d3ce
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096351"
---
# <a name="roledefinition-resource-type"></a>roleDefinition 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示角色定义的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|角色的说明。|
|displayName|String|角色分配的显示名称。|
|templateId|String|模板的的唯一标识符。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.roleDefinition",
  "description": "String",
  "displayName": "String",
  "templateId": "String"
}
```
