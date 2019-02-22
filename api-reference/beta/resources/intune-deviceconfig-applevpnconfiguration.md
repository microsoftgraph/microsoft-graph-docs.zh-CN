---
title: appleVpnConfiguration 资源类型
description: Apple VPN 配置文件。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9f526e256a5ec8ecd4e364b4e017508a999ea17
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163299"
---
# <a name="applevpnconfiguration-resource-type"></a>appleVpnConfiguration 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Apple VPN 配置文件。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 appleVpnConfigurations](../api/intune-deviceconfig-applevpnconfiguration-list.md)|[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)集合|列出[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。|
|[获取 appleVpnConfiguration](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|读取[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|connectionName|字符串|向用户显示的连接名称。|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|连接类型。 可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、、、、、、、、、、。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso`|
|loginGroupOrDomain|字符串|将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。|
|role|字符串|将 "连接类型" 设置为 "脉冲安全" 时的角色。|
|领域|字符串|连接类型设置为脉冲安全时的领域。|
|服务器主板|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|网络上的 VPN 服务器。 请确保最终用户可以访问此网络位置。|
|标识符|字符串|当连接类型设置为自定义 vpn 时, 由 VPN 供应商提供的标识符。 例如: Cisco AnyConnect 使用 AnyConnect 形式的标识符。 applevpn 的标识符|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合|将连接类型设置为自定义 VPN 时的自定义数据。 使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。 请与你的 VPN 供应商联系, 了解如何添加这些键/值对。 此集合最多可包含25个元素。|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|将连接类型设置为自定义 VPN 时的自定义数据。 使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。 请与你的 VPN 供应商联系, 了解如何添加这些键/值对。 此集合最多可包含25个元素。|
|enableSplitTunneling|布尔|通过 VPN 发送所有网络流量。|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|此 VPN 连接的身份验证方法。 可取值为：`certificate`、`usernameAndPassword`。|
|enablePerApp|布尔|将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。|
|safariDomains|String collection|启用此 VPN 每应用程序设置时的 Safari 域。 除了与此 vpn 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 vpn 连接。|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合|按需规则。 该集合最多可包含 500 个元素。|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|代理服务器。|
|optInToDeviceIdSharing|布尔|选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。|

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

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnConfiguration",
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
  "optInToDeviceIdSharing": true
}
```




