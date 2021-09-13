---
title: iosManagedAppProtection 资源类型
description: 用于配置针对特定安全组和 iOS 设备上指定的一组应用的详细管理设置的策略
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b55a28e6be1a9383d7384649e142ac793467c685
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113670"
---
# <a name="iosmanagedappprotection-resource-type"></a>iosManagedAppProtection 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于配置针对特定安全组和 iOS 设备上指定的一组应用的详细管理设置的策略


继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List iosManagedAppProtections](../api/intune-mam-iosmanagedappprotection-list.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 集合|列出 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的属性和关系。|
|[Get iosManagedAppProtection](../api/intune-mam-iosmanagedappprotection-get.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|读取 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的属性和关系。|
|[Create iosManagedAppProtection](../api/intune-mam-iosmanagedappprotection-create.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|创建新的 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象。|
|[Delete iosManagedAppProtection](../api/intune-mam-iosmanagedappprotection-delete.md)|无|删除 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)。|
|[Update iosManagedAppProtection](../api/intune-mam-iosmanagedappprotection-update.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|更新 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|说明|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|String|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|设备未连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration|设备连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许传输其中的数据的源。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedApps`、`none`。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许向其传输数据的目标。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedApps`、`none`。|
|organizationalCredentialsRequired|Boolean|指示是否需要组织凭据才能使用应用。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|可以在托管设备上的应用之间共享剪贴板的级别。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。|
|dataBackupBlocked|Boolean|指示是否阻止备份托管应用的数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|deviceComplianceRequired|Boolean|指示是否需要设备符合性。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|指示是应在托管浏览器应用中打开 Internet 链接，还是应在由 CustomBrowserProtocol (for iOS) 或 CustomBrowserPackageId/CustomBrowserDisplayName (for Android) 指定的任何自定义浏览器继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|指示是否需要应用级 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|阻止或擦除托管应用之前的最大错误引脚重试次数。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 PIN 的字符集。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合|用户可能存储托管数据的数据存储位置。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 PIN，是否需要使用应用 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|指示应在哪个托管 () 打开 Internet 链接。 配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`notConfigured`、`microsoftEdge`。|
|isAssigned|Boolean|指示策略是否部署到任何包含组。 继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|应该用于托管应用中的数据的加密类型。 可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。|
|minimumRequiredSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|deployedAppCount|Int32|当前策略部署到的应用的计数。|
|faceIdBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。|
|customBrowserProtocol|String|在 iOS 上打开 Web 链接的自定义浏览器协议。 配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合|策略部署到的包含组和排除组列表的导航属性。 继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)|
|apps|[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合|策略部署到的应用的列表。|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|配置的部署摘要的导航属性。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "managedBrowser": "String",
  "isAssigned": true,
  "appDataEncryptionType": "String",
  "minimumRequiredSdkVersion": "String",
  "deployedAppCount": 1024,
  "faceIdBlocked": true,
  "customBrowserProtocol": "String"
}
```




