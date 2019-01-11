---
title: windowsIdentityProtectionConfiguration 资源类型
description: 此实体提供了属性、 由 Windows Hello for Business 公开的关系的声明方法的说明。
localization_priority: Normal
ms.openlocfilehash: c83a87737db6deacf7a08cc0fb4a73aff6d4f781
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823399"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>windowsIdentityProtectionConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

此实体提供了属性、 由 Windows Hello for Business 公开的关系的声明方法的说明。

继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 windowsIdentityProtectionConfigurations](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)集合|列出属性和[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象之间的关系。|
|[获取 windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|读取属性和[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象的关系。|
|[创建 windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|创建新的[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象。|
|[删除 windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|无|删除[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)。|
|[更新 windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|更新[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象的属性。|

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
|enhancedAntiSpoofingForFacialFeaturesEnabled|布尔|用于启用增强反欺骗 Windows Hello 图符身份验证的面部功能识别的布尔值。|
|pinMinimumLength|Int32|设置的最小所需的 Windows Hello 业务 PIN 的字符数的整数值。 有效值为 4 到 127 之间，因此小于或等于的值的最大 PIN 设置。 有效值 4 到 127|
|pinMaximumLength|Int32|设置的最大允许工作 PIN 的字符数的整数值。 有效值为 4 到 127 非独占且大于或等于最小 PIN 设置的值。 有效值 4 到 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|此值将使用大写字符中 Windows Hello 配置的业务 PIN。 可取值为：`blocked`、`required`、`allowed`。|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|此值为业务 PIN 在 Windows Hello 配置使用小写字符。 可取值为：`blocked`、`required`、`allowed`。|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|控制能否使用特殊字符中 Windows Hello 业务 PIN。 可取值为：`blocked`、`required`、`allowed`。|
|pinExpirationInDays|Int32|整数值，指定的时间段 （以天为单位） 的系统要求用户更改其之前，可以使用 PIN。 有效值为 0 到 730 之间。 有效值为 0 至 730|
|pinPreviousBlockCount|Int32|控制能否阻止用户使用过旋转中心点。 这必须介于 0 到 50，含之间设置和用户的当前 PIN，包含在该计数。 如果设置为 0，以前 Pin 不会存储。 PIN 历史记录不保留通过 PIN 重置。 有效值为 0 至 50|
|pinRecoveryEnabled|布尔|布尔值，使用户能够通过使用 Windows Hello 业务 PIN 恢复服务更改其 PIN。|
|securityDeviceRequired|Boolean|控制是否用于设置 Windows Hello 的业务要求受信任平台模块 (TPM)。 TPM 提供其他安全的优势，不能在其他设备上使用存储在其上的数据。 如果设置为 False，所有设备可以都设置 Windows Hello for Business 即使没有可用 TPM。|
|unlockWithBiometricsEnabled|Boolean|控制生物手势，如图符和指纹，用作的替代方法 Windows Hello 的业务 PIN。  如果不允许设置为 False，生物手势。 用户仍必须作为出现故障时备份配置 PIN。|
|useCertificatesForOnPremisesAuthEnabled|布尔|启用 Windows Hello for Business 使用证书进行身份验证的本地资源的布尔值。|
|windowsHelloForBusinessBlocked|Boolean|阻止 Windows Hello for Business 作为用于登录到 Windows 方法的布尔值。|

## <a name="relationships"></a>Relationships
|关系|类型|Description|
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
  "@odata.type": "microsoft.graph.windowsIdentityProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
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
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "pinExpirationInDays": 1024,
  "pinPreviousBlockCount": 1024,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





