---
title: iosEnterpriseWiFiConfiguration 资源类型
description: 通过提供此配置文件中的配置，可以指示 iOS 设备连接到所需的Wi-Fi终结点。 通过指定Wi-Fi终结点所需的身份验证方法和安全类型，可以使最终用户的Wi-Fi连接无缝。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d080ae2b0d4521e9ad3f9661413b23b935632ec2
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669131"
---
# <a name="iosenterprisewificonfiguration-resource-type"></a>iosEnterpriseWiFiConfiguration 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过提供此配置文件中的配置，可以指示 iOS 设备连接到所需的Wi-Fi终结点。 通过指定Wi-Fi终结点所需的身份验证方法和安全类型，可以使最终用户的Wi-Fi连接无缝。


继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 iosEnterpriseWiFiConfigurations](../api/intune-deviceconfig-iosenterprisewificonfiguration-list.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) 集合|列出 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) 对象的属性和关系。|
|[获取 iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-get.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|读取 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) 对象的属性和关系。|
|[创建 iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-create.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|创建新的 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) 对象。|
|[删除 iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-delete.md)|None|删除 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)。|
|[更新 iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-update.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|更新 [iosEnterpriseWiFiConfiguration 对象的](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础设备配置是否支持分配范围标记。 如果此值为 false，并且作用域内用户不可见，则不允许分配到 ScopeTags 属性。 对于在 Silverlight 中创建的旧策略，可以通过在 Azure 门户中删除和重新创建策略来解决此问题。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的 OS 版本适用性。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的 OS 版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|networkName|String|从 [iosWiFiConfiguration 继承的](../resources/intune-deviceconfig-ioswificonfiguration.md)网络名称|
|Ssid|String|这是向所有设备广播的Wi-Fi网络的名称。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectAutomatically|Boolean|此网络处于范围内时自动连接。 将此设置为 true 将跳过用户提示，并自动将设备连接到Wi-Fi网络。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|布尔|当网络未 (SSID) 广播其名称时进行连接。 设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|指示Wi-Fi终结点是否使用基于 EAP 的安全类型。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。 可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|此Wi-Fi连接的代理类型继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。 可取值为：`none`、`manual`、`automatic`。|
|proxyManualAddress|String|选择手动配置时，代理服务器的 IP 地址或 DNS 主机名。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyManualPort|Int32|选择手动配置时代理服务器的端口。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|选择自动配置时代理服务器自动配置脚本的 URL。 此 URL 通常是 PAC (代理自动配置) 文件的位置。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|disableMacAddressRandomization|Boolean|如果设置为 true，则强制使用此Wi-Fi配置文件进行连接的设备显示其实际Wi-Fi MAC 地址，而不是随机 MAC 地址。 适用于 iOS 14 及更高版本。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|preSharedKey|String|这是 WPA 个人Wi-Fi网络的预共享密钥。 继承自 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|EAP)  (可扩展身份验证协议。 指示在路由器)  (Wi-Fi终结点上设置的 EAP 协议的类型。 可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` 或 `teap`。|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|当 EAP-FAST 是选定的 EAP 类型时，EAP-FAST 配置选项。 可能的值是：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。|
|trustedServerCertificateNames|字符串集合|将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时，受信任的服务器证书名称。 这是受信任证书颁发机构 (CA) 颁发的证书中使用的常见名称。 如果提供此信息，则可以在最终用户连接到此Wi-Fi网络时绕过在最终用户设备上显示的动态信任对话框。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|将 EAP 类型配置为 PEAP 或 EAP-TTLS 时的身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|当 EAP 类型为 EAP-TTLS 且 Authenticationmethod 为用户名和密码时，用于身份验证的非 EAP 方法。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|String|将 EAP 类型配置为 EAP - TTLS、EAP - FAST 或 PEAP 时，启用标识隐私 (外部标识) 。 此属性使用输入的文本屏蔽用户名。 例如，如果使用“匿名”，则使用其真实用户名通过此Wi-Fi连接进行身份验证的每个用户将显示为“匿名”。|
|usernameFormatString|字符串|用于生成连接到 wifi 的用户名的用户名格式字符串|
|passwordFormatString|String|用于生成连接到 wifi 的密码的密码格式字符串|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户提供的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|rootCertificatesForServerValidation|[iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) 集合|将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时，服务器验证的受信任根证书。 如果提供此值，则无需提供 trustedServerCertificateNames，反之亦然。 该集合最多可包含 500 个元素。|
|identityCertificateForClientAuthentication|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|将 EAP 类型配置为 EAP-TLS、使用证书身份验证) 的 EAP-TTLS (或使用证书身份验证) 的 PEAP (时，用于客户端身份验证的标识证书。|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|用于身份验证的派生凭据的租户级别设置。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "disableMacAddressRandomization": true,
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "usernameFormatString": "String",
  "passwordFormatString": "String"
}
```




