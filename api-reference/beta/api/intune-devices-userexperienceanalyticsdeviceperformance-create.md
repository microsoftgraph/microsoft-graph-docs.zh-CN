---
title: 创建 userExperienceAnalyticsDevicePerformance
description: 创建新的 userExperienceAnalyticsDevicePerformance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3632c3e9982a1f9ca37b6af931491ecac4e0974
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789072"
---
# <a name="create-userexperienceanalyticsdeviceperformance"></a>创建 userExperienceAnalyticsDevicePerformance

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 userExperienceAnalyticsDevicePerformance 对象的 JSON 表示形式。

下表显示创建 userExperienceAnalyticsDevicePerformance 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|用户体验分析设备启动性能设备的唯一标识符。|
|deviceName|String|用户体验分析设备名称。|
|model|String|用户体验分析设备模型。|
|manufacturer|String|用户体验分析设备制造商。|
|diskType|[diskType](../resources/intune-devices-disktype.md)|用户体验分析设备磁盘类型。 可取值为：`unkown`、`hdd`、`ssd`。|
|operatingSystemVersion|String|用户体验分析设备操作系统版本。|
|bootScore|Int32|用户体验分析设备启动分数。|
|coreBootTimeInMs|Int32|用户体验分析设备核心启动时间（以毫秒为单位）。|
|groupPolicyBootTimeInMs|Int32|用户体验分析设备组策略启动时间（以毫秒为单位）。|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析设备的运行状况。 可能的值是：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|loginScore|Int32|用户体验分析设备登录分数。|
|coreLoginTimeInMs|Int32|用户体验分析设备核心登录时间（以毫秒为单位）。|
|groupPolicyLoginTimeInMs|Int32|用户体验分析设备组策略登录时间（以毫秒为单位）。|
|deviceCount|Int64|用户体验分析汇总了设备计数。|
|responsiveDesktopTimeInMs|Int32|用户体验分析响应式桌面时间（以毫秒为单位）。|
|blueScreenCount|Int32|最近 14 天内的蓝屏数。 有效值为 0 到 9999999|
|restartCount|Int32|最近 14 天内的重启次数。 有效值为 0 到 9999999|
|averageBlueScreens|双精度|平均 (表示) 14 天内每个设备的蓝屏数量。 有效值为 0 到 9999999|
|averageRestarts|双精度|平均 (平均) 最近 14 天内每个设备的重启次数。 有效值为 0 到 9999999|
|startupPerformanceScore|双精度|用户体验分析设备启动性能分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|modelStartupPerformanceScore|双精度|用户体验分析模型级别的启动性能分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
Content-type: application/json
Content-length: 739

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0,
  "startupPerformanceScore": 7.666666666666667,
  "modelStartupPerformanceScore": 9.3333333333333339
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 788

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "852ae826-e826-852a-26e8-2a8526e82a85",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0,
  "startupPerformanceScore": 7.666666666666667,
  "modelStartupPerformanceScore": 9.3333333333333339
}
```



