---
title: androidEnterpriseWiFiConfiguration 资源类型
description: 通过提供此配置文件中的配置, 可以指示 Android 设备连接到所需的 wlan 终结点。 通过指定 wi-fi 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 wi-fi 连接。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2cd44e7a0f855477dbc945ee9f3260c0d0d08da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783190"
---
# <a name="androidenterprisewificonfiguration-resource-type"></a>androidEnterpriseWiFiConfiguration 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过提供此配置文件中的配置, 可以指示 Android 设备连接到所需的 wlan 终结点。 通过指定 wi-fi 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 wi-fi 连接。


继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidEnterpriseWiFiConfigurations](../api/intune-deviceconfig-androidenterprisewificonfiguration-list.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)集合|列出[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象的属性和关系。|
|[获取 androidEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidenterprisewificonfiguration-get.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)|读取[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象的属性和关系。|
|[创建 androidEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidenterprisewificonfiguration-create.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)|创建新的[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象。|
|[删除 androidEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidenterprisewificonfiguration-delete.md)|无|删除[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)。|
|[更新 androidEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidenterprisewificonfiguration-update.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)|更新[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔值|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|networkName|String|从[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)继承的网络名称|
|ssid|String|这是广播到所有设备的 wi-fi 网络的名称。 继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)|
|connectAutomatically|布尔值|当此网络在范围内时自动连接。 将此设置为 true 将跳过用户提示, 并自动将设备连接到 wlan 网络。 继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|布尔值|当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。 继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)|
|wiFiSecurityType|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|指示 wi-fi 终结点是否使用基于 EAP 的安全类型。 继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)。 可取值为：`open`、`wpaEnterprise`。|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|指示在 wlan 终结点 (路由器) 上设置的 EAP 协议的类型。 可取值为：`eapTls`、`eapTtls`、`peap`。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时, 客户端 (设备) 需要使用的身份验证方法。 可取值为：`certificate`、`usernameAndPassword`。|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|eap 类型为 eap 时, 用于身份验证的非 EAP 方法 (内部标识)-TTLS 和 Authenticationmethod 为用户名和密码。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时, 用于身份验证的非 EAP 方法 (内部标识)。 可取值为：`none`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|String|将 eap 类型配置为 eap-TTLS 或 PEAP 时启用标识隐私 (外部标识)。 此处提供的字符串用于在用户尝试连接到 wlan 网络时屏蔽各个用户的用户名。|

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
|rootCertificateForServerValidation|[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|将 eap 类型配置为 eap-tls、eap-TTLS 或 PEAP 时用于服务器验证的受信任根证书。 这是在设备尝试连接到 wlan 终结点时由 wi-fi 终结点提供的证书。 设备 (或用户) 必须接受此证书才能继续尝试连接。|
|identityCertificateForClientAuthentication|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|将 eap 类型配置为 eap-tls、eap-TTLS (使用证书身份验证) 或 PEAP (使用证书身份验证) 时, 客户端身份验证的标识证书。 这是客户端向 wi-fi 终结点出示的证书。 wi-fi 终结点后面的身份验证服务器必须接受此证书才能成功建立 wlan 连接。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
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
  "eapType": "String",
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





