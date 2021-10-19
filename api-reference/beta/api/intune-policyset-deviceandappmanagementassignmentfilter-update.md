---
title: 更新 deviceAndAppManagementAssignmentFilter
description: 更新 deviceAndAppManagementAssignmentFilter 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c2fd8bfabcbb082b7d4dbb3c0d82adb6ff827f9
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60492938"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a>更新 deviceAndAppManagementAssignmentFilter

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceAndAppManagementAssignmentFilter 对象](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 的属性。

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
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceAndAppManagementAssignmentFilter 对象的](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) JSON 表示形式。

下表显示创建 [deviceAndAppManagementAssignmentFilter 时所需的属性](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|工作分配筛选器的键。|
|createdDateTime|DateTimeOffset|工作分配筛选器的创建时间。|
|lastModifiedDateTime|DateTimeOffset|工作分配筛选器的上次修改时间。|
|displayName|String|工作分配筛选器的 DisplayName。|
|说明|String|工作分配筛选器的说明。|
|平台|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|工作分配筛选器适用的设备的平台类型。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|rule|String|工作分配筛选器的规则定义。|
|roleScopeTags|String collection|工作分配筛选器的 RoleScopeTags。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
Content-type: application/json
Content-length: 274

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "819818db-18db-8198-db18-9881db189881",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```



