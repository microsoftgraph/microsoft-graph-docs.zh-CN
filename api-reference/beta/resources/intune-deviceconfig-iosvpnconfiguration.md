---
title: iosVpnConfiguration 资源类型
description: 通过在此配置文件中提供配置，你可以指示 iOS 设备连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，你可以为最终用户无缝进行 VPN 连接。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 514c4f52d4fa69b227d269eb67848015d4b69b9e
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58253486"
---
# <a name="iosvpnconfiguration-resource-type"></a>iosVpnConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过在此配置文件中提供配置，你可以指示 iOS 设备连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，你可以为最终用户无缝进行 VPN 连接。


继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 iosVpnConfigurations](../api/intune-deviceconfig-iosvpnconfiguration-list.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 集合|列出 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象的属性和关系。|
|[获取 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-get.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|读取 [iosVpnConfiguration 对象的属性和](../resources/intune-deviceconfig-iosvpnconfiguration.md) 关系。|
|[创建 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-create.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|创建新的 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象。|
|[删除 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-delete.md)|无|删除 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。|
|[更新 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-update.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|更新 [iosVpnConfiguration 对象](../resources/intune-deviceconfig-iosvpnconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|布尔值|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|connectionName|String|向用户显示的连接名称。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|连接类型。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可能的值是 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` ：、、、、、、、、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。|
|loginGroupOrDomain|字符串|连接类型设置为 Dell SonicWALL 移动连接时登录组或域。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|String|将连接类型设置为 Pulse Secure 时的角色。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|realm|字符串|将连接类型设置为 Pulse Secure 时的领域。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|VPN 服务器。 确保最终用户可以访问此网络位置。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|标识符|String|连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。 例如：Cisco AnyConnect 使用 com.cisco.anyconnect.applevpn.plugin 形式的标识符 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合|连接类型设置为自定义 VPN 时自定义数据。 使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。 请联系 VPN 供应商，了解如何添加这些键/值对。 此集合最多可包含 25 个元素。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|[keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md) 集合|连接类型设置为自定义 VPN 时自定义数据。 使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。 请联系 VPN 供应商，了解如何添加这些键/值对。 此集合最多可包含 25 个元素。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|enableSplitTunneling|布尔值|通过 VPN 发送所有网络流量。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|此 VPN 连接的身份验证方法。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。|
|enablePerApp|布尔值|如果设置为 true，Per-App VPN 有效负载，稍后可关联到可在最终用户的 iOS 设备上触发此 VPN 连接的应用。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|safariDomains|String collection|启用"每个应用此 VPN"设置时，Safari 域。 除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合|按需规则。 该集合最多可包含 500 个元素。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|providerType|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|每个应用 VPN 的提供程序类型。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可取值为：`notConfigured`、`appProxy`、`packetTunnel`。|
|associatedDomains|String collection|关联域 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|excludedDomains|String collection|通过公共 Internet 而不是 VPN 访问的域，即使已激活每应用 VPN 也是如此。继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disableOnDemandUserOverride|布尔值|切换以阻止用户在应用中禁用自动 VPN 设置继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdle|布尔值|在按需连接空闲后是否断开连接 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdleTimerInSeconds|Int32|断开按需连接之前要等待的时间长度（秒）。 有效值 0 至 65535 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|代理服务器。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|optInToDeviceIdSharing|布尔值|Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|userDomain|String|仅 Zscaler。 在 Zscaler 应用中输入要预填充登录字段的静态域。 如果此域留空，将Azure Active Directory用户的域。|
|strictEnforcement|布尔值|仅 Zscaler。 阻止网络流量，直到用户登录 Zscaler 应用。 "True"表示流量被阻止。|
|cloudName|String|仅 Zscaler。 用户分配到的 Zscaler 云。|
|excludeList|String collection|仅 Zscaler。 未通过 Zscaler 云发送的网络地址列表。|
|targetedMobileApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|目标移动应用。 该集合最多可包含 500 个元素。|
|microsoftTunnelSiteId|字符串|Microsoft Tunnel网站 ID。|

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
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|身份验证方法为证书时用于客户端身份验证的标识证书。|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|要用于身份验证的派生凭据的租户级别设置。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "providerType": "String",
  "associatedDomains": [
    "String"
  ],
  "excludedDomains": [
    "String"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 1024,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true,
  "userDomain": "String",
  "strictEnforcement": true,
  "cloudName": "String",
  "excludeList": [
    "String"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "microsoftTunnelSiteId": "String"
}
```




