---
title: macOSWiredNetworkConfiguration 资源类型
description: MacOS 有线网络配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c62bd24e18faa7c3aa12c75c0c0427ed1f3e7483
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290565"
---
# <a name="macoswirednetworkconfiguration-resource-type"></a>macOSWiredNetworkConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 有线网络配置文件。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSWiredNetworkConfigurations](../api/intune-deviceconfig-macoswirednetworkconfiguration-list.md)|[macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) 集合|列出 [macOSWiredNetworkConfiguration 对象的属性和](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) 关系。|
|[获取 macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-get.md)|[macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|读取 [macOSWiredNetworkConfiguration 对象的属性和](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) 关系。|
|[创建 macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-create.md)|[macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|创建新的 [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) 对象。|
|[删除 macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-delete.md)|无|删除 [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)。|
|[更新 macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-update.md)|[macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|更新 [macOSWiredNetworkConfiguration 对象](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) 的属性。|

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
|description|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|String|网络名称|
|networkInterface|[wiredNetworkInterface](../resources/intune-deviceconfig-wirednetworkinterface.md)|网络接口。 可取值为：`anyEthernet`、`firstActiveEthernet`、`secondActiveEthernet`、`thirdActiveEthernet`、`firstEthernet`、`secondEthernet` 或 `thirdEthernet`。|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|可扩展身份验证协议 (EAP) 。 指示在有线网络上设置的 EAP 协议类型。 可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` 或 `teap`。|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|当 EAP-FAST FAST为所选的 EAP 类型时，选择 EAP-FAST配置选项。 可能的值是：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。|
|trustedServerCertificateNames|字符串集合|将 EAP 类型配置为 EAP-TLS/TTLS/FAST PEAP 时受信任的服务器证书名称。 这是由受信任证书颁发机构颁发给 CA 证书颁发机构颁发的 (名) 。 如果提供此信息，可以在最终用户连接到此有线网络时绕过显示在最终用户设备上的动态信任对话框。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|当 EAP 类型配置为 PEAP 或 EAP-TTLS 时身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。|
|nonEapAuthenticationMethodForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|当 EAP 类型为 EAP-TTLS (Authentication 方法为用户名和密码) 时，用于身份验证的非 EAP 方法将包含内部标识。 可能的值是：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|enableOuterIdentityPrivacy|String|将 EAP 类型 (EAP 类型) EAP-TTLS、EAP-FAST PEAP 时，启用标识隐私和外部标识。 此属性会屏蔽输入文本的用户名。 例如，如果使用"匿名"，则使用真实用户名对此有线网络进行身份验证的每个用户将显示为"匿名"。|

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
|rootCertificateForServerValidation|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|将 EAP 类型配置为 EAP-TLS/TTLS/FAST PEAP 时用于服务器验证的受信任根证书。|
|identityCertificateForClientAuthentication|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|将 EAP 类型配置为 EAP-TLS、EAP-TTLS (（具有证书身份验证) ）或 PEAP (证书身份验证时用于客户端身份验证的标识证书) 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSWiredNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
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
  "networkInterface": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "nonEapAuthenticationMethodForEapTtls": "String",
  "enableOuterIdentityPrivacy": "String"
}
```




