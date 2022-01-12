---
title: managementIntent 资源类型
description: 表示基线的元数据以及包含哪些管理模板。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c3e4954e34768b711f621efe98b00eda5baae1d9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791929"
---
# <a name="managementintent-resource-type"></a>managementIntent 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示基线的元数据以及包含哪些管理模板。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managementIntents](../api/managedtenants-managedtenant-list-managementintents.md)|[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) 集合|获取 [managementIntent 对象及其](../resources/managedtenants-managementintent.md) 属性的列表。|
|[获取 managementIntent](../api/managedtenants-managementintent-get.md)|[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|读取 [managementIntent](../resources/managedtenants-managementintent.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|管理显示名称目的的一个方法。 可选。 只读。|
|id|String|管理意图的唯一标识符。 必需。 只读。|
|isGlobal|布尔|指示管理意图是否全局的标志。 必需。 只读。|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) 集合|与管理意图关联的管理模板的集合。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementIntent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "isGlobal": "Boolean",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
