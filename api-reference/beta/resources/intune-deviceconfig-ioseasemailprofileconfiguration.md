---
title: iosEasEmailProfileConfiguration 资源类型
description: 通过提供此配置文件中的配置，您可以指示本机电子邮件客户端在 iOS 设备上的，与 Exchange server 通信和获取电子邮件、 联系人、 日历、 提醒和 notes。 此外，您还可以指定多少电子邮件到同步和设备应同步频率。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 220be246b359c353ff4bd2294000a7f43205106d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402158"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a>iosEasEmailProfileConfiguration 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过提供此配置文件中的配置，您可以指示本机电子邮件客户端在 iOS 设备上的，与 Exchange server 通信和获取电子邮件、 联系人、 日历、 提醒和 notes。 此外，您还可以指定多少电子邮件到同步和设备应同步频率。


继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 iosEasEmailProfileConfigurations](../api/intune-deviceconfig-ioseasemailprofileconfiguration-list.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)集合|列出属性和[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象之间的关系。|
|[获取 iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-get.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|读取属性和[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的关系。|
|[创建 iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-create.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|创建新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。|
|[删除 iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-delete.md)|无|删除[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)。|
|[更新 iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-update.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|更新[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
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
|usernameSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|AAD 字段，将用于检索用户名电子邮件配置文件的名称。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`fullDomainName`、`netBiosDomainName`。|
|customDomainName|String|在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|accountName|String|帐户名。|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|此电子邮件配置文件的身份验证方法。 可取值为：`usernameAndPassword`、`certificate`。|
|blockMovingMessagesToOtherEmailAccounts|Boolean|指示阻止移动到其他电子邮件帐户的消息。|
|blockSendingEmailFromThirdPartyApps|Boolean|指示阻止发送电子邮件从第三方应用程序。|
|blockSyncingRecentlyUsedEmailAddresses|Boolean|指示阻止同步最近使用的电子邮件地址，例如-撰写新电子邮件时。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|应返回到同步的时间电子邮件持续时间。 . 可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|hostName|String|Exchange 的 (URL) 的位置的本机邮件应用程序连接到。|
|requireSmime|Boolean|指示使用 S/MIME 证书。|
|smimeEnablePerMessageSwitch|Boolean|指示允许未加密的邮件。|
|smimeEncryptByDefaultEnabled|Boolean|如果设置为 true 的 S/MIME 加密默认情况下启用。|
|smimeSigningEnabled|Boolean|如果设置为 true 的 S/MIME 签名已启用此帐户|
|smimeSigningUserOverrideEnabled|Boolean|如果设置为 true，则用户可以切换 S/MIME 签名打开或关闭。|
|smimeEncryptByDefaultUserOverrideEnabled|Boolean|如果设置为 true，则用户可以切换默认设置的加密。|
|smimeSigningCertificateUserOverrideEnabled|Boolean|如果设置为 true，则用户可以选择的签名的标识。|
|smimeEncryptionCertificateUserOverrideEnabled|Boolean|如果设置为 true 用户可以选择的 S/MIME 加密标识。 |
|requireSsl|Boolean|指示使用 SSL。|
|useOAuth|Boolean|指定连接是否应使用 OAuth 进行身份验证。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|标识证书。|
|smimeSigningCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|S/MIME 签名证书。|
|smimeEncryptionCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|S/MIME 加密证书。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "authenticationMethod": "String",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true
}
```




