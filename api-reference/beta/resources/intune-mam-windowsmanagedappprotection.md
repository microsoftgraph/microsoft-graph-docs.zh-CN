---
title: windowsManagedAppProtection 资源类型
description: 用于配置针对特定安全组和Windows设备上的指定应用集的详细管理设置的策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d3116545d5d9bf8480f8c35dcd7ed7703739304
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858538"
---
# <a name="windowsmanagedappprotection-resource-type"></a>windowsManagedAppProtection 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于配置针对特定安全组和Windows设备上的指定应用集的详细管理设置的策略


继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsManagedAppProtections](../api/intune-mam-windowsmanagedappprotection-list.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) 集合|列出 [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) 对象的属性和关系。|
|[获取 windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-get.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|读取 [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) 对象的属性和关系。|
|[创建 windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-create.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|创建新的 [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) 对象。|
|[删除 windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-delete.md)|None|删除 [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)。|
|[更新 windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-update.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|更新 [windowsManagedAppProtection 对象的](../resources/intune-mam-windowsmanagedappprotection.md) 属性。|
|[targetApps 操作](../api/intune-mam-windowsmanagedappprotection-targetapps.md)|无|尚未记录|
|[分配操作](../api/intune-mam-windowsmanagedappprotection-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|String|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|isAssigned|Boolean|如果为 TRUE，则指示策略已部署到某些包含组。 如果为 FALSE，则指示策略未部署到任何包含组。 默认值为 FALSE。|
|deployedAppCount|Int32|指示为其部署当前策略的应用程序总数。|
|printBlocked|Boolean|如果为 TRUE，则指示从托管应用阻止打印。 如果为 FALSE，则指示允许从托管应用打印。 默认值为 FALSE。|
|allowedInboundDataTransferSources|[windowsManagedAppDataTransferLevel](../resources/intune-mam-windowsmanagedappdatatransferlevel.md)|指示允许从中传输数据的源。 某些可能的值为 allApps 或 none。 可取值为：`allApps`、`none`。|
|allowedOutboundClipboardSharingLevel|[windowsManagedAppClipboardSharingLevel](../resources/intune-mam-windowsmanagedappclipboardsharinglevel.md)|指示剪贴板可以跨组织&非组织资源共享到的级别。 一些可能的值是 anyDestinationAnySource 或无。 可取值为：`anyDestinationAnySource`、`none`。|
|allowedOutboundDataTransferDestinations|[windowsManagedAppDataTransferLevel](../resources/intune-mam-windowsmanagedappdatatransferlevel.md)|指示允许将数据传输到的目标。 某些可能的值为 allApps 或 none。 可取值为：`allApps`、`none`。|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果设置，它将指定在用户因身份验证令牌无效而无法签入的情况下要采取的操作。 当用户在 AAD 中被删除或禁用时，会发生这种情况。 一些可能的值是块或擦除。 如果未设置此属性，则不会执行任何操作。 可取值为：`block`、`wipe`、`warn`。|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|移动威胁防御应用报告的最大允许设备威胁级别。 可取值为：`notConfigured`、`secured`、`low`、`medium`、`high`。|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|确定如果未达到移动威胁防御威胁阈值，将执行哪些操作。 一些可能的值是块或擦除。 警告不是此属性支持的值。 可取值为：`block`、`wipe`、`warn`。|
|minimumRequiredSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 例如：“8.1.0”或“13.1.1”。|
|minimumWipeSdkVersion|String|低于指定版本的版本将擦除托管应用和关联的公司数据。 例如：“8.1.0”或“13.1.1”。|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 例如：“8.1.0”或“13.1.1”。|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 例如：“8.1.0”或“13.1.1”。|
|minimumWipeOsVersion|String|低于指定版本的版本将擦除托管应用和关联的公司数据。 例如：“8.1.0”或“13.1.1”。|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 例如：“8.1.0”或“13.1.1”。|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 例如：“8.1.0”或“13.1.1”。|
|minimumWipeAppVersion|String|低于指定版本的版本将擦除托管应用和关联的公司数据。 例如：“8.1.0”或“13.1.1”。|
|maximumRequiredOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。 例如：“8.1.0”或“13.1.1”。|
|maximumWarningOsVersion|String|大于指定版本的版本将导致托管应用收到来自访问公司数据的警告消息。 例如：“8.1.0”或“13.1.1”。|
|maximumWipeOsVersion|String|大于指定版本的版本将擦除托管应用和关联的公司数据。 例如：“8.1.0”或“13.1.1”。|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。 例如，P5D 指示间隔持续时间为 5 天。 时间跨度值 PT0S 表示当设备未连接到 Internet 时，将永远不会擦除托管数据。|
|periodOfflineBeforeAccessCheck|Duration|设备未连接到 Internet 时在该时间段后检查访问权限。 例如，PT5M 指示间隔持续时间为 5 分钟。 时间跨度值 PT0S 表示当设备未连接到 Internet 时，访问将立即被阻止。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合|策略部署到的包含组和排除组列表的导航属性。|
|apps|[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合|策略部署到的应用的列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "isAssigned": true,
  "deployedAppCount": 1024,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundClipboardSharingLevel": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "appActionIfUnableToAuthenticateUser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "minimumRequiredSdkVersion": "String",
  "minimumWipeSdkVersion": "String",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeAppVersion": "String",
  "maximumRequiredOsVersion": "String",
  "maximumWarningOsVersion": "String",
  "maximumWipeOsVersion": "String",
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "periodOfflineBeforeAccessCheck": "String (duration)"
}
```




