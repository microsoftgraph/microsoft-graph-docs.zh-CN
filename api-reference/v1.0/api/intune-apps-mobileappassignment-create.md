---
title: 创建 mobileAppAssignment
description: 创建新的 mobileAppAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc9fd43ae46e66772eae5ef6a492cae9802692fc
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730523"
---
# <a name="create-mobileappassignment"></a>创建 mobileAppAssignment

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。

下表显示创建 mobileAppAssignment 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|intent|[installIntent](../resources/intune-shared-installintent.md)|由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|由管理员定义的目标组分配。|
|settings|[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)|由管理员定义的目标分配的设置。|



## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 861

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings",
    "notifications": "showReboot",
    "restartSettings": {
      "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
      "gracePeriodInMinutes": 4,
      "countdownDisplayBeforeRestartInMinutes": 6,
      "restartNotificationSnoozeDurationInMinutes": 10
    },
    "installTimeSettings": {
      "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
      "useLocalTime": true,
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "deadlineDateTime": "2017-01-01T00:00:21.0378955-08:00"
    },
    "deliveryOptimizationPriority": "foreground"
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 910

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings",
    "notifications": "showReboot",
    "restartSettings": {
      "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
      "gracePeriodInMinutes": 4,
      "countdownDisplayBeforeRestartInMinutes": 6,
      "restartNotificationSnoozeDurationInMinutes": 10
    },
    "installTimeSettings": {
      "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
      "useLocalTime": true,
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "deadlineDateTime": "2017-01-01T00:00:21.0378955-08:00"
    },
    "deliveryOptimizationPriority": "foreground"
  }
}
```





