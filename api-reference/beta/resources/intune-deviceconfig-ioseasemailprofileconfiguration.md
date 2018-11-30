---
title: iosEasEmailProfileConfiguration 资源类型
description: 通过提供此配置文件中的配置，您可以指示本机电子邮件客户端在 iOS 设备上的，与 Exchange server 通信和获取电子邮件、 联系人、 日历、 提醒和 notes。 此外，您还可以指定多少电子邮件到同步和设备应同步频率。
ms.openlocfilehash: 4ce93ed8963a6ee82775adbfc8edd14a15b4188d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042802"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a>iosEasEmailProfileConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|supportsScopeTags|布尔|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|usernameSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|AAD 字段，将用于检索用户名电子邮件配置文件的名称。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。 可取值为：`fullDomainName`、`netBiosDomainName`。|
|customDomainName|字符串|在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。 继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|accountName|字符串|帐户名。|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|此电子邮件配置文件的身份验证方法。 可取值为：`usernameAndPassword`、`certificate`。|
|blockMovingMessagesToOtherEmailAccounts|布尔|指示阻止移动到其他电子邮件帐户的消息。|
|blockSendingEmailFromThirdPartyApps|布尔|指示阻止发送电子邮件从第三方应用程序。|
|blockSyncingRecentlyUsedEmailAddresses|布尔|指示阻止同步最近使用的电子邮件地址，例如-撰写新电子邮件时。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|应返回到同步的时间电子邮件持续时间。 . 可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|hostName|String|Exchange 的 (URL) 的位置的本机邮件应用程序连接到。|
|requireSmime|布尔|指示使用 S/MIME 证书。|
|smimeEnablePerMessageSwitch|布尔|指示允许未加密的邮件。|
|requireSsl|布尔|指示使用 SSL。|
|useOAuth|布尔|指定连接是否应使用 OAuth 进行身份验证。|

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
  "requireSsl": true,
  "useOAuth": true
}
```





