---
title: 更新 mobileAppTroubleshootingEvent
description: 介绍 Microsoft Graph API 的 Update mobileAppTroubleshootingEvent 方法 Intune，支持多个工作流。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10bf103a3e796cb5a9e84f1c87ff0571c0bbf551
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429451"
---
# <a name="update-mobileapptroubleshootingevent"></a>更新 mobileAppTroubleshootingEvent

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
|&nbsp; &nbsp; **设备管理**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **疑难解答**|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的 JSON 表示形式。

下表显示时创建[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|**疑难解答**|
|additionalInformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|字符串键和字符串值对的一组提供了有关疑难解答事件其他信息。|
|applicationId|String|Intune 应用程序标识符。|
|correlationId|String|用于跟踪服务中的失败的 ID。 |
|eventDateTime|DateTimeOffset|该事件发生的时间。 |
|事件名称|String|对应于疑难解答事件的事件名称。 可选。|
|历史记录|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合|疑难解答历史记录项 Intune 移动应用程序。|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|对象包含有关错误和其修复的详细的信息。 |
|userId|String|尝试注册设备的用户的标识符。|

## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




