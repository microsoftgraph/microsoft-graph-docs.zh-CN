---
title: 创建 androidEasEmailProfileConfiguration
description: 创建新的 androidEasEmailProfileConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b59a1e551aaad0e4ad23c1001ca3fea515333ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817778"
---
# <a name="create-androideasemailprofileconfiguration"></a>创建 androidEasEmailProfileConfiguration

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。
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
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 androidEasEmailProfileConfiguration 对象的 JSON 表示形式。

下表显示时创建 androidEasEmailProfileConfiguration 所需的属性。

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
|accountName|字符串|Exchange ActiveSync 帐户名，向用户显示为 EAS (this) 配置文件的名称。|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Exchange ActiveSync 的身份验证方法。 可取值为：`usernameAndPassword`、`certificate`。|
|syncCalendar|布尔|同步日历的切换。 如果设置为 false 的日历已在设备上关闭。|
|syncContacts|布尔|切换同步联系人。 如果设置为 false 的联系人设备上关闭。|
|syncTasks|布尔|同步任务的切换。 如果设置为 false 的任务在设备上关闭。|
|syncNotes|布尔|同步注释的切换。 如果设置为 false 的说明在设备上关闭。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|应为同步的时间电子邮件持续时间。 可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|emailSyncSchedule|[emailSyncSchedule](../resources/intune-deviceconfig-emailsyncschedule.md)|电子邮件的同步计划。 可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage`。|
|hostName|String|Exchange 位置 (URL) 的本机邮件应用程序连接到。|
|requireSmime|布尔|指示使用 S/MIME 证书。|
|requireSsl|布尔|指示使用 SSL。|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。 可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。 可取值为：`fullDomainName`、`netBiosDomainName`。|
|customDomainName|字符串|在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 857

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 965

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```





