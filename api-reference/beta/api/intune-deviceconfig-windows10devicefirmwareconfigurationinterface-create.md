---
title: 创建 windows10DeviceFirmwareConfigurationInterface
description: 创建新的 windows10DeviceFirmwareConfigurationInterface 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ef1042b4942160c2491760ccbfc33358c772e8d
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857888"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a>创建 windows10DeviceFirmwareConfigurationInterface

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 对象。

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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 windows10DeviceFirmwareConfigurationInterface 对象提供 JSON 表示形式。

下表显示了创建 windows10DeviceFirmwareConfigurationInterface 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 如果此值为 false，并且作用域内用户不可见，则不允许分配到 ScopeTags 属性。 对于在 Silverlight 中创建的旧策略，可以通过在 Azure 门户中删除和重新创建策略来解决此问题。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的 OS 版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的 OS 版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|定义授予用户更改 UEFI 设置的权限级别。 可取值为：`notConfiguredOnly`、`none`。|
|virtualizationOfCpuAndIO|[支持](../resources/intune-shared-enablement.md)|定义是否启用 CPU 和 IO 虚拟化。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|相机|[支持](../resources/intune-shared-enablement.md)|定义是否启用内置相机。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|microphonesAndSpeakers|[支持](../resources/intune-shared-enablement.md)|定义是否启用内置麦克风或扬声器。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|收音机|[支持](../resources/intune-shared-enablement.md)|定义是否启用内置无线电，例如 WIFI、NFC、蓝牙。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|bootFromExternalMedia|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户从外部媒体启动。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|bootFromBuiltInNetworkAdapters|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户从内置网络适配器启动。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|windowsPlatformBinaryTable|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用Windows平台二进制表。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|simultaneousMultiThreading|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用同时进行多线程处理。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|frontCamera|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用 Front 相机。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|rearCamera|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用后置摄像头。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|infraredCamera|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用红外相机。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|麦克风|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用麦克风。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|蓝牙|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用蓝牙。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|wirelessWideAreaNetwork|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用无线广域网。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|nearFieldCommunication|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用近场通信。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|无线|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用 WiFi。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|usbTypeAPort|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用 USB 类型 A 端口。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|sdCard|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用 SD 卡端口。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|wakeOnLAN|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户在 LAN 上启用唤醒。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|wakeOnPower|[支持](../resources/intune-shared-enablement.md)|定义是否允许用户启用 Power 唤醒。 可取值为：`notConfigured`、`enabled`、`disabled`。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1754

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled",
  "frontCamera": "enabled",
  "rearCamera": "enabled",
  "infraredCamera": "enabled",
  "microphone": "enabled",
  "bluetooth": "enabled",
  "wirelessWideAreaNetwork": "enabled",
  "nearFieldCommunication": "enabled",
  "wiFi": "enabled",
  "usbTypeAPort": "enabled",
  "sdCard": "enabled",
  "wakeOnLAN": "enabled",
  "wakeOnPower": "enabled"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1926

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "id": "96474363-4363-9647-6343-479663434796",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled",
  "frontCamera": "enabled",
  "rearCamera": "enabled",
  "infraredCamera": "enabled",
  "microphone": "enabled",
  "bluetooth": "enabled",
  "wirelessWideAreaNetwork": "enabled",
  "nearFieldCommunication": "enabled",
  "wiFi": "enabled",
  "usbTypeAPort": "enabled",
  "sdCard": "enabled",
  "wakeOnLAN": "enabled",
  "wakeOnPower": "enabled"
}
```




