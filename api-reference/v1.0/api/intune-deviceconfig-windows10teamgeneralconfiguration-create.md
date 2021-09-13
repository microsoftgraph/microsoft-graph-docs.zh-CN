---
title: 创建 windows10TeamGeneralConfiguration
description: 创建新的 windows10TeamGeneralConfiguration 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58b2e665d5dd744a3efb2ee8befa5faae93e534a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59140064"
---
# <a name="create-windows10teamgeneralconfiguration"></a>创建 windows10TeamGeneralConfiguration

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 windows10TeamGeneralConfiguration 对象的 JSON 表示形式。

下表显示了创建 windows10TeamGeneralConfiguration 时所需的属性。

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



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```




