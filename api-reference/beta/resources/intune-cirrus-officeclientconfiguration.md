---
title: officeClientConfiguration 资源类型
description: Office 客户端配置。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ddc1846afe96c99b616f28d6c831adca3eae960
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984057"
---
# <a name="officeclientconfiguration-resource-type"></a>officeClientConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Office 客户端配置。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 officeClientConfigurations](../api/intune-cirrus-officeclientconfiguration-list.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合|列出属性和[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象之间的关系。|
|[获取 officeClientConfiguration](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|读取属性和[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象的关系。|
|[assign 操作](../api/intune-cirrus-officeclientconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合|更换所有目标的组策略。|
|[updatePriorities 操作](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|无|更新策略优先级。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Office 客户端配置策略的 id。|
|userPreferencePayload|Stream|首选项设置为 JSON 字符串以二进制格式，用户可以重写这些值。|
|policyPayload|Stream|策略设置 JSON 字符串以二进制格式，不能由用户更改这些值。|
|说明|字符串|尚未记录|
|displayName|字符串|管理员提供的 office 客户端的说明配置策略。|
|lastModifiedDateTime|日期时间|上次修改日期时间戳的策略。|
|priority|Int32|优先级值应为每个策略下租户的唯一值并将用于指定在冲突解决，较低值意味着很高的优先级。|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|用户签入的摘要策略。|
|checkinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合|Office 客户端中签入状态的列表。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合|组策略的工作分配列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```



