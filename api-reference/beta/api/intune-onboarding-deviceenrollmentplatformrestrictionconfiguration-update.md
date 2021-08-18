---
title: 更新 deviceEnrollmentPlatformRestrictionConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0badf01c10ff5f63adf294a53b7f070e8712b025
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259280"
---
# <a name="update-deviceenrollmentplatformrestrictionconfiguration"></a>更新 deviceEnrollmentPlatformRestrictionConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceEnrollmentPlatformRestrictionConfiguration 对象](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 对象的 JSON 表示形式。

下表显示创建 [deviceEnrollmentPlatformRestrictionConfiguration 时所需的属性](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|字符串|设备注册显示名称继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|String|设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|如果用户位于分配了注册配置的多个组中，则使用优先级。 用户仅受优先级值最低的配置使用。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|String collection|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|platformRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|基于平台、平台操作系统版本和设备所有权的限制|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|应用此限制的平台类型。 可取值为：`allPlatforms`、`ios`、`windows`、`windowsPhone`、`android`、`androidForWork`、`androidAosp`、`mac`。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 716

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 888

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




