---
title: 更新 mobileAppInstallSummary
description: 更新 mobileAppInstallSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc911920a1027c4157b373069d8503b1ed5245d388059973ac6111677fd35fdb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180143"
---
# <a name="update-mobileappinstallsummary"></a>更新 mobileAppInstallSummary

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [mobileAppInstallSummary 对象](../resources/intune-apps-mobileappinstallsummary.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象的 JSON 表示形式。

下表显示创建 [mobileAppInstallSummary 时所需的属性](../resources/intune-apps-mobileappinstallsummary.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|installedDeviceCount|Int32|已成功安装此应用的设备数。|
|failedDeviceCount|Int32|未能安装此应用的设备数。|
|notApplicableDeviceCount|Int32|不适用于此应用的设备数。|
|notInstalledDeviceCount|Int32|未安装此应用的设备数。|
|pendingInstallDeviceCount|Int32|已通知安装此应用的设备数。|
|installedUserCount|Int32|其设备全部成功安装此应用的用户数。|
|failedUserCount|Int32|拥有 1 台或多台设备未能安装此应用的用户数量。|
|notApplicableUserCount|Int32|其设备均不适用于此应用的用户数。|
|notInstalledUserCount|Int32|具有 1 台或多台设备未安装此应用的用户数量。|
|pendingInstallUserCount|Int32|拥有 1 台或多台设备且已收到通知安装此应用且设备有 0 台失败的用户数量。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```




