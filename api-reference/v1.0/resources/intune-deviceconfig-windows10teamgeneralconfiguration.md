---
title: windows10TeamGeneralConfiguration 资源类型
description: 本主题提供由 windows10TeamGeneralConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9fedf05eaac3453079d4c80514653e5b59909eb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056016"
---
# <a name="windows10teamgeneralconfiguration-resource-type"></a>windows10TeamGeneralConfiguration 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 windows10TeamGeneralConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windows10TeamGeneralConfigurations](../api/intune-deviceconfig-windows10teamgeneralconfiguration-list.md)|[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 集合|列出 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性和关系。|
|[Get windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-get.md)|[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)|读取 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性和关系。|
|[Create windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-create.md)|[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)|创建新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。|
|[Delete windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-delete.md)|无|删除 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)。|
|[Update windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-update.md)|[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)|更新 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|azureOperationalInsightsBlockTelemetry|Boolean|指示是否阻止 Azure 操作见解。|
|azureOperationalInsightsWorkspaceId|String|Azure 操作见解工作区 ID。|
|azureOperationalInsightsWorkspaceKey|String|Azure 操作见解工作区键。|
|connectAppBlockAutoLaunch|Boolean|指定是否在启动投影时自动启动 Connect 应用。|
|maintenanceWindowBlocked|Boolean|指示是否阻止设置设备更新的维护时段。|
|maintenanceWindowDurationInHours|Int32|设备更新的维护时段持续时间。 有效值为 0 至 5|
|maintenanceWindowStartTime|TimeOfDay|设备更新的维护时段开始时间。|
|miracastChannel|[miracastChannel](../resources/intune-deviceconfig-miracastchannel.md)|频道。 可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。|
|miracastBlocked|Boolean|指示是否阻止无线投影。|
|miracastRequirePin|Boolean|指示是否需要 PIN 才能进行无线投影。|
|settingsBlockMyMeetingsAndFiles|Boolean|指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。|
|settingsBlockSessionResume|Boolean|指定是否允许在会话超时时恢复会话。|
|settingsBlockSigninSuggestions|Boolean|指定是否禁用计划会议的被邀请者自动填充登录对话框。|
|settingsDefaultVolume|Int32|指定新会话的默认音量值。 允许的值为 0-100。 默认值为 45。 有效值为 0 至 100|
|settingsScreenTimeoutInMinutes|Int32|指定 Hub 屏幕关闭前的分钟数。|
|settingsSessionTimeoutInMinutes|Int32|指定会话超时前的分钟数。|
|settingsSleepTimeoutInMinutes|Int32|指定 Hub 进入睡眠模式前的分钟数。|
|welcomeScreenBlockAutomaticWakeUp|Boolean|指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。|
|welcomeScreenBackgroundImageUrl|String|欢迎屏幕背景图像 URL。 URL 必须使用 HTTPS 协议并返回 PNG 图像。|
|welcomeScreenMeetingInformation|[welcomeScreenMeetingInformation](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|显示的欢迎屏幕会议信息。 可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10TeamGeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "String",
  "azureOperationalInsightsWorkspaceKey": "String",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 1024,
  "maintenanceWindowStartTime": "String (time of day)",
  "miracastChannel": "String",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 1024,
  "settingsScreenTimeoutInMinutes": 1024,
  "settingsSessionTimeoutInMinutes": 1024,
  "settingsSleepTimeoutInMinutes": 1024,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "String",
  "welcomeScreenMeetingInformation": "String"
}
```




