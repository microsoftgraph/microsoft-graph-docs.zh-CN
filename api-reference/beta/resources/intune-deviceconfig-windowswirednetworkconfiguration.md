---
title: windowsWiredNetworkConfiguration 资源类型
description: 此实体提供有线网络 CSP 公开的已声明方法、属性和关系的说明。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0f557826cac1a923324c817d5b30a4f06b9edad
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631026"
---
# <a name="windowswirednetworkconfiguration-resource-type"></a>windowsWiredNetworkConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体提供有线网络 CSP 公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsWiredNetworkConfigurations](../api/intune-deviceconfig-windowswirednetworkconfiguration-list.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) 集合|列出 [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) 对象的属性和关系。|
|[获取 windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-get.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|读取 [windowsWiredNetworkConfiguration 对象的属性和](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) 关系。|
|[创建 windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-create.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|创建新的 [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) 对象。|
|[删除 windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-delete.md)|无|删除 [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)。|
|[更新 windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-update.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|更新 [windowsWiredNetworkConfiguration 对象](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) 的属性。|

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
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|authenticationType|[wiredNetworkAuthenticationType](../resources/intune-deviceconfig-wirednetworkauthenticationtype.md)|指定是对用户、设备进行身份验证，还是使用来宾身份验证， (身份验证) 。 如果使用证书身份验证，请确保证书类型与身份验证类型匹配。 可取值为：`none`、`user`、`machine`、`machineOrUser`、`guest`。 可取值为：`none`、`user`、`machine`、`machineOrUser`、`guest`、`unknownFutureValue`。|
|cacheCredentials|Boolean|如果为 TRUE，则缓存设备中的用户凭据，以便用户无需每次连接时都一直输入凭据。 如果为 FALSE，请不要缓存凭据。 默认值为 FALSE。|
|authenticationPeriodInSeconds|Int32|指定客户端在身份验证尝试失败之前等待的秒数。 有效范围为 1-3600。|
|authenticationRetryDelayPeriodInSeconds|Int32|指定失败的身份验证和下一次身份验证尝试之间的秒数。 有效范围为 1-3600。|
|eapolStartPeriodInSeconds|Int32|指定在"开始"消息中通过 LAN 发送 EAPOL (可扩展身份验证协议) 秒数。 有效范围为 1-3600。|
|maximumEAPOLStartMessages|Int32|指定通过 LAN 的 EAPOL (可扩展身份验证协议的最大) 在返回失败之前发送的"开始"消息。 有效范围为 1-100。|
|maximumAuthenticationFailures|Int32|指定一组凭据允许的最大身份验证失败数。 有效范围为 1-100。|
|enforce8021X|Boolean|如果为 TRUE，有线网络的自动配置服务需要使用 802.1X 进行端口身份验证。 如果为 FALSE，则不需要 802.1X。 默认值为 FALSE。|
|authenticationBlockPeriodInMinutes|Int32|指定在身份验证尝试失败后阻止自动身份验证尝试的持续时间。|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|可扩展身份验证协议 (EAP) 。 指示在 Wi-Fi 路由器 (上设置的 EAP) 。 可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` 或 `teap`。 可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` 或 `teap`。|
|trustedServerCertificateNames|String 集合|指定受信任的服务器证书名称。|
|authenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|指定身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。 可能的值是：`certificate`、`usernameAndPassword`、`derivedCredential`、`unknownFutureValue`。|
|secondaryAuthenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|指定辅助身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。 可能的值是：`certificate`、`usernameAndPassword`、`derivedCredential`、`unknownFutureValue`。|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|为 EAP TTLS 指定内部身份验证协议。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|String|使用 EAP TTLS 或 PEAP 时，指定用于替换隐私用户名的字符串。|
|performServerValidation|Boolean|如果为 TRUE，则当选择 EAP 类型为 PEAP 时，通过验证证书来验证服务器的身份。 如果为 FALSE，则不验证证书。 默认值为 TRUE。|
|disableUserPromptForServerValidation|Boolean|如果为 TRUE，则当选择 EAP 类型为 PEAP 时，阻止提示用户为受信任的证书颁发机构授权新服务器。 如果为 FALSE，则不阻止提示用户。 默认值为 FALSE。|
|requireCryptographicBinding|Boolean|如果为 TRUE，则当选择 EAP 类型作为 PEAP 时启用加密绑定。 如果为 FALSE，则不启用加密绑定。 默认值为 TRUE。|
|forceFIPSCompliance|Boolean|如果为 TRUE，则强制 FIPS 合规性。 如果为 FALSE，则不启用 FIPS 合规性。 默认值为 FALSE。|

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
|rootCertificatesForServerValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 集合|指定用于服务器验证的根证书。 该集合最多可包含 500 个元素。|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|指定客户端身份验证的标识证书。|
|secondaryIdentityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|指定客户端身份验证的辅助标识证书。|
|rootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|指定用于客户端验证的根证书。|
|secondaryRootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|指定用于客户端验证的辅助根证书。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWiredNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWiredNetworkConfiguration",
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
  "authenticationType": "String",
  "cacheCredentials": true,
  "authenticationPeriodInSeconds": 1024,
  "authenticationRetryDelayPeriodInSeconds": 1024,
  "eapolStartPeriodInSeconds": 1024,
  "maximumEAPOLStartMessages": 1024,
  "maximumAuthenticationFailures": 1024,
  "enforce8021X": true,
  "authenticationBlockPeriodInMinutes": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "secondaryAuthenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "requireCryptographicBinding": true,
  "forceFIPSCompliance": true
}
```




