---
title: 更新 userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
description: 更新 userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 473c01d8c59912bc88880aaff42fe105b35ba234
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265547"
---
# <a name="update-userexperienceanalyticsworkfromanywherehardwarereadinessmetric"></a>更新 userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric 对象](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric 时所需的属性](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析硬件准备情况指标对象的唯一标识符。|
|totalDeviceCount|Int32|组织中设备总数。 有效值 -2147483648 to 2147483647|
|upgradeEligibleDeviceCount|Int32|组织中符合 Windows 升级条件的设备计数。 有效值 -2147483648 to 2147483647|
|ramCheckFailedPercentage|双精度|RAM 硬件检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|storageCheckFailedPercentage|双精度|存储硬件检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processorCoreCountCheckFailedPercentage|双精度|处理器硬件核心计数检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processorSpeedCheckFailedPercentage|双精度|处理器硬件速度检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|tpmCheckFailedPercentage|双精度|受信任的平台模块与 TPM (检查) 的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|secureBootCheckFailedPercentage|双精度|安全启动硬件检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processorFamilyCheckFailedPercentage|双精度|处理器硬件系列检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processor64BitCheckFailedPercentage|双精度|处理器硬件 64 位体系结构检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|osCheckFailedPercentage|双精度|操作系统检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
Content-type: application/json
Content-length: 626

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "totalDeviceCount": 0,
  "upgradeEligibleDeviceCount": 10,
  "ramCheckFailedPercentage": 8.0,
  "storageCheckFailedPercentage": 9.3333333333333339,
  "processorCoreCountCheckFailedPercentage": 13.0,
  "processorSpeedCheckFailedPercentage": 11.666666666666666,
  "tpmCheckFailedPercentage": 8.0,
  "secureBootCheckFailedPercentage": 10.333333333333334,
  "processorFamilyCheckFailedPercentage": 12.0,
  "processor64BitCheckFailedPercentage": 11.666666666666666,
  "osCheckFailedPercentage": 7.666666666666667
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "id": "6df21a06-1a06-6df2-061a-f26d061af26d",
  "totalDeviceCount": 0,
  "upgradeEligibleDeviceCount": 10,
  "ramCheckFailedPercentage": 8.0,
  "storageCheckFailedPercentage": 9.3333333333333339,
  "processorCoreCountCheckFailedPercentage": 13.0,
  "processorSpeedCheckFailedPercentage": 11.666666666666666,
  "tpmCheckFailedPercentage": 8.0,
  "secureBootCheckFailedPercentage": 10.333333333333334,
  "processorFamilyCheckFailedPercentage": 12.0,
  "processor64BitCheckFailedPercentage": 11.666666666666666,
  "osCheckFailedPercentage": 7.666666666666667
}
```




