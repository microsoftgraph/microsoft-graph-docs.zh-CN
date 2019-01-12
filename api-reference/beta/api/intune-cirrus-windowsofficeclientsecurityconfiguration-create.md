---
title: 创建 windowsOfficeClientSecurityConfiguration
description: 创建新的 windowsOfficeClientSecurityConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b52cd6ac3f5eb58be38ee45413fe234ed654923c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991963"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a>创建 windowsOfficeClientSecurityConfiguration

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象的 JSON 表示形式。

下表显示时创建[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Office 客户端配置策略的 id。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Stream|首选项设置为 JSON 字符串以二进制格式，用户可以重写这些值。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Stream|策略设置 JSON 字符串以二进制格式，不能由用户更改这些值。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|说明|字符串|管理员提供的 office 客户端的说明配置策略。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|字符串|管理员提供的 office 客户端配置策略的名称。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|assignments|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合|策略的组分配列表正在 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|priority|Int32|优先级值应为每个策略下租户的唯一值并将用于指定在冲突解决，较低值意味着很高的优先级。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|日期时间|上次修改日期时间戳的策略。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|用户签入的摘要策略。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合|Office 客户端中签入状态的列表。 继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|




## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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
HTTP/1.1 201 Created
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



