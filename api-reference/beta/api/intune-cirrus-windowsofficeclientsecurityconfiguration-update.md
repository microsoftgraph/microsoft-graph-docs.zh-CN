---
title: 更新 windowsOfficeClientSecurityConfiguration
description: 更新 windowsOfficeClientSecurityConfiguration 对象的属性。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b346c7218ab35368d4a71a964b7a10461a61c93
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785003"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a>更新 windowsOfficeClientSecurityConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [windowsOfficeClientSecurityConfiguration 对象](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 对象的 JSON 表示形式。

下表显示创建 [windowsOfficeClientSecurityConfiguration 时所需的属性](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Office 客户端配置策略的 ID。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Stream|首选项设置 二进制格式的 JSON 字符串，用户可以替代这些值。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Stream|策略设置 二进制格式的 JSON 字符串，用户无法更改这些值。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|String|管理员提供了 Office 客户端配置策略的说明。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|字符串|管理员提供的 Office 客户端配置策略的名称。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|assignments|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合|策略的组分配列表。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|priority|Int32|优先级值应为租户下每个策略的唯一值，并且将用于冲突解决，较低的值表示优先级较高。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|日期/时间|策略的上次修改日期/时间戳。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|策略的用户签入摘要。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合|Office 客户端签入状态列表。 继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}
Content-type: application/json
Content-length: 949

{
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```



