---
title: 创建 microsoftTunnelHealthThreshold
description: 创建新的 microsoftTunnelHealthThreshold 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eec3d33082e1accef4c9bb0f5ec7f980009a2c13
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59041806"
---
# <a name="create-microsofttunnelhealththreshold"></a>创建 microsoftTunnelHealthThreshold

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelHealthThresholds
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 microsoftTunnelHealthThreshold 对象的 JSON 表示形式。

下表显示创建 microsoftTunnelHealthThreshold 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|指标名称|
|healthyThreshold|Int64|正常运行的阈值|
|unhealthyThreshold|Int64|不正常的阈值|
|defaultHealthyThreshold|Int64|正常运行的默认阈值|
|defaultUnhealthyThreshold|Int64|不正常的默认阈值|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelHealthThresholds
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "healthyThreshold": 0,
  "unhealthyThreshold": 2,
  "defaultHealthyThreshold": 7,
  "defaultUnhealthyThreshold": 9
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "id": "419c526e-526e-419c-6e52-9c416e529c41",
  "healthyThreshold": 0,
  "unhealthyThreshold": 2,
  "defaultHealthyThreshold": 7,
  "defaultUnhealthyThreshold": 9
}
```



