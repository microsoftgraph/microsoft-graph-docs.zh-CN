---
title: 更新 mobileAppTroubleshootingEvent
description: 介绍 Microsoft for Intune Graph API 的更新 mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e08d81f6738a6734b2a23c44e653263fc86fec69
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59107349"
---
# <a name="update-mobileapptroubleshootingevent"></a>更新 mobileAppTroubleshootingEvent

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本的 API 可能会更改。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [mobileAppTroubleshootingEvent 对象](../resources/intune-shared-mobileapptroubleshootingevent.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
|&nbsp; &nbsp; **设备管理**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **疑难解答**|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
|&nbsp; &nbsp; **设备管理**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **疑难解答**|DeviceManagementManagedDevices.ReadWrite.All|

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
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的 JSON 表示形式。

下表显示创建 [mobileAppTroubleshootingEvent 时所需的属性](../resources/intune-shared-mobileapptroubleshootingevent.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|**疑难解答**|
|additionalInformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|一组字符串键和字符串值对，提供有关疑难解答事件的其他信息。|
|applicationId|String|Intune 应用程序标识符。|
|correlationId|String|用于跟踪服务中的故障的 ID。 |
|eventDateTime|DateTimeOffset|事件发生的时间。 |
|eventName|String|与疑难解答事件对应的事件名称。 可选。|
|history|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) 集合|Intune 移动应用程序疑难解答历史记录项。|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|包含有关错误及其修正的详细信息的对象。 |
|userId|String|尝试注册设备的用户的标识符。|

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象。

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










