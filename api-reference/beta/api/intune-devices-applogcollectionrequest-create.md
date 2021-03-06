---
title: 创建 appLogCollectionRequest
description: 创建新的 appLogCollectionRequest 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbd19f042c6dbfe80a4c02ec224fde5b1e5fb696
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136480"
---
# <a name="create-applogcollectionrequest"></a>创建 appLogCollectionRequest

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 对象。

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
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 appLogCollectionRequest 对象的 JSON 表示形式。

下表显示创建 appLogCollectionRequest 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一标识符。 这是userId_DeviceId_AppId ID。|
|状态|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|记录上载状态。 可取值为：`pending`、`completed`、`failed`。|
|errorMessage|String|上传过程中出现错误消息（如果有）|
|customLogFolders|String collection|日志文件夹列表。 |
|completedDateTime|DateTimeOffset|上载日志请求达到终端状态的时间|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 306

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```




