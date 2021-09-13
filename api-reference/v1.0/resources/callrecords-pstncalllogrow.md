---
title: pstnCallLogRow 资源类型
description: 代表公用电话交换网或 PSTN 呼叫日志中 (一) 行。
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2a4d14df3b46e4a31d74b2f3a0cf2e111e7d1bc0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113817"
---
# <a name="pstncalllogrow-resource-type"></a>pstnCallLogRow 资源类型

命名空间：microsoft.graph.callRecords

代表公用电话交换网或 PSTN 呼叫日志中 (一) 行。 每行映射到一个调用。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [getPstnCalls](../api/callrecords-callrecord-getpstncalls.md) | [microsoft.graph.callRecords.pstnCallLogRow 集合](callrecords-pstncalllogrow.md) | 列出 **呼叫记录中的 pstnCallLogRow** 对象。 |

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|callDurationSource|microsoft.graph.callRecords.pstnCallDurationSource|呼叫持续时间数据源。 如果呼叫通过 Operator 连接 程序使用第三方电信运营商，则运营商可能会提供其自己的呼叫持续时间数据。 在这种情况下，属性值为 `operator` 。 否则，值为 `microsoft` 。|
|calleeNumber|String|以 [E.164 格式拨打的](https://en.wikipedia.org/wiki/E.164) 号码。|
|callerNumber|String|接收入站呼叫呼叫的号码或为出站呼叫拨打的号码。 E.164 格式。|
|callId|String|呼叫标识符。 不保证是唯一的。|
|callType|String|该呼叫是 PSTN 出站呼叫还是入站呼叫，以及呼叫类型，如用户拨打的呼叫还是音频会议呼叫。|
|charge|双精度|向你的帐户收取的呼叫的金额或费用。|
|conferenceId|String|音频会议的 ID。|
|connectionCharge|双精度|连接费用价格。|
|currency|String|用于计算 ISO [4217](https://en.wikipedia.org/wiki/ISO_4217) 中呼叫 (的货币) 。|
|destinationContext|String|呼叫是国内呼叫 (或地区) ，还是 (或地区) 或地区以外的国际呼叫。根据用户的位置。|
|destinationName|String|拨打的国家/地区。|
|duration|Int32|呼叫连接时间（以秒表示）。|
|endDateTime|DateTimeOffset|呼叫结束时间。|
|id|String|唯一呼叫标识符。 GUID。|
|inventoryType|String|用户的电话号码类型，如免费电话号码服务。|
|licenseCapability|String|用于呼叫的许可证。|
|operator|String|为此呼叫提供 PSTN 服务的电信运营商。 这可能是 Microsoft，或者可能是通过 Operator 连接[程序的第三方运营商](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398)。|
|startDateTime|DateTimeOffset|呼叫开始时间。|
|tenantCountryCode|String|租户的国家/地区代码 [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。|
|usageCountryCode|String|用户的国家/地区代码 [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。|
|userDisplayName|String|用户的显示名称。|
|userId|String|呼叫用户 ID Graph。 GUID。 对于自动程序呼叫类型，此信息和其他用户信息将为 null/空 (ucap_in ucap_out) 。|
|userPrincipalName|String|UserPrincipalName (中的登录) Azure Active Directory。 这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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


