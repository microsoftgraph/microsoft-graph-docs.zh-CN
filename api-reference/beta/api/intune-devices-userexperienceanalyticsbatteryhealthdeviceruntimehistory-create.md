---
title: 创建 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory
description: 创建新的 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 908a95223edf46681976c9d0224ee34c7713aa3a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695552"
---
# <a name="create-userexperienceanalyticsbatteryhealthdeviceruntimehistory"></a>创建 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) 对象。

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
POST /deviceManagement/userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 对象的 JSON 表示形式。

下表显示创建 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况运行时对象的唯一标识符。|
|deviceId|String|设备的唯一标识符，Intune DeviceID 或 SCCM 设备 ID。|
|runtimeDateTime|String|运行时历史记录实例的日期时间。|
|estimatedRuntimeInMinutes|Int32|电池完全充电时设备的预计运行时。 单位（以分钟表示）。 有效值 -2147483648 2147483647|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory",
  "deviceId": "Device Id value",
  "runtimeDateTime": "Runtime Date Time value",
  "estimatedRuntimeInMinutes": 9
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory",
  "id": "0fbcbdaf-bdaf-0fbc-afbd-bc0fafbdbc0f",
  "deviceId": "Device Id value",
  "runtimeDateTime": "Runtime Date Time value",
  "estimatedRuntimeInMinutes": 9
}
```



