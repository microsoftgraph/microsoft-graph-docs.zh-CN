---
title: 创建 deviceManagementComplianceActionItem
description: 创建新的 deviceManagementComplianceActionItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82a362cb22f3d4b23cf78d0e748f49510b4df25f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688255"
---
# <a name="create-devicemanagementcomplianceactionitem"></a>创建 deviceManagementComplianceActionItem

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 对象。

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
POST /deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}/scheduledActionsForRule/{deviceManagementComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementComplianceActionItem 对象的 JSON 表示形式。

下表显示创建 deviceManagementComplianceActionItem 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|包含此设置的策略中的此设置的键。 自动生成。|
|gracePeriodHours|Int32|强制执行操作前要等待的小时数。 有效值为 0 至 8760|
|actionType|[deviceManagementComplianceActionType](../resources/intune-deviceconfigv2-devicemanagementcomplianceactiontype.md)|要采取的操作。 可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。|
|notificationTemplateId|String|要使用的通知消息模板|
|notificationMessageCCList|String collection|指定此通知邮件抄送对象的组 ID 列表。 此集合最多可包含 100 个元素。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/compliancePolicies/{deviceManagementCompliancePolicyId}/scheduledActionsForRule/{deviceManagementComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceActionItem",
  "id": "cd938372-8372-cd93-7283-93cd728393cd",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```



