---
title: 创建 microsoftTunnelServerLogCollectionResponse
description: 创建新的 microsoftTunnelServerLogCollectionResponse 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ed03526f01e73b30a8a199a6edc6bb5e5f8ef10
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341080"
---
# <a name="create-microsofttunnelserverlogcollectionresponse"></a>创建 microsoftTunnelServerLogCollectionResponse

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelServerLogCollectionResponses
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 microsoftTunnelServerLogCollectionResponse 对象的 JSON 表示形式。

下表显示创建 microsoftTunnelServerLogCollectionResponse 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一 ID|
|状态|[microsoftTunnelLogCollectionStatus](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|日志集合的状态。 可取值为：`pending`、`completed`、`failed`。|
|startDateTime|DateTimeOffset|收集的日志的开始时间 |
|endDateTime|DateTimeOffset|收集的日志的结束时间|
|sizeInBytes|Int64|日志的大小（以字节为单位）|
|serverId|String|请求日志集合的服务器 ID|
|requestDateTime|DateTimeOffset|请求日志集合的时间|
|expiryDateTime|DateTimeOffset|日志集合过期的时间|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses
Content-type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11,
  "serverId": "Server Id value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expiryDateTime": "2017-01-01T00:03:32.5199332-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 444

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11,
  "serverId": "Server Id value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expiryDateTime": "2017-01-01T00:03:32.5199332-08:00"
}
```




