---
title: 更新 userExperienceAnalyticsBatteryHealthRuntimeDetails
description: 更新 userExperienceAnalyticsBatteryHealthRuntimeDetails 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 51c4158b46f4fb3cc9a3f90fb01817d019ec2105
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335094"
---
# <a name="update-userexperienceanalyticsbatteryhealthruntimedetails"></a>更新 userExperienceAnalyticsBatteryHealthRuntimeDetails

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsBatteryHealthRuntimeDetails 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) 的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthRuntimeDetails
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsBatteryHealthRuntimeDetails 时所需的属性](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况运行时对象的唯一标识符。|
|activeDevices|Int32|租户中的活动设备数。 有效值 -2147483648 to 2147483647|
|batteryRuntimeGood|Int32|活动运行时大于 5 小时的设备数量。 有效值 -2147483648 to 2147483647|
|batteryRuntimeFair|Int32|活动运行时大于 3 小时但小于 5 小时的设备数量。 有效值 -2147483648 to 2147483647|
|batteryRuntimePoor|Int32|活动运行时小于 3 小时的设备数量。 有效值 -2147483648 to 2147483647|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthRuntimeDetails
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails",
  "activeDevices": 13,
  "batteryRuntimeGood": 2,
  "batteryRuntimeFair": 2,
  "batteryRuntimePoor": 2
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails",
  "id": "f6ac1dbf-1dbf-f6ac-bf1d-acf6bf1dacf6",
  "activeDevices": 13,
  "batteryRuntimeGood": 2,
  "batteryRuntimeFair": 2,
  "batteryRuntimePoor": 2
}
```




