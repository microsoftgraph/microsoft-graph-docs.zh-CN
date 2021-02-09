---
title: pstnCallLogRow 资源类型
description: 代表 PSTN 呼叫日志中公用电话交换 (中的) 行。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5103404bdaa6ac4eafbfcffd45deef41c217600a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155578"
---
# <a name="pstncalllogrow-resource-type"></a>pstnCallLogRow 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 PSTN 呼叫日志中公用电话交换 (中的) 行。 每行映射到一个调用。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一呼叫标识符。 GUID。|
|callId|String|呼叫标识符。 不保证是唯一的。|
|userId|String|在 Graph 中调用用户 ID。 GUID。 对于自动程序呼叫类型，此信息和其他用户信息将为 null/ (ucap_in，ucap_out) 。|
|userPrincipalName|String|UserPrincipalName (Azure Active Directory) 登录名。 这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。|
|userDisplayName|String|用户的显示名称。|
|startDateTime|DateTimeOffset|呼叫开始时间。|
|endDateTime|DateTimeOffset|呼叫结束时间。|
|duration|Int32|呼叫连接时间（以秒表示）。|
|charge|双精度|向你的帐户收取的呼叫的金额或费用。|
|callType|String|呼叫是 PSTN 出站呼叫还是入站呼叫以及呼叫类型，例如用户拨打的呼叫或音频会议。|
|currency|String|用于计算 ISO [4217](https://en.wikipedia.org/wiki/ISO_4217) (呼叫成本的货币) 。|
|calleeNumber|String|[E.164 格式](https://en.wikipedia.org/wiki/E.164)拨打的号码。|
|usageCountryCode|String|用户的国家/地区代码[，ISO 3166-1 alpha-2。](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)|
|tenantCountryCode|String|租户的国家/地区代码 [，ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。|
|connectionCharge|双精度|连接费用价格。|
|callerNumber|String|接收入站呼叫呼叫的号码或为出站呼叫拨打的号码。 E.164 格式。|
|destinationContext|String|呼叫是 (国家/地区) ，还是位于 (或) 地理位置之外的国际呼叫。|
|destinationName|String|拨打的国家/地区。|
|conferenceId|String|音频会议的 ID。|
|licenseCapability|String|用于呼叫的许可证。|
|inventoryType|String|用户的电话号码类型，如免费电话号码服务。|

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
  "inventoryType": "String"
}
```


