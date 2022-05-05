---
title: aospDeviceOwnerEnterpriseWiFiConfiguration 资源类型
description: 通过提供此配置文件中的配置，可以指示 AOSP 设备所有者设备连接到所需的Wi-Fi终结点。 通过指定Wi-Fi终结点所需的身份验证方法和安全类型，可以使最终用户的Wi-Fi连接无缝。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da1e031af52b8b19c8f6cbd6057998f9f716ca5c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203195"
---
# <a name="aospdeviceownerenterprisewificonfiguration-resource-type"></a>aospDeviceOwnerEnterpriseWiFiConfiguration 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过提供此配置文件中的配置，可以指示 AOSP 设备所有者设备连接到所需的Wi-Fi终结点。 通过指定Wi-Fi终结点所需的身份验证方法和安全类型，可以使最终用户的Wi-Fi连接无缝。


继承自 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 aospDeviceOwnerEnterpriseWiFiConfigurations](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-list.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) 集合|列出 [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) 对象的属性和关系。|
|[获取 aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-get.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|读取 [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) 对象的属性和关系。|
|[创建 aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-create.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|创建新的 [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) 对象。|
|[删除 aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-delete.md)|无|删除 [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)。|
|[更新 aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-update.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|更新 [aospDeviceOwnerEnterpriseWiFiConfiguration 对象的](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 如果此值为 false，并且作用域内用户不可见，则不允许分配到 ScopeTags 属性。 对于在 Silverlight 中创建的旧策略，可以通过在 Azure 门户中删除和重新创建策略来解决此问题。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的 OS 版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的 OS 版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|字符串|从 [aospDeviceOwnerWiFiConfiguration 继承的](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)网络名称|
|Ssid|字符串|这是向所有设备广播的Wi-Fi网络的名称。 继承自 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|connectAutomatically|Boolean|此网络在范围内时自动连接。 将此设置为 true 将跳过用户提示，并自动将设备连接到Wi-Fi网络。 继承自 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。 继承自 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|wiFiSecurityType|[aospDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-aospdeviceownerwifisecuritytype.md)|指示Wi-Fi终结点是否使用基于 EAP 的安全类型。 继承自 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)。 可能的值是：`open`、`wep`、`wpaPersonal`、`wpaEnterprise`。|
|preSharedKey|String|这是 WPA 个人Wi-Fi网络的预共享密钥。 继承自 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|preSharedKeyIsSet|Boolean|这是 WPA 个人Wi-Fi网络的预共享密钥。 继承自 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|指示在路由器)  (Wi-Fi终结点上设置的 EAP 协议的类型。 可取值为：`eapTls`、`eapTtls`、`peap`。|
|trustedServerCertificateNames|String collection|将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时，受信任的服务器证书名称。 这是受信任证书颁发机构 (CA) 颁发的证书中使用的常见名称。 如果提供此信息，则可以在最终用户连接到此Wi-Fi网络时绕过在最终用户设备上显示的动态信任对话框。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|指示客户端 (设备) 配置为 PEAP 或 EAP-TTLS 时需要使用的身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|当 EAP 类型为 EAP-TTLS 且 Authenticationmethod 为用户名和密码时，用于身份验证的非 EAP 方法 (内部标识) 。 可能的值是：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时，用于身份验证的非 EAP 方法 (内部标识) 。 该集合最多可包含 500 个元素。 可取值为：`none`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|String|将 EAP 类型配置为 EAP-TTLS 或 PEAP 时，启用标识隐私 (外部标识) 。 此处提供的字符串用于在单个用户尝试连接到Wi-Fi网络时屏蔽用户名。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户提供的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|rootCertificateForServerValidation|[aospDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-aospdeviceownertrustedrootcertificate.md)|将 EAP 类型配置为 EAP-TLS、EAP-TTLS 或 PEAP 时，服务器验证的受信任根证书。 这是设备尝试连接到Wi-Fi终结点时，Wi-Fi终结点提供的证书。 设备 (或用户) 必须接受此证书才能继续连接尝试。|
|identityCertificateForClientAuthentication|[aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)|将 EAP 类型配置为 EAP-TLS、使用证书身份验证) 的 EAP-TTLS (或使用证书身份验证) 的 PEAP (时，用于客户端身份验证的标识证书。 这是客户端向Wi-Fi终结点提供的证书。 位于Wi-Fi终结点后面的身份验证服务器必须接受此证书才能成功建立Wi-Fi连接。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aospDeviceOwnerEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerEnterpriseWiFiConfiguration",
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
  "preSharedKey": "String",
  "preSharedKeyIsSet": true,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```




