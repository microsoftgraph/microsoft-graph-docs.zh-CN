---
title: macOSEnterpriseWiFiConfiguration 资源类型
description: MacOS Wi-fi WPA-企业/WPA2-企业配置配置文件。
ms.openlocfilehash: fd1cbc5b3fd657f86f95a092f8e8cb71f660e5b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042054"
---
# <a name="macosenterprisewificonfiguration-resource-type"></a>macOSEnterpriseWiFiConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

MacOS Wi-fi WPA-企业/WPA2-企业配置配置文件。

继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 macOSEnterpriseWiFiConfigurations](../api/intune-deviceconfig-macosenterprisewificonfiguration-list.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)集合|列出属性和[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象之间的关系。|
|[获取 macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-get.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|读取属性和[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象的关系。|
|[创建 macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-create.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|创建新的[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象。|
|[删除 macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-delete.md)|无|删除[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)。|
|[更新 macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-update.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|更新[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)对象的属性。|

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
|networkName|字符串|网络名称继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|ssid|字符串|这是广播到所有设备 Wi-fi 网络的名称。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectAutomatically|布尔|自动连接此网络何时范围中。 将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|布尔|网络未进行广播其名称 (SSID) 连接。 当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|指示是否 Wi-fi 终结点使用 EAP 基于安全类型。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)。 可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|代理类型从[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)此 Wi-fi 连接继承的。 可取值为：`none`、`manual`、`automatic`。|
|proxyManualAddress|字符串|选择手动配置时，代理服务器的 IP 地址或 DNS 主机名。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyManualPort|Int32|选择手动配置时的代理服务器的端口。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|字符串|代理服务器自动配置脚本时选择了自动配置的 URL。 此 URL 通常是 PAC （代理自动配置） 文件的位置。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|preSharedKey|字符串|这是预共享的 WPA 个人 Wi-fi 网络密钥。 继承自[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|可扩展的身份验证协议 (EAP)。 指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。 可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|EAP FAST 配置选项时 EAP FAST 是所选的 EAP 类型。 可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。|
|trustedServerCertificateNames|String 集合|当 EAP 类型配置为 EAP-TLS/TTL/FAST 或 PEAP 受信任服务器证书名称。 这是您的受信任的证书颁发机构 (CA) 颁发的证书中使用的通用名称。 如果您提供此信息，您可以跳过它们连接到此 Wi-fi 网络时，最终用户设备显示动态信任对话框。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|当 EAP 类型配置为 PEAP 或 EAP TTL 身份验证方法。 可取值为：`certificate`、`usernameAndPassword`。|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|身份验证 （内部标识） EAP 类型时 EAP TTL 和 Authenticationmethod 非 EAP 方法是用户名和密码。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|字符串|到 EAP TTL、 EAP FAST 或 PEAP 配置 EAP 类型时启用标识隐私 （外部标识）。 此属性将屏蔽用户名与您输入的文本。 例如，如果您使用匿名，每个与使用其实际用户名此 Wi-fi 连接进行身份验证的用户显示为匿名。|

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
|rootCertificateForServerValidation|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|受信任的根证书服务器验证 EAP 类型配置到 EAP-TLS/TTL/FAST 或 PEAP 时。|
|identityCertificateForClientAuthentication|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|客户端身份验证时 EAP 类型配置为 EAP TLS、 EAP-TTL （使用证书身份验证） 或 PEAP （使用证书身份验证） 的标识证书。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





