---
title: iosikEv2VpnConfiguration 资源类型
description: 通过在此配置文件中提供配置，你可以指示 iOS 设备连接到所需的 IKEv2 VPN 终结点。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 93bfdaa2ee10c096a6141eaf6ed0531ddcb8742d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867474"
---
# <a name="iosikev2vpnconfiguration-resource-type"></a>iosikEv2VpnConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过在此配置文件中提供配置，你可以指示 iOS 设备连接到所需的 IKEv2 VPN 终结点。


继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 iosikEv2VpnConfigurations](../api/intune-deviceconfig-iosikev2vpnconfiguration-list.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 集合|列出 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象的属性和关系。|
|[获取 iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-get.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|读取 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象的属性和关系。|
|[创建 iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-create.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|创建新的 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象。|
|[删除 iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-delete.md)|无|删除 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)。|
|[Update iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-update.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|更新 [iosikEv2VpnConfiguration 对象](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|connectionName|String|向用户显示的连接名称。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|连接类型。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可能的值是 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` ：、、、、、、、、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。|
|loginGroupOrDomain|String|连接类型设置为 Dell SonicWALL 移动连接时登录组或域。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|String|将连接类型设置为 Pulse Secure 时的角色。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|realm|String|将连接类型设置为 Pulse Secure 时的领域。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|VPN 服务器。 确保最终用户可以访问此网络位置。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|标识符|String|连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。 例如：Cisco AnyConnect 使用 com.cisco.anyconnect.applevpn.plugin 形式的标识符 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合|连接类型设置为自定义 VPN 时自定义数据。 使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。 请联系 VPN 供应商，了解如何添加这些键/值对。 此集合最多可包含 25 个元素。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|连接类型设置为自定义 VPN 时自定义数据。 使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。 请联系 VPN 供应商，了解如何添加这些键/值对。 此集合最多可包含 25 个元素。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|enableSplitTunneling|Boolean|通过 VPN 发送所有网络流量。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|此 VPN 连接的身份验证方法。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。|
|enablePerApp|Boolean|如果设置为 true，Per-App VPN 有效负载，稍后可关联到可在最终用户的 iOS 设备上触发此 VPN 连接的应用。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|safariDomains|String 集合|启用"每个应用此 VPN"设置时，Safari 域。 除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合|按需规则。 该集合最多可包含 500 个元素。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|providerType|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|每个应用 VPN 的提供程序类型。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可取值为：`notConfigured`、`appProxy`、`packetTunnel`。|
|associatedDomains|String 集合|关联域 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|excludedDomains|String 集合|通过公共 Internet 而不是 VPN 访问的域，即使已激活每应用 VPN 也是如此。继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disableOnDemandUserOverride|Boolean|切换以阻止用户在"设置"应用中禁用自动 VPN 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdle|Boolean|是否在按需连接空闲后断开连接 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdleTimerInSeconds|Int32|断开按需连接之前要等待的时间长度（秒）。 有效值 0 至 65535 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|代理服务器。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|optInToDeviceIdSharing|Boolean|Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|userDomain|String|仅 Zscaler。 输入静态域，以在 Zscaler 应用中预填充登录字段。 如果为空，将改为使用用户的 Azure Active Directory 域。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|strictEnforcement|Boolean|仅 Zscaler。 阻止网络流量，直到用户登录 Zscaler 应用。 "True"表示流量被阻止。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|cloudName|String|仅 Zscaler。 用户分配到的 Zscaler 云。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|excludeList|String 集合|仅 Zscaler。 未通过 Zscaler 云发送的网络地址列表。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|targetedMobileApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|目标移动应用。 该集合最多可包含 500 个元素。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|microsoftTunnelSiteId|String|Microsoft 隧道站点 ID。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|childSecurityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|子安全关联参数|
|clientAuthenticationType|[vpnClientAuthenticationType](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|VPN 客户端将使用的客户端身份验证的类型。 可取值为：`userAuthentication`、`deviceAuthentication`。|
|deadPeerDetectionRate|[vpnDeadPeerDetectionRate](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|确定检查对等连接是否仍处于活动状态频繁。 . 可取值为：`medium`、`none`、`low`、`high`。|
|disableMobilityAndMultihoming|Boolean|禁用 MOBIKE|
|disableRedirect|Boolean|禁用重定向|
|enableCertificateRevocationCheck|Boolean|启用最佳吊销检查;服务器响应超时不会导致失败|
|enableEAP|Boolean|启用仅 EAP 身份验证|
|enablePerfectForwardSecrecy|Boolean|启用"完全向前保密" (PFS) 。|
|enableUseInternalSubnetAttributes|Boolean|启用"使用内部子网属性"。|
|localIdentifier|[vpnLocalIdentifier](../resources/intune-deviceconfig-vpnlocalidentifier.md)|用于标识尝试通过 VPN 连接的客户端的方法。 . 可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。|
|remoteIdentifier|String|IKEv2 服务器的地址。 必须是 FQDN、UserFQDN、网络地址或 ASN1DN|
|securityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|安全关联参数|
|serverCertificateCommonName|String|服务器身份验证中使用的 IKEv2 服务器证书的公用名|
|serverCertificateIssuerCommonName|String|颁发者 身份验证中使用的 IKEv2 服务器证书颁发者公用名|
|serverCertificateType|[vpnServerCertificateType](../resources/intune-deviceconfig-vpnservercertificatetype.md)|VPN 服务器将呈现给 VPN 客户端以进行身份验证的证书类型。 可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。|
|sharedSecret|String|在选择"共享密码身份验证"时使用|
|tlsMaximumVersion|String|要与 EAP-TLS 身份验证一同使用的最大 TLS 版本|
|tlsMinimumVersion|String|要与 EAP-TLS 身份验证一起使用的最低 TLS 版本|
|allowDefaultSecurityAssociationParameters|Boolean|除非明确指定，否则允许使用安全关联参数，具体方法为将所有参数设置为设备默认值。|
|allowDefaultChildSecurityAssociationParameters|Boolean|除非明确指定，否则允许使用子安全关联参数，具体方法为将所有参数设置为设备默认值。|
|alwaysOnConfiguration|[appleVpnAlwaysOnConfiguration](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|AlwaysOn 配置|
|enableAlwaysOnConfiguration|Boolean|确定是否启用始终启用 VPN|
|mtuSizeInBytes|Int32|最大传输单元数。 有效值为 1280 至 1400|

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
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|身份验证方法为证书时用于客户端身份验证的标识证书。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|要用于身份验证的派生凭据的租户级别设置。 继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosikEv2VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
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
  "microsoftTunnelSiteId": "String",
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "clientAuthenticationType": "String",
  "deadPeerDetectionRate": "String",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "String",
  "remoteIdentifier": "String",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "serverCertificateCommonName": "String",
  "serverCertificateIssuerCommonName": "String",
  "serverCertificateType": "String",
  "sharedSecret": "String",
  "tlsMaximumVersion": "String",
  "tlsMinimumVersion": "String",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "String",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "String",
    "airPrintExceptionAction": "String",
    "cellularExceptionAction": "String",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "String"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 1024,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 1024
}
```




