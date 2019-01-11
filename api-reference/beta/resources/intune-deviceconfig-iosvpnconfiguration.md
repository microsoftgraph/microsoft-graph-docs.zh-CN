---
title: iosVpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，您可以指示 iOS 设备，以连接到所需 VPN 终结点。 通过指定的身份验证方法和安全类型预期 VPN 终结点，可进行 VPN 连接无缝的最终用户。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4ab5b53c47022b106bbe337254d6f0b1043f83c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849516"
---
# <a name="iosvpnconfiguration-resource-type"></a>iosVpnConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

通过提供此配置文件中的配置，您可以指示 iOS 设备，以连接到所需 VPN 终结点。 通过指定的身份验证方法和安全类型预期 VPN 终结点，可进行 VPN 连接无缝的最终用户。

继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 iosVpnConfigurations](../api/intune-deviceconfig-iosvpnconfiguration-list.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)集合|列出属性和[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象之间的关系。|
|[获取 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-get.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|读取属性和[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象的关系。|
|[创建 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-create.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|创建新的[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象。|
|[删除 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-delete.md)|无|删除[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。|
|[更新 iosVpnConfiguration](../api/intune-deviceconfig-iosvpnconfiguration-update.md)|[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|更新[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|connectionName|字符串|向用户显示的连接名称。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|连接|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|连接类型。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可能的值为： `ciscoAnyConnect`， `pulseSecure`， `f5EdgeClient`， `dellSonicWallMobileConnect`， `checkPointCapsuleVpn`， `customVpn`， `ciscoIPSec`， `citrix`， `ciscoAnyConnectV2`， `paloAltoGlobalProtect`， `zscalerPrivateAccess`， `f5Access2018`， `citrixSso`， `paloAltoGlobalProtectV2`。|
|loginGroupOrDomain|字符串|登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|字符串|当连接类型设置为脉冲安全角色。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|领域|字符串|当连接类型设置为脉冲安全领域。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|服务器|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|在网络上的 VPN 服务器。 请确保最终用户可以访问此网络位置。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|标识符|字符串|当连接类型设置为自定义 VPN VPN 供应商提供的标识符。 例如： Cisco AnyConnect 使用[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)从窗体 com.cisco.anyconnect.applevpn.plugin 继承的标识符|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md)集合|当设置为自定义 VPN 连接类型的自定义数据。 使用此字段启用不支持 Intune，但在 VPN 解决方案中可用的功能。 了解如何添加这些键/值对 VPN 供应商联系。 此集合可以包含最多 25 元素。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|当设置为自定义 VPN 连接类型的自定义数据。 使用此字段启用不支持 Intune，但在 VPN 解决方案中可用的功能。 了解如何添加这些键/值对 VPN 供应商联系。 此集合可以包含最多 25 元素。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|enableSplitTunneling|布尔|将发送所有网络流量通过 VPN。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|此 VPN 连接的身份验证方法。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。 可取值为：`certificate`、`usernameAndPassword`。|
|enablePerApp|布尔|将此值设置为 true 时，创建更高版本可以是与可触发本 VPN 连接最终用户的 iOS 设备上的应用程序关联的每个应用程序 VPN 负载。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|safariDomains|String 集合|Safari 域时启用此 VPN 每应用程序设置。 与此 VPN 关联的应用程序，除了 Safari 域指定此处还将能够触发本 VPN 连接。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合|按需规则。 该集合最多可包含 500 个元素。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|代理服务器|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|代理服务器。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|optInToDeviceIdSharing|布尔|加入到共享网络访问控制验证过程中的第三方 vpn 客户端使用的设备的 Id。 继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|提供程序类型|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|每个应用程序 VPN 的提供程序类型。 可取值为：`notConfigured`、`appProxy`、`packetTunnel`。|
|userDomain|字符串|仅 Zscaler。 输入静态域预填充具有 Zscaler 应用程序中的登录字段。 如果这保留为空，将使用用户的 Azure Active Directory 域。|
|strictEnforcement|布尔|仅 Zscaler。 块到 Zscaler 应用程序直到用户迹象网络流量。 搕 rue 意味着阻止流量。|
|cloudName|字符串|仅 Zscaler。 该用户分配给 Zscaler 云。|
|excludeList|String 集合|仅 Zscaler。 不会通过 Zscaler 云发送的网络地址的列表。|

## <a name="relationships"></a>Relationships
|关系|类型|Description|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|客户端身份验证证书身份验证方法时的标识证书。|

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
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true,
  "providerType": "String",
  "userDomain": "String",
  "strictEnforcement": true,
  "cloudName": "String",
  "excludeList": [
    "String"
  ]
}
```





