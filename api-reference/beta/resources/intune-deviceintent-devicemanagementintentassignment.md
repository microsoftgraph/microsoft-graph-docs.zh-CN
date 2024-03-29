---
title: deviceManagementIntentAssignment 资源类型
description: 意图分配实体
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8cc2ef384439c11d8be7a21ffc4965cd49d056ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137957"
---
# <a name="devicemanagementintentassignment-resource-type"></a>deviceManagementIntentAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

意图分配实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementIntentAssignments](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) 集合|列出 [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) 对象的属性和关系。|
|[获取 deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|读取 [deviceManagementIntentAssignment 对象的属性和](../resources/intune-deviceintent-devicemanagementintentassignment.md) 关系。|
|[创建 deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|创建新的 [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) 对象。|
|[删除 deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|无|删除 [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)。|
|[更新 deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|更新 [deviceManagementIntentAssignment 对象](../resources/intune-deviceintent-devicemanagementintentassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|工作分配 ID|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|工作分配目标|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```



