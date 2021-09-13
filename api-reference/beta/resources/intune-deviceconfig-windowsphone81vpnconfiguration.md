---
title: windowsPhone81VpnConfiguration 资源类型
description: 通过在此配置文件中提供配置，你可以指示 Windows Phone 8.1 连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，你可以为最终用户无缝进行 VPN 连接。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72eeffc3336fe9fea6da356a017651b8493e3e26
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147883"
---
# <a name="windowsphone81vpnconfiguration-resource-type"></a>windowsPhone81VpnConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过在此配置文件中提供配置，你可以指示 Windows Phone 8.1 连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，你可以为最终用户无缝进行 VPN 连接。


继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsPhone81VpnConfigurations](../api/intune-deviceconfig-windowsphone81vpnconfiguration-list.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 集合|列出 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 对象的属性和关系。|
|[获取 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-get.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|读取 [windowsPhone81VpnConfiguration 对象的属性和](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 关系。|
|[创建 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-create.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|创建新的 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 对象。|
|[删除 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-delete.md)|无|删除 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)。|
|[更新 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-update.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|更新 [windowsPhone81VpnConfiguration 对象](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|connectionName|String|向用户显示的连接名称。 继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|服务器|[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合|网络上 VPN 服务器的列表。 确保最终用户可以访问这些网络位置。 该集合最多可包含 500 个元素。 继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|二进制|配置 VPN 连接的自定义 XML 命令。  (UTF8 编码的字节数组) 继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|applyOnlyToWindows81|Boolean|指示此策略是否仅适用于 Windows 8.1 的值。 此属性是只读的。 继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|connectionType|[windowsVpnConnectionType](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|连接类型。 继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。 可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。|
|loginGroupOrDomain|String|连接类型设置为 Dell SonicWALL 移动连接时登录组或域。 继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|enableSplitTunneling|Boolean|为 VPN 启用拆分隧道。 继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|proxyServer|[windows81VpnProxyServer](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|代理服务器。 继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|bypassVpnOnCompanyWifi|Boolean|在公司 WI-Fi 上绕过 VPN。|
|bypassVpnOnHomeWifi|Boolean|在家庭 WI-Fi 上绕过 VPN。|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。|
|rememberUserCredentials|Boolean|请记住用户凭据。|
|dnsSuffixSearchList|字符串集合|DNS 后缀搜索列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|identityCertificate|[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)|身份验证方法为证书时用于客户端身份验证的标识证书。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "applyOnlyToWindows81": true,
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "String"
  ]
}
```



