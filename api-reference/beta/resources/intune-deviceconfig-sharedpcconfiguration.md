---
title: sharedPCConfiguration 资源类型
description: 本主题提供由 sharedPCConfiguration 资源公开的已声明方法、属性和关系的说明。
ms.openlocfilehash: fec817184ed5027904b4afebcf867f45b2ac7808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043110"
---
# <a name="sharedpcconfiguration-resource-type"></a>sharedPCConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

本主题提供由 sharedPCConfiguration 资源公开的已声明方法、属性和关系的说明。

继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List sharedPCConfigurations](../api/intune-deviceconfig-sharedpcconfiguration-list.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 集合|列出 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的属性和关系。|
|[Get sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-get.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|读取 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的属性和关系。|
|[Create sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-create.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|创建新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。|
|[Delete sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-delete.md)|无|删除 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)。|
|[Update sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-update.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|更新 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的属性。|

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
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|指定在共享电脑上管理帐户的方式。 仅当 disableAccountManager 为 false 时适用。|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|指示允许在共享电脑上使用哪种类型的帐户。 可取值为：`guest`、`domain`。|
|localStorage|[启用](../resources/intune-shared-enablement.md)|指定在共享电脑上是否允许本地存储。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|allowLocalStorage|Boolean|指定在共享电脑上是否允许本地存储。|
|setAccountManager|[启用](../resources/intune-shared-enablement.md)|禁用共享电脑模式的帐户管理器。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|disableAccountManager|Boolean|禁用共享电脑模式的帐户管理器。|
|setEduPolicies|[启用](../resources/intune-shared-enablement.md)|指定是否默认共享 PC 教育环境策略应启用/禁用/不配置。 对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|disableEduPolicies|Boolean|指定是否应禁用默认的共享电脑教育环境策略。 对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。|
|setPowerPolicies|[启用](../resources/intune-shared-enablement.md)|指定是否默认共享 PC 电源策略应启用/禁用。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|disablePowerPolicies|Boolean|指定是否应禁用默认的共享电脑电源策略。|
|signInOnResume|[启用](../resources/intune-shared-enablement.md)|指定签名的要求中次设备从唤醒休眠模式。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|disableSignInOnResume|Boolean|禁用每当设备从睡眠模式唤醒时需要登录的要求。|
|enabled|Boolean|启用共享的电脑模式并应用共享的电脑策略。|
|idleTimeBeforeSleepInSeconds|Int32|指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。 将此值设置为 0 可防止发生睡眠超时。|
|kioskAppDisplayName|String|指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。 仅在设置 KioskAppUserModelId 后适用。|
|kioskAppUserModelId|String|指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。|
|maintenanceStartTime|TimeOfDay|指定维护小时的每日开始时间。|

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

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "localStorage": "String",
  "allowLocalStorage": true,
  "setAccountManager": "String",
  "disableAccountManager": true,
  "setEduPolicies": "String",
  "disableEduPolicies": true,
  "setPowerPolicies": "String",
  "disablePowerPolicies": true,
  "signInOnResume": "String",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```





