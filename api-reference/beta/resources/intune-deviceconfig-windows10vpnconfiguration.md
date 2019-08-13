---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置, 可以指示 Windows 10 设备 (桌面或移动版) 连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 VPN 连接。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00908d1adb28cd7139be415497f8c972b6326b05
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369715"
---
# <a name="windows10vpnconfiguration-resource-type"></a>windows10VpnConfiguration 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过提供此配置文件中的配置, 可以指示 Windows 10 设备 (桌面或移动版) 连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 VPN 连接。


继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10VpnConfigurations](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合|列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。|
|[获取 windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|读取[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。|
|[创建 windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。|
|[删除 windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|无|删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。|
|[更新 windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|connectionName|String|向用户显示的连接名称。 继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|台|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合|网络上的 VPN 服务器的列表。 请确保最终用户可以访问这些网络位置。 该集合最多可包含 500 个元素。 继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|Binary|配置 VPN 连接的自定义 XML 命令。 (UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|profileTarget|[windows10VpnProfileTarget](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|配置文件目标类型。 可取值为：`user`、`device`、`autoPilotDevice`。|
|connectionType|[windows10VpnConnectionType](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|连接类型。 可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。|
|enableSplitTunneling|Boolean|启用拆分隧道。|
|enableAlwaysOn|Boolean|启用始终打开模式。|
|enableDeviceTunnel|Boolean|启用设备隧道。|
|enableDnsRegistration|Boolean|使用内部 DNS 启用 IP 地址注册。|
|dnsSuffixes|String collection|指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。|
|authenticationMethod|[windows10VpnAuthenticationMethod](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。|
|rememberUserCredentials|Boolean|记住用户凭据。|
|enableConditionalAccess|Boolean|启用条件访问。|
|enableSingleSignOnWithAlternateCertificate|Boolean|启用具有备用证书的单一登录 (SSO)。|
|singleSignOnEku|[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)|单一登录扩展密钥用法 (EKU)。|
|singleSignOnIssuerHash|String|单一登录颁发者哈希。|
|eapXml|Binary|可扩展的身份验证协议 (EAP) XML。 （UTF8 编码的字节数组）|
|proxyServer|[windows10VpnProxyServer](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|代理服务器。|
|associatedApps|[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合|关联的应用。 该集合最多可包含 10000 个元素。|
|onlyAssociatedAppsCanUseConnection|Boolean|仅关联的应用程序可以使用连接 (每个应用 VPN)。|
|windowsInformationProtectionDomain|String|与此连接关联的 Windows 信息保护 (WIP) 域。|
|trafficRules|[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合|流量规则。 该集合最多可包含 1000 个元素。|
|航线|[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合|路由 (可选用于第三方提供程序)。 该集合最多可包含 1000 个元素。|
|dnsRules|[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合|DNS 规则。 该集合最多可包含 1000 个元素。|
|trustedNetworkDomains|String collection|受信任的网络域|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|将 identitycertificate|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|在身份验证方法为证书时, 用于客户端身份验证的标识证书。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ]
}
```



