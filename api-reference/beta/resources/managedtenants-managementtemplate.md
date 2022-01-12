---
title: managementTemplate 资源类型
description: 表示一组可以针对托管租户执行的操作和设置。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 6dacd5d94c921ca4afd59219be24509f6879c5b8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792048"
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
|category|managementCategory|管理模板的管理类别。 可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。 必需。 只读。|
|说明|String|管理模板的说明。 可选。 只读。|
|displayName|String|管理显示名称的表单。 必需。 只读。|
|id|String|管理模板的唯一标识符。 必需。 只读。|
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
