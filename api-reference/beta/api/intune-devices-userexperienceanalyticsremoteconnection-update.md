---
title: 更新 userExperienceAnalyticsRemoteConnection
description: 更新 userExperienceAnalyticsRemoteConnection 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a26b5bfaabe9a10eb77f7f3337138d47db0dea88
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159135"
---
# <a name="update-userexperienceanalyticsremoteconnection"></a>更新 userExperienceAnalyticsRemoteConnection

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsRemoteConnection 对象](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsRemoteConnection 时所需的属性](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析远程连接实体的唯一标识符。|
|deviceId|String|设备的 ID。|
|deviceName|String|设备的名称。|
|model|String|用户体验分析设备模型。|
|virtualNetwork|String|用户体验分析虚拟网络。|
|deviceCount|Int32|远程连接计数。 有效值为 0 到 2147483647|
|cloudPcRoundTripTime|双精度|云电脑设备的舍入提示时间。 有效值为 0 到 1.79769313486232E+308|
|cloudPcSignInTime|双精度|云电脑设备的登录时间。 有效值为 0 到 1.79769313486232E+308|
|remoteSignInTime|双精度|云电脑设备的远程登录时间。 有效值为 0 到 1.79769313486232E+308|
|coreBootTime|双精度|云电脑设备的核心启动时间。 有效值为 0 到 1.79769313486232E+308|
|coreSignInTime|双精度|云电脑设备的核心登录时间。 有效值为 0 到 1.79769313486232E+308|
|cloudPcFailurePercentage|双精度|云电脑设备的登录失败百分比。 有效值为 0 至 100|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```




