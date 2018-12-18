---
title: 创建 iosEnterpriseWiFiConfiguration
description: 创建新的 iosEnterpriseWiFiConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 2e11b506df4fde586aa181602e25da4c499ab6bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320697"
---
# <a name="create-iosenterprisewificonfiguration"></a>创建 iosEnterpriseWiFiConfiguration

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


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
|授权|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 iosEnterpriseWiFiConfiguration 对象的 JSON 表示形式。

下表显示时创建 iosEnterpriseWiFiConfiguration 所需的属性。

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
|networkName|字符串|网络名称继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|ssid|字符串|这是广播到所有设备 Wi-fi 网络的名称。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectAutomatically|Boolean|自动连接此网络何时范围中。 将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|网络未进行广播其名称 (SSID) 连接。 当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|指示是否 Wi-fi 终结点使用 EAP 基于安全类型。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。 可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|代理类型从[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)此 Wi-fi 连接继承的。 可取值为：`none`、`manual`、`automatic`。|
|proxyManualAddress|字符串|选择手动配置时，代理服务器的 IP 地址或 DNS 主机名。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyManualPort|Int32|选择手动配置时的代理服务器的端口。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|字符串|代理服务器自动配置脚本时选择了自动配置的 URL。 此 URL 通常是 PAC （代理自动配置） 文件的位置。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|preSharedKey|字符串|这是预共享的 WPA 个人 Wi-fi 网络密钥。 继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|可扩展的身份验证协议 (EAP)。 指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。 可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|EAP FAST 配置选项时 EAP FAST 是所选的 EAP 类型。 可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。|
|trustedServerCertificateNames|String 集合|当 EAP 类型配置为 EAP-TLS/TTL/FAST 或 PEAP 受信任服务器证书名称。 这是您的受信任的证书颁发机构 (CA) 颁发的证书中使用的通用名称。 如果您提供此信息，您可以跳过它们连接到此 Wi-fi 网络时，最终用户的设备显示动态信任对话框。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|当 EAP 类型配置为 PEAP 或 EAP TTL 身份验证方法。 可取值为：`certificate`、`usernameAndPassword`。|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|用于身份验证 EAP TTL 并 Authenticationmethod EAP 类型时的非 EAP 方法是用户名和密码。 可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。|
|outerIdentityPrivacyTemporaryValue|字符串|时 EAP 类型配置为 EAP-TTL，EAP-启用标识隐私 （外部标识） FAST 或 PEAP。 此属性将屏蔽用户名与您输入的文本。 例如，如果您使用匿名，每个与使用其实际用户名此 Wi-fi 连接进行身份验证的用户显示为匿名。|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





