---
title: 更新 mobileAppInstallSummary
description: 更新 mobileAppInstallSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 19bd1e61359c5d2bdaff6ee87e807bae7dba0f05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864797"
---
# <a name="update-mobileappinstallsummary"></a>更新 mobileAppInstallSummary

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

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
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的 JSON 表示形式。

下表显示时创建[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|installedDeviceCount|Int32|已成功安装此应用程序的设备数。|
|failedDeviceCount|Int32|未能安装此应用程序的设备数。|
|notApplicableDeviceCount|Int32|不适用于此应用程序的设备数。|
|notInstalledDeviceCount|Int32|没有安装该应用程序的设备数目。|
|pendingInstallDeviceCount|Int32|已被通知安装此应用程序的设备数。|
|installedUserCount|Int32|所有成功安装此应用程序的设备的用户数。|
|failedUserCount|Int32|用户具有 1 或无法安装此应用程序的更多设备数。|
|notApplicableUserCount|Int32|其设备未所有适用于此应用程序的用户数。|
|notInstalledUserCount|Int32|未安装该应用程序的一个或多个设备的用户数。|
|pendingInstallUserCount|Int32|用户具有 1 或更多已经通知安装此应用程序和失败的 0 设备的设备数。|



## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
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





