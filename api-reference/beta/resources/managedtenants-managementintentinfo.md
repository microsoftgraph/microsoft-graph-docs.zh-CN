---
title: managementIntentInfo 资源类型
description: 表示管理意图的关系信息。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 05442959aaa64ddc0fa1059ff599b18d421dcd7b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61789983"
---
# <a name="managementintentinfo-resource-type"></a>managementIntentInfo 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示管理意图的关系信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managementIntentDisplayName|String|管理显示名称目的的一个方法。 可选。 只读。|
|managementIntentId|String|管理意图的标识符。 必需。 只读。|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) 集合|与管理意图关联的管理模板信息的集合。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntentInfo",
  "managementIntentId": "String",
  "managementIntentDisplayName": "String",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
