---
title: zebraFotaDeploymentSettings 资源类型
description: Zebra FOTA 部署复杂类型，描述创建 FOTA 部署所需的设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b055ae91e93919a3f6b8af63d7ae7a207ffaaac
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213197"
---
# <a name="zebrafotadeploymentsettings-resource-type"></a>zebraFotaDeploymentSettings 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Zebra FOTA 部署复杂类型，描述创建 FOTA 部署所需的设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceModel|String|仅使用此模型为设备部署更新。|
|updateType|[zebraFotaUpdateType](../resources/intune-androidfotaservice-zebrafotaupdatetype.md)|部署的更新类型。 可能的值为自定义值、最新值和自动值。设置自定义模式时，请求必须提供项目值。 设置最新类型时，最新发布的更新将成为目标 OS。 如果指定了最新值，则不需要固件目标值。 注意：最新版本可能会将设备更新为新的 Android 版本。 当值设置为自动时，设备始终查找可用的最新包，并在有新包可用时尝试更新。 这会一直持续到管理员取消自动更新为止。 虽然其他模式返回以 FOTA-x 开头的 ID，但自动模式返回以 AUTO-x 开头的 ID。 可能的值是：`custom`、`latest`、`auto`、`unknownFutureValue`。|
|timeZoneOffsetInMinutes|Int32|此属性指示部署时间偏移量 (例如`180` 表示偏移 `+03:00`量，并 `-270` 表示) 的 `-04:30` 偏移量。 时间偏移量是设备所在的时区。 部署开始和结束数据使用此时区|
|firmwareTargetBoardSupportPackageVersion|String|部署的开发板支持包 (BSP。 G.g.：'01.18.02.00') 。 仅需要自定义更新类型。|
|firmwareTargetPatch|String|目标修补程序名称 (，即：“U06”) 。 仅需要自定义更新类型。|
|firmwareTargetOsVersion|String|目标 OS 版本 (，即“8.1.0”) 。 仅需要自定义更新类型。|
|scheduleMode|[zebraFotaScheduleMode](../resources/intune-androidfotaservice-zebrafotaschedulemode.md)|部署安装计划模式。 默认值为 installNow。 所有计划的部署日期和时间都在设备的时区中。 对于立即安装，日期和时间位于 UTC 中 () 世界任何地方的相同日期和时间。 可取值为：`installNow`、`scheduled`、`unknownFutureValue`。|
|scheduleDurationInDays|Int32|最大 28 天。 默认值为 28 天。 日期序列为：1) 下载开始日期。 2) 安装开始日期。 3) 计划结束日期。 如果未提供任何值，则使用序列前面步骤中提供的日期。 如果未提供任何值，则使用当前 UTC 的字符串值。|
|downloadRuleNetworkType|[zebraFotaNetworkType](../resources/intune-androidfotaservice-zebrafotanetworktype.md)|下载网络类型，如“zebraFotaNetworkType”中所述。 默认值：任意。 可取值为：`any`、`wifi`、`cellular`、`wifiAndCellular`、`unknownFutureValue`。|
|downloadRuleStartDateTime|DateTimeOffset|启动下载的设备时区中的日期和时间 (例如， `2018-07-25T10:20:32`) 。 默认值现在是 UTC，最大值为部署创建后的 10 天。|
|installRuleStartDateTime|DateTimeOffset|安装开始时的设备时区中的日期和时间。 默认值 - 如果已配置，则下载 startDate，否则默认为 NOW。 当部署更新类型设置为自动时忽略。|
|installRuleWindowStartTime|TimeOfDay|一天中的时间 (00：00：00 - 23：30：00) 何时开始安装。 时间以 24 小时格式表示，为 hh：mm，位于设备时区中。 默认值 - 00：00：00。 受所有更新类型的值（包括 AUTO）的尊重。|
|installRuleWindowEndTime|TimeOfDay|安装无法启动的一天中的时间。 可能的范围为 00：30：00 到 23：59：59。 应大于“installRuleWindowStartTime”30 分钟。 时间以 24 小时格式表示，为 hh：mm，位于设备时区中。 默认值 - 23：59：59。 受所有更新类型的值（包括 AUTO）的尊重。|
|batteryRuleMinimumBatteryLevelPercentage|Int32|下载和安装所需的最低电池电量 (%) 。 默认值：-1 (系统默认值) 。 最大值为 100。|
|batteryRuleRequireCharger|Boolean|指示是否需要充电器的标志。 当设置为 false 时，客户端可以安装更新，无论设备是在充电器中还是在充电器外。 仅适用于安装。 默认值为 false。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeploymentSettings",
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
}
```




