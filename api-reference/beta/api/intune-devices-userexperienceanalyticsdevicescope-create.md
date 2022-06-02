---
title: 创建 userExperienceAnalyticsDeviceScope
description: 创建新的 userExperienceAnalyticsDeviceScope 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edca6bf2c5a88a17ea155510ac8a5fb0e1c07d2a
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857993"
---
# <a name="create-userexperienceanalyticsdevicescope"></a>创建 userExperienceAnalyticsDeviceScope

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceScopes
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 userExperienceAnalyticsDeviceScope 对象提供 JSON 表示形式。

下表显示了创建 userExperienceAnalyticsDeviceScope 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|设备范围配置的唯一标识符。|
|deviceScopeName|String|用户体验分析设备范围配置的名称。|
|ownerId|String|创建设备范围配置的管理员)  (人员的唯一标识符。|
|isBuiltIn|Boolean|指示设备范围配置是内置配置还是自定义配置。 如果为 TRUE，则设备范围配置是内置的。 如果为 FALSE，则设备范围配置为自定义。 默认值为 FALSE。|
|enabled|Boolean|指示设备范围是已启用还是已禁用。 如果为 TRUE，则启用设备范围。 如果为 FALSE，则禁用设备范围。 默认值为 FALSE。|
|status|[deviceScopeStatus](../resources/intune-devices-devicescopestatus.md)|指示设备范围启用后的设备范围状态。 可能的值为：none、computing、insufficientData 或 completed。 默认值为无。 可取值为：`none`、`computing`、`insufficientData`、`completed`、`unknownFutureValue`。|
|形参|[deviceScopeParameter](../resources/intune-devices-devicescopeparameter.md)|设备范围配置参数。 将来将扩展它以添加更多参数。 Eg：设备范围参数可以是 OS 版本、磁盘类型、设备制造商、设备模型或范围标记。 默认值：scopeTag。 可取值为：`none`、`scopeTag`、`unknownFutureValue`。|
|operator|[deviceScopeOperator](../resources/intune-devices-devicescopeoperator.md)|设备范围配置查询运算符。 可能的值为：equals、notEquals、contains、notContains、greaterThan、lessThan。 默认值：等于。 可取值为：`none`、`equals`、`unknownFutureValue`。|
|valueObjectId|String|用于创建设备范围配置的用户设备范围标记 ID 的唯一标识符。|
|value|String|设备范围配置查询子句值。|
|createdDateTime|DateTimeOffset|指示自定义设备范围的创建日期和时间。|
|lastModifiedDateTime|DateTimeOffset|指示自定义设备范围的上次更新日期和时间。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScopes
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "deviceScopeName": "Device Scope Name value",
  "ownerId": "Owner Id value",
  "isBuiltIn": true,
  "enabled": true,
  "status": "computing",
  "parameter": "scopeTag",
  "operator": "equals",
  "valueObjectId": "Value Object Id value",
  "value": "Value value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "id": "936b0460-0460-936b-6004-6b9360046b93",
  "deviceScopeName": "Device Scope Name value",
  "ownerId": "Owner Id value",
  "isBuiltIn": true,
  "enabled": true,
  "status": "computing",
  "parameter": "scopeTag",
  "operator": "equals",
  "valueObjectId": "Value Object Id value",
  "value": "Value value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




