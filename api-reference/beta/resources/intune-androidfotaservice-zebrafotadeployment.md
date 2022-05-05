---
title: zebraFotaDeployment 资源类型
description: 描述设置、创建 FOTA 部署所需的部署设备组和部署状态的 Zebra FOTA 部署实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d3ba6ffd223320be5bfbe1b259768534a47941c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213183"
---
# <a name="zebrafotadeployment-resource-type"></a>zebraFotaDeployment 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述设置、创建 FOTA 部署所需的部署设备组和部署状态的 Zebra FOTA 部署实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 zebraFotaDeployments](../api/intune-androidfotaservice-zebrafotadeployment-list.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 集合|列出 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 对象的属性和关系。|
|[获取 zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-get.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|读取 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 对象的属性和关系。|
|[创建 zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-create.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|创建新的 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 对象。|
|[删除 zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-delete.md)|无|删除 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)。|
|[更新 zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-update.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|更新 [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) 对象的属性。|
|[取消操作](../api/intune-androidfotaservice-zebrafotadeployment-cancel.md)|Boolean|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|在创建部署期间提供的系统生成的部署 ID。 仅当操作成功时才返回。|
|displayName|String|部署的人工可读名称。|
|说明|字符串|有关部署的人工可读说明。|
|deploymentSettings|[zebraFotaDeploymentSettings](../resources/intune-androidfotaservice-zebrafotadeploymentsettings.md)|表示创建部署所需的设置，例如部署类型、项目信息、下载和安装|
|deploymentAssignments|[androidFotaDeploymentAssignment](../resources/intune-androidfotaservice-androidfotadeploymentassignment.md) 集合|Android FOTA 分配的集合|
|deploymentStatus|[zebraFotaDeploymentStatus](../resources/intune-androidfotaservice-zebrafotadeploymentstatus.md)|表示 Zebra 的部署状态。 状态是部署的高级状态，而不是每个设备的详细状态。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaDeployment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "String",
    "updateType": "String",
    "timeZoneOffsetInMinutes": 1024,
    "firmwareTargetBoardSupportPackageVersion": "String",
    "firmwareTargetPatch": "String",
    "firmwareTargetOsVersion": "String",
    "scheduleMode": "String",
    "scheduleDurationInDays": 1024,
    "downloadRuleNetworkType": "String",
    "downloadRuleStartDateTime": "String (timestamp)",
    "installRuleStartDateTime": "String (timestamp)",
    "installRuleWindowStartTime": "String (time of day)",
    "installRuleWindowEndTime": "String (time of day)",
    "batteryRuleMinimumBatteryLevelPercentage": 1024,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "String",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "String"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "String",
    "totalDevices": 1024,
    "totalCreated": 1024,
    "totalScheduled": 1024,
    "totalDownloading": 1024,
    "totalAwaitingInstall": 1024,
    "totalSucceededInstall": 1024,
    "totalCanceled": 1024,
    "totalUnknown": 1024,
    "totalFailedDownload": 1024,
    "totalFailedInstall": 1024,
    "completeOrCanceledDateTime": "String (timestamp)",
    "cancelRequested": true,
    "lastUpdatedDateTime": "String (timestamp)"
  }
}
```




