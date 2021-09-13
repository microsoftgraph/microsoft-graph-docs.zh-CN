---
title: 更新 windowsDriverUpdateInventory
description: 更新 windowsDriverUpdateInventory 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 90abc5dec10bed9998cf988783f4cdb9c67fef89
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138510"
---
# <a name="update-windowsdriverupdateinventory"></a>更新 windowsDriverUpdateInventory

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [windowsDriverUpdateInventory 对象](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 的属性。

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
PATCH /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories/{windowsDriverUpdateInventoryId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 对象的 JSON 表示形式。

下表显示创建 [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|驱动程序的 ID。|
|name|String|驱动程序的名称。|
|version|String|驱动程序的版本。|
|manufacturer|String|驱动程序的制造商。|
|releaseDateTime|DateTimeOffset|驱动程序的发布日期时间。|
|driverClass|String|驱动程序的类。|
|applicableDeviceCount|Int32|此驱动程序适用的设备数量。|
|approvalStatus|[driverApprovalStatus](../resources/intune-softwareupdate-driverapprovalstatus.md)|此驱动程序的审批状态。 可取值为：`needsReview`、`declined`、`approved`、`suspended`。|
|“类别”|[driverCategory](../resources/intune-softwareupdate-drivercategory.md)|此驱动程序的类别。 可取值为：`recommended`、`previouslyApproved`、`other`。|
|deployDateTime|DateTimeOffset|如果 approvalStatus 获得批准，应部署驱动程序的日期时间。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories/{windowsDriverUpdateInventoryId}
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
  "name": "Name value",
  "version": "Version value",
  "manufacturer": "Manufacturer value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "driverClass": "Driver Class value",
  "applicableDeviceCount": 5,
  "approvalStatus": "declined",
  "category": "previouslyApproved",
  "deployDateTime": "2017-01-01T00:01:14.7822152-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
  "id": "3b14b403-b403-3b14-03b4-143b03b4143b",
  "name": "Name value",
  "version": "Version value",
  "manufacturer": "Manufacturer value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "driverClass": "Driver Class value",
  "applicableDeviceCount": 5,
  "approvalStatus": "declined",
  "category": "previouslyApproved",
  "deployDateTime": "2017-01-01T00:01:14.7822152-08:00"
}
```



