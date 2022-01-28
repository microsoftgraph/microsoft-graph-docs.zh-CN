---
title: teamworkDevice 资源类型
description: 表示有关Microsoft Teams租户预配的启用租户的设备的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7cd91f9901c02d1008e5c08a72c47e416222ab75
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262474"
---
# <a name="teamworkdevice-resource-type"></a>teamworkDevice 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关Microsoft Teams租户预配的启用租户的设备的详细信息。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 teamworkDevices](../api/teamworkdevice-list.md)|[teamworkDevice](../resources/teamworkdevice.md) 集合|获取为租户Microsoft Teams已启用设备的列表。|
|[获取 teamworkDevice](../api/teamworkdevice-get.md)|[teamworkDevice](../resources/teamworkdevice.md)|获取启用Microsoft Teams设备的属性。|
|[restart](../api/teamworkdevice-restart.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|重新启动已启用Microsoft Teams设备。|
|[runDiagnostics](../api/teamworkdevice-rundiagnostics.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|运行并生成指定已启用Microsoft Teams诊断日志。|
|[updateSoftware](../api/teamworkdevice-updatesoftware.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|更新启用了 Microsoft Teams 的设备的软件。|
|[列举操作](../api/teamworkdeviceoperation-list.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) 集合|获取在启用了移动设备的设备上Teams操作的列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|activityState|teamworkDeviceActivityState|设备的活动状态。 可能的值包括 `unknown`、`busy`、`idle`、`unavailable`、`unknownFutureValue`。|
|companyAssetTag|String|由设备上管理员分配的公司资产标记。|
|createdBy|[identitySet](../resources/identityset.md)|将设备注册到租户的用户的标识。|
|createdDateTime|DateTimeOffset|设备注册到租户的 UTC 日期和时间。|
|currentUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|设备上登录的用户。|
|deviceType|[teamworkDeviceType](../resources/teamworkdevice.md#teamworkdevicetype-values)|设备的类型。 可能的值包括：、`unknown``teamsRoom``ipPhone`、`surfaceHub`、`collaborationBar`、、`teamsDisplay`、、`touchConsole``sip``lowCostPhone``teamsPanel``unknownFutureValue`、。|
|hardwareDetail|[teamworkHardwareDetail](../resources/teamworkhardwaredetail.md)|硬件相关的属性的集合。 例如， **oemSerialNumber** 和 **model**。|
|healthStatus|[teamworkDeviceHealthStatus](../resources/teamworkdevice.md#teamworkdevicehealthstatus-values)|设备的运行状况。 可能的值包括 `unknown`、`offline`、`critical`、`nonUrgent`、`healthy`、`unknownFutureValue`。|
|id|字符串|设备标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改设备详细信息的用户的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备详细信息的 UTC 日期和时间。|
|notes|String|管理员添加到设备的注释。|


### <a name="teamworkdevicetype-values"></a>teamworkDeviceType 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|unknown|0|未知设备。|
|ipPhone|1|IP 电话设备是桌面电话，供用户拨打和接听音频呼叫或加入会议。|
|teamsRoom|2|Microsoft Teams 会议室基于 Windows IoT 的设备，旨在将会议体验扩展到会议室。|
|surfaceHub|3|Surface Hub是具有交互式白板的挂式或立式安装设备。|
|collaborationBar|4|Android 上Microsoft Teams 会议室用于小型会议空间的协作栏。|
|teamsDisplay|5|Teams设备是手机Teams演变。 这些设备是一类一体式专用Teams设备，具有环境触摸屏和由 Cortana 支持的免费Cortana。|
|touchConsole|6 |触摸控制台设备是 Android Teams 会议室执行所有设备操作的设备可选外设。|
|lowCostPhone|7 |低成本电话设备是经济高效的Microsoft Teams电话。|
|teamsPanel|8 |Microsoft Teams面板是紧凑式触摸屏设备，用于显示通过会议计划的会议Teams。|
|sip|9 |会话初始 (SIP) 支持Teams来自 Microsoft 的 SIP 网关进行呼叫的设备。|
|unknownFutureValue|10 |可发展枚举 sentinel 值。 请勿使用。|


### <a name="teamworkdevicehealthstatus-values"></a>teamworkDeviceHealthStatus 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|unknown|0|未知运行状况状态。|
|offline|1|设备处于脱机状态，无法使用。|
|critical|2|状态需要紧急注意和操作，因为它可能会显著影响设备的性能，或者使呼叫或会议无法使用状态。|
|nonUrgent|3|状态需要关注，因为问题或通知对联机设备的性能影响最小。|
|healthy|4|设备联机且状态良好。|
|unknownFutureValue|5|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|活动|[teamworkDeviceActivity](../resources/teamworkdeviceactivity.md)|根据设备使用情况更改的活动属性。|
|configuration|[teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md)|设备的配置属性。|
|health|[teamworkDeviceHealth](../resources/teamworkdevicehealth.md)|设备的运行状况属性。|
|operations|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) 集合|设备上异步操作。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDevice",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDevice",
  "activityState": "String",
  "companyAssetTag": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "currentUser": {
    "@odata.type": "microsoft.graph.teamworkUserIdentity"
  },
  "deviceType": "String",
  "hardwareDetail": {
    "@odata.type": "microsoft.graph.teamworkHardwareDetail"
  },
  "healthStatus": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "notes": "String"
}
```

