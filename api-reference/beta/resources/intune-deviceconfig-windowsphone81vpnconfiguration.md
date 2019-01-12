---
title: windowsPhone81VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，您可以指示 Windows Phone 8.1，以连接到所需 VPN 终结点。 通过指定的身份验证方法和安全类型预期 VPN 终结点，可进行 VPN 连接无缝的最终用户。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 41d27504e7a8bb83385cd9707c9cdaeb08c6e927
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984554"
---
# <a name="windowsphone81vpnconfiguration-resource-type"></a>windowsPhone81VpnConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

通过提供此配置文件中的配置，您可以指示 Windows Phone 8.1，以连接到所需 VPN 终结点。 通过指定的身份验证方法和安全类型预期 VPN 终结点，可进行 VPN 连接无缝的最终用户。

继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 windowsPhone81VpnConfigurations](../api/intune-deviceconfig-windowsphone81vpnconfiguration-list.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)集合|列出属性和[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象之间的关系。|
|[获取 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-get.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|读取属性和[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的关系。|
|[创建 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-create.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|创建新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。|
|[删除 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-delete.md)|无|删除[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)。|
|[更新 windowsPhone81VpnConfiguration](../api/intune-deviceconfig-windowsphone81vpnconfiguration-update.md)|[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|更新[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|connectionName|字符串|向用户显示的连接名称。 继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|服务器|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合|VPN 服务器的网络上的列表。 确保最终用户可以访问这些网络位置。 该集合最多可包含 500 个元素。 继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|Binary|配置 VPN 连接的自定义 XML 命令。 （UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|applyOnlyToWindows81|Boolean|指示此策略是否仅适用于 Windows 8.1 的值。 此属性是只读的。 继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|连接|[windowsVpnConnectionType](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|连接类型。 继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。 可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。|
|loginGroupOrDomain|字符串|登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。 继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|enableSplitTunneling|Boolean|启用拆分隧道的 VPN。 继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|代理服务器|[windows81VpnProxyServer](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|代理服务器。 继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|
|bypassVpnOnCompanyWifi|Boolean|在公司 Wi-fi 绕过 VPN。|
|bypassVpnOnHomeWifi|Boolean|绕过 Wi-fi 主页上的 VPN。|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|身份验证方法。 可取值为：`certificate`、`usernameAndPassword`。|
|rememberUserCredentials|Boolean|请记住用户凭据。|
|dnsSuffixSearchList|String 集合|DNS 后缀搜索列表。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|identityCertificate|[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)|客户端身份验证证书身份验证方法时的标识证书。|

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





