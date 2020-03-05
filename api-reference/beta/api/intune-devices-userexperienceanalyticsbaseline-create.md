---
title: 创建 userExperienceAnalyticsBaseline
description: 创建新的 userExperienceAnalyticsBaseline 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14191e3b35ff1854eb8d7b14793991da1b31537c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468584"
---
# <a name="create-userexperienceanalyticsbaseline"></a>创建 userExperienceAnalyticsBaseline

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 userExperienceAnalyticsBaseline 对象的 JSON 表示形式。

下表显示创建 userExperienceAnalyticsBaseline 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 比较基准的唯一标识符。|
|displayName|String|User experience analytics 基线的名称。|
|overallScore|Int32|用户体验分析基准的总体分数。|
|isBuiltIn|Boolean|指示当前基线是商业中间基线还是自定义基线。|
|createdDateTime|DateTimeOffset|自定义基线的创建日期。|



## <a name="response"></a>响应
如果成功，此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00"
}
```





