---
title: managementAction 资源类型
description: 表示给定托管租户的基线管理操作。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 156d4ff0d7ffb9574793ccdd5d56bc2a89cd3b22
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402400"
---
# <a name="managementaction-resource-type"></a>managementAction 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的基线管理操作。 管理操作的示例包括设备加密、执行配置Azure Active Directory注册设备，以及要求管理员进行多重身份验证。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managementActions](../api/managedtenants-managedtenant-list-managementactions.md)|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) 集合|获取 [managementAction 对象](../resources/managedtenants-managementaction.md) 及其属性的列表。|
|[获取 managementAction](../api/managedtenants-managementaction-get.md)|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|读取 [managementAction](../resources/managedtenants-managementaction.md) 对象的属性和关系。|
|[apply](../api/managedtenants-managementaction-apply.md)|[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)|对托管租户应用管理操作。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|category|managementCategory|管理操作类别。 可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。 可选。 只读。|
|说明|String|管理操作的说明。 可选。 只读。|
|displayName|String|管理显示名称的项。 可选。 只读。|
|id|String|管理操作的唯一标识符。 必填。 只读。|
|referenceTemplateId|String|用于生成管理操作的管理模板的引用。 必填。 只读。|
|workloadActions|[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) 集合|与管理操作关联的工作负荷操作的集合。 必填。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementAction",
  "id": "String (identifier)",
  "referenceTemplateId": "String",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
