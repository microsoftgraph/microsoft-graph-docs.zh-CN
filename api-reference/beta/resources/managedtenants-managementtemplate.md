---
title: managementTemplate 资源类型
description: 表示一组可以针对托管租户执行的操作和设置。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2055db2d291dce3da0b4ad144c07b09bbb2fea6f
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402277"
---
# <a name="managementtemplate-resource-type"></a>managementTemplate 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一组可以针对托管租户执行的操作和设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managementTemplates](../api/managedtenants-managedtenant-list-managementtemplates.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) 集合|获取 [managementTemplate 对象](../resources/managedtenants-managementtemplate.md) 及其属性的列表。|
|[获取 managementTemplate](../api/managedtenants-managementtemplate-get.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|读取 [managementTemplate](../resources/managedtenants-managementtemplate.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|category|managementCategory|管理模板的管理类别。 可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。 必填。 只读。|
|说明|String|管理模板的说明。 可选。 只读。|
|displayName|String|管理显示名称的表单。 必填。 只读。|
|id|String|管理模板的唯一标识符。 必填。 只读。|
|parameters|[microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md) 集合|管理模板使用的参数集合。 可选。 只读。|
|workloadActions|[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) 集合|与管理模板关联的工作负荷操作的集合。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.managedTenants.templateParameter"
    }
  ],
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
