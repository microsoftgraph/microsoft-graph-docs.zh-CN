---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d346884d22ec9dbdae554b396eebdca00f4ac7af
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787333"
---
# <a name="get-devicecategory"></a>获取 deviceCategory

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本的 API 可能会更改。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All|
| &nbsp; &nbsp; **载入** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All|
| &nbsp; &nbsp; **载入** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP 请求

**设备管理**

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

**载入**

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头

|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是请求的示例。

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a>响应

下面是一个响应示例。 注意：为简洁起见，可能会截断此处显示的响应对象。 从实际调用返回的属性因上下文而异。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```









