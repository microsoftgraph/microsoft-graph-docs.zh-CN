---
title: 更新 zebraFotaConnector
description: 更新 zebraFotaConnector 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f38c88548649d462747dd1df0aa56df23276a66d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213026"
---
# <a name="update-zebrafotaconnector"></a>更新 zebraFotaConnector

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/zebraFotaConnector
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) 对象提供 JSON 表示形式。

下表显示了创建 [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|ZebraFotaConnector 的 ID。|
|state|[zebraFotaConnectorState](../resources/intune-androidfotaservice-zebrafotaconnectorstate.md)|Zebra 连接器状态。 可取值为：`none`、`connected`、`disconnected`、`unknownFutureValue`。|
|enrollmentToken|String|Zebra 的租户注册令牌。 该令牌用于通过应用配置在 FOTA 服务中注册 Zebra 设备。|
|enrollmentAuthorizationUrl|String|完成帐户注册授权 URL。 这与 Zebra API 文档中的verification_uri_complete相对应。|
|lastSyncDateTime|DateTimeOffset|帐户上次与 Zebra 同步的日期和时间|
|fotaAppsApproved|Boolean|指示是否已批准所需的固件无线 (FOTA) 应用的标志。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/zebraFotaConnector
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "state": "connected",
  "enrollmentToken": "Enrollment Token value",
  "enrollmentAuthorizationUrl": "https://example.com/enrollmentAuthorizationUrl/",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "fotaAppsApproved": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "id": "2301310a-310a-2301-0a31-01230a310123",
  "state": "connected",
  "enrollmentToken": "Enrollment Token value",
  "enrollmentAuthorizationUrl": "https://example.com/enrollmentAuthorizationUrl/",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "fotaAppsApproved": true
}
```




