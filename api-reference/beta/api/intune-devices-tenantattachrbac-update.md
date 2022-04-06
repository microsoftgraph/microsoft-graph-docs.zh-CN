---
title: 更新 tenantAttachRBAC
description: 更新 tenantAttachRBAC 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6515e1f88337fc989653147a15810cac5f1bfaeb
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631013"
---
# <a name="update-tenantattachrbac"></a>更新 tenantAttachRBAC

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [tenantAttachRBAC 对象](../resources/intune-devices-tenantattachrbac.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/tenantAttachRBAC
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md) 对象的 JSON 表示形式。

下表显示创建 [tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|



## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/tenantAttachRBAC
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.tenantAttachRBAC"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.tenantAttachRBAC",
  "id": "37568f2c-8f2c-3756-2c8f-56372c8f5637"
}
```




