---
title: pstnCallLogRow 资源类型
description: 代表公用电话交换网或 PSTN 呼叫日志中 (一) 行。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 584efcd6e320a95dc6e62f59b112d1041535f054
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697170"
---
# <a name="pstncalllogrow-resource-type"></a>pstnCallLogRow 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表公用电话交换网或 PSTN 呼叫日志中 (一) 行。 每行映射到一个调用。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|callDurationSource|pstnCallDurationSource|呼叫持续时间数据源。 如果呼叫通过 Operator Connect 计划使用第三方电信运营商，则运营商可能会提供其自己的呼叫持续时间数据。 在这种情况下，属性值为 `operator` 。 否则，值为 `microsoft` 。|
|calleeNumber|String|以 [E.164 格式拨打的](https://en.wikipedia.org/wiki/E.164) 号码。|
|callerNumber|String|接收入站呼叫呼叫的号码或为出站呼叫拨打的号码。 E.164 格式。|
|callId|String|呼叫标识符。 不保证是唯一的。|
|callType|String|该呼叫是 PSTN 出站呼叫还是入站呼叫以及呼叫类型，例如用户拨打的呼叫还是音频会议呼叫。|
|charge|双精度|向你的帐户收取的呼叫的金额或费用。|
|conferenceId|String|音频会议的 ID。|
|connectionCharge|双精度|连接费用价格。|
|currency|String|用于计算 [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) (开销的货币) 。|
|destinationContext|String|呼叫是国内呼叫 (或地区内) 或 (或地区外部的) 用户位置进行呼叫。|
|destinationName|String|拨打的国家/地区。|
|duration|Int32|呼叫连接时间（以秒表示）。|
|endDateTime|DateTimeOffset|呼叫结束时间。|
|id|String|唯一呼叫标识符。 GUID。|
|inventoryType|String|用户的电话号码类型，如免费电话号码服务。|
|licenseCapability|String|用于呼叫的许可证。|
|operator|String|为此呼叫提供 PSTN 服务的电信运营商。 这可能是 Microsoft，或者可能是通过 Operator Connect Program 的第三 [方运营商](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398)。|
|startDateTime|DateTimeOffset|呼叫开始时间。|
|tenantCountryCode|String|租户的国家/地区代码 [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。|
|usageCountryCode|String|用户的国家/地区代码 [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。|
|userDisplayName|String|用户的显示名称。|
|userId|String|在 Graph 中调用用户 ID。 GUID。 对于自动程序呼叫类型，此信息和其他用户信息将为 null/空 (ucap_in ucap_out) 。|
|userPrincipalName|String|UserPrincipalName (Azure Active Directory) 登录名。 这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
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
  "inventoryType": "String",
  "operator": "String",
  "callDurationSource": "String"
}
```


