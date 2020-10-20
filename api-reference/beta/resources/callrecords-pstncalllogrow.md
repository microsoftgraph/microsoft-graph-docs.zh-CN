---
title: pstnCallLogRow 资源类型
description: 表示公共交换机电话网络 (PSTN) 呼叫日志中的数据行。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bc83f3304eeb918d665b2651fda9809fd8a05880
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601669"
---
# <a name="pstncalllogrow-resource-type"></a>pstnCallLogRow 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示公共交换机电话网络 (PSTN) 呼叫日志中的数据行。 每行都映射到一个调用。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一的呼叫标识符。 Containerparentjob.|
|callId|String|呼叫标识符。 不保证是唯一的。|
|userId|String|在 Graph 中调用用户的 ID。 Containerparentjob. 对于 bot 呼叫类型 (ucap_in ucap_out) ，此信息和其他用户信息将为 null/空。|
|userPrincipalName|String|在 Azure Active Directory 中) 的 UserPrincipalName (登录名。 这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。|
|userDisplayName|String|用户的显示名称。|
|startDateTime|DateTimeOffset|呼叫开始时间。|
|endDateTime|DateTimeOffset|呼叫结束时间。|
|duration|Int32|呼叫的连接时间，以秒为单位。|
|帐|双精度|向您的帐户收取的通话的金额或成本。|
|callType|String|呼叫是 PSTN 出站呼叫还是入站呼叫，例如用户发出的呼叫或音频会议的呼叫类型。|
|currency|String|用于计算 ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)) 的呼叫成本的货币类型。|
|calleeNumber|String|以 [164](https://en.wikipedia.org/wiki/E.164) 格式拨打的号码。|
|usageCountryCode|String|用户的国家/地区代码， [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。|
|tenantCountryCode|String|租户的国家/地区代码， [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。|
|connectionCharge|双精度|连接费价格。|
|callerNumber|String|为入站呼叫接收呼叫或拨打出站呼叫的电话号码的号码。 . 164 格式。|
|destinationContext|String|呼叫是否为国家或地区内 () 或国际 (之外的国家或地区) 基于用户的位置。|
|destinationName|String|拨打的国家或地区。|
|conferenceId|String|音频会议的 ID。|
|licenseCapability|String|用于呼叫的许可证。|
|inventoryType|String|用户的电话号码类型，如免费电话号码的服务。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "baseType": "",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.pstnCallLogRow",
  "id": "String (identifier)",
  "callId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "duration": "Integer",
  "charge": "Double",
  "callType": "String",
  "currency": "String",
  "calleeNumber": "String",
  "usageCountryCode": "String",
  "tenantCountryCode": "String",
  "connectionCharge": "Double",
  "callerNumber": "String",
  "destinationContext": "String",
  "destinationName": "String",
  "conferenceId": "String",
  "licenseCapability": "String",
  "inventoryType": "String"
}
```


