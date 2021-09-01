---
title: 更新 certificateConnectorDetails
description: 更新 certificateConnectorDetails 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: daec761daba4abace27af57f0915fcc073358e7c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789272"
---
# <a name="update-certificateconnectordetails"></a>更新 certificateConnectorDetails

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [certificateConnectorDetails 对象](../resources/intune-raimportcerts-certificateconnectordetails.md) 的属性。

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
PATCH /deviceManagement/certificateConnectorDetails/{certificateConnectorDetailsId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md) 对象的 JSON 表示形式。

下表显示创建 [certificateConnectorDetails 时所需的属性](../resources/intune-raimportcerts-certificateconnectordetails.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|此 ConnectorDetails 集的唯一标识符。|
|connectorName|字符串|连接器名称 (注册期间设置的) 。|
|machineName|String|承载此连接器服务的机器的名称。|
|enrollmentDateTime|DateTimeOffset|注册此连接器的日期/时间。|
|lastCheckinDateTime|DateTimeOffset|此连接器上次连接到服务的日期/时间。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/certificateConnectorDetails/{certificateConnectorDetailsId}
Content-type: application/json
Content-length: 278

{
  "@odata.type": "#microsoft.graph.certificateConnectorDetails",
  "connectorName": "Connector Name value",
  "machineName": "Machine Name value",
  "enrollmentDateTime": "2016-12-31T23:57:59.3726057-08:00",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "@odata.type": "#microsoft.graph.certificateConnectorDetails",
  "id": "104d7361-7361-104d-6173-4d1061734d10",
  "connectorName": "Connector Name value",
  "machineName": "Machine Name value",
  "enrollmentDateTime": "2016-12-31T23:57:59.3726057-08:00",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```



