---
title: windowsDefenderApplicationControlSupplementalPolicyAssignment 资源类型
description: 包含用于向组分配 WindowsDefenderApplicationControl 补充策略的属性的类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b410a9fd4d6d9b8dbf51711436a30d7834b1261
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100825"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicyassignment-resource-type"></a>windowsDefenderApplicationControlSupplementalPolicyAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于向组分配 WindowsDefenderApplicationControl 补充策略的属性的类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsDefenderApplicationControlSupplementalPolicyAssignments](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-list.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) 集合|列出 [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) 对象的属性和关系。|
|[获取 windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-get.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|读取 [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) 对象的属性和关系。|
|[创建 windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-create.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|创建新的 [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) 对象。|
|[删除 windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-delete.md)|无|删除 [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)。|
|[更新 windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-update.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|更新 [windowsDefenderApplicationControlSupplementalPolicyAssignment 对象](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|由管理员定义的目标组分配。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



