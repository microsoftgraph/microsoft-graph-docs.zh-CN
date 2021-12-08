---
title: 更新 windowsManagementApp
description: 更新 windowsManagementApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69cdb248653b44479f804121921e8cd694309405
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336315"
---
# <a name="update-windowsmanagementapp"></a>更新 windowsManagementApp

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [windowsManagementApp 对象](../resources/intune-devices-windowsmanagementapp.md) 的属性。

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
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [windowsManagementApp 对象的](../resources/intune-devices-windowsmanagementapp.md) JSON 表示形式。

下表显示创建 [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|管理应用程序的唯Windows标识符|
|availableVersion|String|Windows管理应用可用版本。|
|managedInstaller|[managedInstallerStatus](../resources/intune-devices-managedinstallerstatus.md)|托管安装程序状态。 可取值为：`disabled`、`enabled`。|
|managedInstallerConfiguredDateTime|String|托管安装程序配置的日期时间|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```




