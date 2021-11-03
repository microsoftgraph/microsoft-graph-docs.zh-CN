---
title: 更新 userExperienceAnalyticsScoreHistory
description: 更新 userExperienceAnalyticsScoreHistory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6a40bf69f1b387c14657b2ae6e307d8b1a6d6a2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688841"
---
# <a name="update-userexperienceanalyticsscorehistory"></a>更新 userExperienceAnalyticsScoreHistory

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsScoreHistory 对象](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsScoreHistory 时所需的属性](../resources/intune-devices-userexperienceanalyticsscorehistory.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析设备启动过程的唯一标识符。|
|startupDateTime|DateTimeOffset|用户体验分析设备启动日期时间。|
|overallScore|Int32|用户体验分析总体分数。 分数范围为 0-100，100 是理想分数。 有效值为 0 至 100|
|startupScore|Int32|用户体验分析设备启动分数。 分数范围为 0-100，100 是理想分数。|
|coreBootScore|Int32|用户体验分析设备核心启动分数。 分数范围为 0-100，100 是理想分数。|
|coreSigninScore|Int32|用户体验分析设备核心登录分数。 分数范围为 0-100，100 是理想分数。|
|recommendedSoftwareScore|Int32|用户体验分析设备核心登录分数。 分数范围为 0-100，100 是理想分数。|
|appHealthOverallScore|Int32|用户体验分析应用运行状况总体分数。|
|batteryHealthScore|Int32|用户体验分析电池运行状况分数。|
|startupTotalDevices|Int32|用户体验分析类别启动性能的总设备计数。|
|recommendedSoftwareTotalDevices|Int32|用户体验分析类别推荐软件的总设备计数。|
|appHealthTotalDevices|Int32|用户体验分析类别应用运行状况的总设备计数。|
|batteryHealthTotalDevices|Int32|用户体验分析类别电池运行状况的总设备计数。|
|restartScore|Int32|重启分数。 分数将在 0-100 之间，100 是理想分数，0 表示重启过多。 有效值为 0 到 9999999|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 485

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "appHealthOverallScore": 5,
  "batteryHealthScore": 2,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "batteryHealthTotalDevices": 9,
  "restartScore": 12
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 534

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "appHealthOverallScore": 5,
  "batteryHealthScore": 2,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "batteryHealthTotalDevices": 9,
  "restartScore": 12
}
```



