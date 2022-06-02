---
title: 创建 windowsManagedAppProtection
description: 创建新的 windowsManagedAppProtection 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abc368802533ea2dcd0243a890dfdee32a82b30b
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858693"
---
# <a name="create-windowsmanagedappprotection"></a>创建 windowsManagedAppProtection

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagedAppProtections
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 windowsManagedAppProtection 对象提供 JSON 表示形式。

下表显示了创建 windowsManagedAppProtection 时所需的属性。

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



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsManagedAppProtections
Content-type: application/json
Content-length: 1453

{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "isAssigned": true,
  "deployedAppCount": 0,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "none",
  "allowedOutboundClipboardSharingLevel": "none",
  "allowedOutboundDataTransferDestinations": "none",
  "appActionIfUnableToAuthenticateUser": "wipe",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1625

{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "c7894cd1-4cd1-c789-d14c-89c7d14c89c7",
  "version": "Version value",
  "isAssigned": true,
  "deployedAppCount": 0,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "none",
  "allowedOutboundClipboardSharingLevel": "none",
  "allowedOutboundDataTransferDestinations": "none",
  "appActionIfUnableToAuthenticateUser": "wipe",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S"
}
```




