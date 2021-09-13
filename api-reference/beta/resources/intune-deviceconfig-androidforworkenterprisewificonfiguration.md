---
title: androidForWorkEnterpriseWiFiConfiguration 资源类型
description: 通过在此配置文件中提供配置，你可以指示 Android for Work 设备连接到所需的 Wi-Fi 终结点。 通过指定终结点预期的身份验证Wi-Fi，可以使最终用户Wi-Fi无缝连接。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f24afc5ad1ff2b87416606545b9906ee96dd989
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106467"
---
# <a name="androidforworkenterprisewificonfiguration-resource-type"></a>androidForWorkEnterpriseWiFiConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过在此配置文件中提供配置，你可以指示 Android for Work 设备连接到所需的 Wi-Fi 终结点。 通过指定终结点预期的身份验证Wi-Fi，可以使最终用户Wi-Fi无缝连接。


继承自 [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidForWorkEnterpriseWiFiConfigurations](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-list.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) 集合|列出 [androidForWorkEnterpriseWiFiConfiguration 对象的属性和](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) 关系。|
|[获取 androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-get.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)|读取 [androidForWorkEnterpriseWiFiConfiguration 对象的属性和](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) 关系。|
|[创建 androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-create.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)|创建新的 [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) 对象。|
|[删除 androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-delete.md)|无|删除 [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)。|
|[更新 androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-update.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)|更新 [androidForWorkEnterpriseWiFiConfiguration 对象](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) 的属性。|

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
|networkName|String|网络名称 继承自 [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|ssid|String|这是广播到所有Wi-Fi网络的名称。 继承自 [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|connectAutomatically|Boolean|连接网络在范围内时自动运行。 如果设置为 true，将跳过用户提示，并自动将设备Wi-Fi网络。 继承自 [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。 继承自 [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|wiFiSecurityType|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|指示Wi-Fi是否使用基于 EAP 的安全类型。 继承自 [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)。 可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|指示在 Wi-Fi (路由器上设置的 EAP (类型) 。 可取值为：`eapTls`、`eapTtls`、`peap`。|
|trustedServerCertificateNames|字符串集合|将 EAP 类型配置为 EAP-TLS/TTLS/FAST PEAP 时受信任的服务器证书名称。 这是由受信任证书颁发机构颁发给 CA 证书颁发机构颁发的证书 (名) 。 如果提供此信息，则当最终用户连接到此网络时，可以绕过在最终用户设备上显示的动态信任Wi-Fi对话框。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|指示当 EAP 类型 (EAP) EAP-TTLS 时，需要使用的客户端身份验证方法。 可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|当 EAP 类型为 EAP-TTLS) Authentication 方法为 Username 和 Password 时，用于身份验证的非 EAP (内部标识方法。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|当 EAP 类型为 PEAP (Authentication 方法为 Username 和 Password) 时，用于身份验证的非 EAP 方法将包含内部标识。 可取值为：`none`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|String|将 EAP (EAP 类型) EAP-TTLS 或 PEAP 时，启用标识隐私和外部标识。 此处提供的字符串用于在用户尝试连接到网络时屏蔽Wi-Fi用户名。|

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
|rootCertificateForServerValidation|[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)|将 EAP 类型配置为 EAP-TLS、EAP-TTLS 或 PEAP 时用于服务器验证的受信任的根证书。 这是设备尝试连接到 Wi-Fi 终结点时，Wi-Fi证书。 设备或 (用户) 必须接受此证书，以继续尝试连接。|
|identityCertificateForClientAuthentication|[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|当 EAP 类型配置为 EAP-TLS、EAP-TTLS (（具有证书身份验证) ）或 PEAP (证书身份验证) 时，用于客户端身份验证的标识证书。 这是客户端向 Wi-Fi 证书。 安全终结点后面的身份验证Wi-Fi必须接受此证书，以成功建立Wi-Fi连接。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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



