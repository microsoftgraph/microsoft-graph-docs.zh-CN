---
title: 创建 iosEasEmailProfileConfiguration
description: 创建新的 iosEasEmailProfileConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a09aa3f2680599869b1762c7d8712e40f7f9ae31
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339412"
---
# <a name="create-ioseasemailprofileconfiguration"></a>创建 iosEasEmailProfileConfiguration

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

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
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中, 提供 iosEasEmailProfileConfiguration 对象的 JSON 表示形式。

下表显示创建 iosEasEmailProfileConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|usernameSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|AAD 字段的名称, 将用于检索电子邮件配置文件的用户名。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`fullDomainName`、`netBiosDomainName`。|
|customDomainName|String|在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|帐户|String|帐户名称。|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|此电子邮件配置文件的身份验证方法。 可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。|
|blockMovingMessagesToOtherEmailAccounts|Boolean|指示是否阻止将邮件移动到其他电子邮件帐户。|
|blockSendingEmailFromThirdPartyApps|Boolean|指示是否阻止来自第三方应用的发送电子邮件。|
|blockSyncingRecentlyUsedEmailAddresses|Boolean|指示是否阻止同步最近使用的电子邮件地址, 例如, 撰写新电子邮件时。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|电子邮件的持续时间应同步回。 . 可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|hostName|String|本机邮件应用程序连接到的 Exchange 位置 (URL)。|
|requireSmime|Boolean|指示是否使用 S/MIME 证书。|
|smimeEnablePerMessageSwitch|Boolean|指示是否允许未加密的电子邮件。|
|smimeEncryptByDefaultEnabled|Boolean|如果设置为 "true S/MIME 加密", 则默认为启用。|
|smimeSigningEnabled|Boolean|如果为此帐户启用了设置为 true S/MIME 签名|
|smimeSigningUserOverrideEnabled|Boolean|如果设置为 true, 则用户可以打开或关闭 S/MIME 签名。|
|smimeEncryptByDefaultUserOverrideEnabled|Boolean|如果设置为 true, 则用户可以默认切换加密设置。|
|smimeSigningCertificateUserOverrideEnabled|Boolean|如果设置为 true, 则用户可以选择签名标识。|
|smimeEncryptionCertificateUserOverrideEnabled|Boolean|如果设置为 true, 则用户可以选择 S/MIME 加密标识。 |
|requireSsl|Boolean|指示是否使用 SSL。|
|useOAuth|Boolean|指定连接是否应使用 OAuth 进行身份验证。|
|signingCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|此电子邮件配置文件的签名证书类型。 可取值为：`none`、`certificate`、`derivedCredential`。|
|encryptionCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|此电子邮件配置文件的加密证书类型。 可取值为：`none`、`certificate`、`derivedCredential`。|



## <a name="response"></a>响应
如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2057

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2229

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```






