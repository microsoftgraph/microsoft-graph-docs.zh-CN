---
title: 更新 hardwareConfigurationRunSummary
description: 更新 hardwareConfigurationRunSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5657005360e6f66d361f9490481d2b89653ea244
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348416"
---
# <a name="update-hardwareconfigurationrunsummary"></a>更新 hardwareConfigurationRunSummary

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [hardwareConfigurationRunSummary 对象](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) 的属性。

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
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) 对象的 JSON 表示形式。

下表显示创建 [hardwareConfigurationRunSummary 时所需的属性](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置运行摘要实体的键。 此属性是只读的。|
|successfulDeviceCount|Int32|已配置硬件而未出现任何问题的设备数量|
|failedDeviceCount|Int32|硬件配置发现问题的设备数量|
|pendingDeviceCount|Int32|其硬件配置为待定状态的设备数量|
|errorDeviceCount|Int32|硬件配置状态为错误的设备数量|
|notApplicableDeviceCount|Int32|硬件配置状态不适用的设备数量|
|unknownDeviceCount|Int32|硬件配置状态未知的设备数量|
|successfulUserCount|Int32|未出现任何问题的情况下配置其硬件的用户数量|
|failedUserCount|Int32|硬件配置发现问题的用户数量|
|pendingUserCount|Int32|其硬件配置为待定状态的用户数量|
|errorUserCount|Int32|硬件配置状态为错误的用户数量|
|notApplicableUserCount|Int32|硬件配置状态不适用的用户数量|
|unknownUserCount|Int32|硬件配置状态未知用户的数量|
|lastRunDateTime|DateTimeOffset|跨所有设备的配置的上次运行时间|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
Content-type: application/json
Content-length: 469

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2,
  "successfulUserCount": 3,
  "failedUserCount": 15,
  "pendingUserCount": 0,
  "errorUserCount": 14,
  "notApplicableUserCount": 6,
  "unknownUserCount": 0,
  "lastRunDateTime": "2016-12-31T23:57:28.499537-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "id": "76b964f2-64f2-76b9-f264-b976f264b976",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2,
  "successfulUserCount": 3,
  "failedUserCount": 15,
  "pendingUserCount": 0,
  "errorUserCount": 14,
  "notApplicableUserCount": 6,
  "unknownUserCount": 0,
  "lastRunDateTime": "2016-12-31T23:57:28.499537-08:00"
}
```




