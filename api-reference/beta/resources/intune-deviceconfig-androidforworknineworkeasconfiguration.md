---
title: androidForWorkNineWorkEasConfiguration 资源类型
description: 通过提供此配置文件中的配置，您可以指示九工作电子邮件客户端上的工作 Android 设备与 Exchange server 通信和获取电子邮件、 联系人、 日历、 任务和注释。 此外，您还可以指定多少电子邮件到同步和设备应同步频率。
ms.openlocfilehash: 6829e6a20b87b56937f0b646ee70c986747da5a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043585"
---
# <a name="androidforworknineworkeasconfiguration-resource-type"></a>androidForWorkNineWorkEasConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

通过提供此配置文件中的配置，您可以指示九工作电子邮件客户端上的工作 Android 设备与 Exchange server 通信和获取电子邮件、 联系人、 日历、 任务和注释。 此外，您还可以指定多少电子邮件到同步和设备应同步频率。

继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 androidForWorkNineWorkEasConfigurations](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-list.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)集合|列出属性和[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)对象之间的关系。|
|[获取 androidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-get.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|读取属性和[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)对象的关系。|
|[创建 androidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-create.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|创建新的[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)对象。|
|[删除 androidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-delete.md)|无|删除[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)。|
|[更新 androidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-update.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|更新[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)对象的属性。|

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
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Exchange ActiveSync 的身份验证方法。 继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。 可取值为：`usernameAndPassword`、`certificate`。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|应为同步的时间电子邮件持续时间。 继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。 可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。 继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。 可取值为：`userPrincipalName`、`primarySmtpAddress`。|
|hostName|String|Exchange 位置 (URL) 的邮件应用程序连接到。 继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|
|requireSsl|布尔|指示使用 SSL。 继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。 继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。 可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。|
|syncCalendar|布尔|同步日历的切换。 如果设置为 false 日历已在设备上关闭。|
|syncContacts|布尔|切换同步联系人。 如果设置为 false 的联系人设备上关闭。|
|syncTasks|布尔|同步任务的切换。 如果设置为 false 的任务在设备上关闭。|

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
|identityCertificate|[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|标识证书。 继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkNineWorkEasConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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
  "authenticationMethod": "String",
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSsl": true,
  "usernameSource": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```





