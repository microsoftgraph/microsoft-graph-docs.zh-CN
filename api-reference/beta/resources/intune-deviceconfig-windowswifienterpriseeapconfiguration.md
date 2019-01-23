---
title: windowsWifiEnterpriseEAPConfiguration 资源类型
description: 此实体提供声明的方法、 属性和由 Wifi CSP 公开的关系的说明。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c5e7f92c8b84512ae71144d379a38eac24eb08c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407093"
---
# <a name="windowswifienterpriseeapconfiguration-resource-type"></a>windowsWifiEnterpriseEAPConfiguration 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体提供声明的方法、 属性和由 Wifi CSP 公开的关系的说明。


继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 windowsWifiEnterpriseEAPConfigurations](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-list.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)集合|列出属性和[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象之间的关系。|
|[获取 windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-get.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|读取属性和[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的关系。|
|[创建 windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-create.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|创建新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。|
|[删除 windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-delete.md)|无|删除[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)。|
|[更新 windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-update.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|更新[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的属性。|

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
|preSharedKey|String|这是预共享的 WPA 个人 Wi-fi 网络密钥。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|指定的 Wifi 安全类型。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。 可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|指定 wifi 连接的按流量计费的连接限制类型。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。 可取值为：`unrestricted`、`fixed`、`variable`。|
|ssid|String|指定 wifi 连接的 SSID。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkName|String|指定的网络配置名称。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectAutomatically|Boolean|指定应在范围中自动连接是否 wifi 连接。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectToPreferredNetwork|Boolean|指定 wifi 连接是否应连接到时已连接到此的更多首选网络。  需要 ConnectAutomatically 为 true。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|指定是否 wifi 连接应自动连接即使时 SSID 未进行广播。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|指定从[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)设置 Wi-fi 配置继承的代理。 可取值为：`none`、`manual`、`automatic`。|
|proxyManualAddress|String|指定代理服务器的 IP 地址。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyManualPort|Int32|指定的代理服务器的端口。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|指定代理服务器配置脚本的 URL。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|forceFIPSCompliance|Boolean|指定是否强制 FIPS 合规性。 继承自[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkSingleSignOn|[networkSingleSignOnType](../resources/intune-deviceconfig-networksinglesignontype.md)|指定网络单一登录类型。 可取值为：`disabled`、`prelogon`、`postlogon`。|
|maximumAuthenticationTimeoutInSeconds|Int32|指定最大的身份验证超时 （以秒为单位）。  有效的范围： 1-120|
|promptForAdditionalAuthenticationCredentials|Boolean|指定 wifi 连接是否应提示其他身份验证凭据。|
|enablePairwiseMasterKeyCaching|Boolean|指定 wifi 连接是否应启用缓存成对的主密钥。|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|指定最大成对主密钥缓存时间 （以分钟为单位）。  有效的范围： 5 1440年|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|在缓存中指定成对的主密钥的最大数量。  有效的范围： 1 到 255|
|enablePreAuthentication|Boolean|指定是否应启用预身份验证。|
|maximumPreAuthenticationAttempts|Int32|指定最大预身份验证尝试。  有效的范围： 1-16|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|可扩展的身份验证协议 (EAP)。 指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。 可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。|
|trustedServerCertificateNames|String 集合|指定受信任的服务器证书名称。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|指定的身份验证方法。 可取值为：`certificate`、`usernameAndPassword`。|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|指定 EAP TTL 内部身份验证协议。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|String|指定要使用 EAP TTL 或 PEAP 时替换为隐私的用户名的字符串。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|rootCertificatesForServerValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)集合|指定 server 验证的根证书。|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|指定标识的客户端身份验证的证书。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiEnterpriseEAPConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "String",
  "maximumAuthenticationTimeoutInSeconds": 1024,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 1024,
  "maximumNumberOfPairwiseMasterKeysInCache": 1024,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```




