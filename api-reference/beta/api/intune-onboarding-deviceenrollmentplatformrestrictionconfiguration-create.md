---
title: 创建 deviceEnrollmentPlatformRestrictionConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58c2cf5df254b13eaa11e2e8ccd62e9b2658085f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212292"
---
# <a name="create-deviceenrollmentplatformrestrictionconfiguration"></a>创建 deviceEnrollmentPlatformRestrictionConfiguration

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 deviceEnrollmentPlatformRestrictionConfiguration 对象提供 JSON 表示形式。

下表显示了创建 deviceEnrollmentPlatformRestrictionConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的帐户的唯一标识符|
|displayName|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的显示名称|
|说明|字符串|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配了注册配置的多个组中时，将使用优先级。 用户仅受优先级最低的配置的约束。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|在 UTC 中创建的设备注册配置的日期时间继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的 UTC 中上次修改的日期时间|
|version|Int32|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的版本|
|roleScopeTagIds|字符串集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|支持从 [deviceEnrollmentConfiguration 继承的](../resources/intune-shared-deviceenrollmentconfiguration.md)注册配置类型。 可能的值是：`unknown`、`limit`、`platformRestrictions`、`windowsHelloForBusiness`、`defaultLimit`、`defaultPlatformRestrictions`、`defaultWindowsHelloForBusiness`、`defaultWindows10EnrollmentCompletionPageConfiguration`、`windows10EnrollmentCompletionPageConfiguration`、`deviceComanagementAuthorityConfiguration`、`singlePlatformRestriction`、`unknownFutureValue`、`enrollmentNotificationsConfiguration`。|
|platformRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|基于平台、平台操作系统版本和设备所有权的限制|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|此限制适用的平台类型。 可取值为：`allPlatforms`、`ios`、`windows`、`windowsPhone`、`android`、`androidForWork`、`mac`。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 765

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
  "platformRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "platformType": "ios"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 937

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration",
  "id": "dedce9f4-e9f4-dedc-f4e9-dcdef4e9dcde",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
  "platformRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "platformType": "ios"
}
```




