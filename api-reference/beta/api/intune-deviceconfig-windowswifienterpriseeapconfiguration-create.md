---
title: 创建 windowsWifiEnterpriseEAPConfiguration
description: 创建新的 windowsWifiEnterpriseEAPConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f3ab25f8d74546bd75d4fdc65cc5306fd4c48d25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413477"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a>创建 windowsWifiEnterpriseEAPConfiguration

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 windowsWifiEnterpriseEAPConfiguration 对象的 JSON 表示形式。

下表显示时创建 windowsWifiEnterpriseEAPConfiguration 所需的属性。

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



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




