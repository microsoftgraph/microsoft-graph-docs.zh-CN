---
title: 创建 deviceManagementPartner
description: 创建新的 deviceManagementPartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e771bc99a2348f461c1306ee870c635fd4718f044980b2c77b1d70fac2cc027
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54203986"
---
# <a name="create-devicemanagementpartner"></a>创建 deviceManagementPartner

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementPartner 对象的 JSON 表示形式。

下表显示创建 deviceManagementPartner 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的 ID|
|lastHeartbeatDateTime|DateTimeOffset|管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|此租户的合作伙伴状态。 可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|合作伙伴应用类型。 可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。|
|singleTenantAppId|String|合作伙伴单个租户应用 ID|
|displayName|字符串|合作伙伴显示名称|
|isConfigured|Boolean|是否配置了设备管理合作伙伴|
|whenPartnerDevicesWillBeRemoved|DateTimeOffset|将删除 PartnerDevices 的 DateTime（UTC 时间）。 这将很快成为删除。|
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset|将 PartnerDevices 标记为"不兼容"的 DateTime（UTC 时间）。 这将很快成为删除。|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|要删除 PartnerDevices 时的日期/时间（UTC 时间）|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）|
|groupsRequiringPartnerEnrollment|[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) 集合|指定是否通过合作伙伴注册的用户组。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 1140

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1189

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




