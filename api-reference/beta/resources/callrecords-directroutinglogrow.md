---
title: directRoutingLogRow 资源类型
description: 表示直接路由呼叫日志中的一行数据。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 21104f3d0812edd2af7918d6b55ff9a2f9013037
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159652"
---
# <a name="directroutinglogrow-resource-type"></a>directRoutingLogRow 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示直接路由呼叫日志中的一行数据。 每行映射到一个调用。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一呼叫标识符。 GUID。|
|correlationId|String|调用 Microsoft 支持时可以使用的呼叫的标识符。 GUID。|
|userId|String|在 Graph 中调用用户 ID。 对于机器人呼叫类型，此信息和其他用户信息将为 null/空。 GUID。|
|userPrincipalName|String|UserPrincipalName (Azure Active Directory) 登录名。 这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。|
|userDisplayName|String|用户的显示名称。|
|startDateTime|DateTimeOffset|呼叫开始时间。<br/>对于失败和未接听的呼叫，这等于邀请或失败时间。|
|inviteDateTime|DateTimeOffset| 发送初始邀请时。|
|failureDateTime|DateTimeOffset| 仅对未完全建立 (失败) 存在。|
|endDateTime|DateTimeOffset| 只有成功建立 (调用) 存在。 呼叫结束的时间。|
|duration|Int32| 呼叫的持续时间（以秒表示）。|
|callType|String| 呼叫类型和方向。|
|successfulCall|布尔| 成功或尝试。|
|callerNumber|String| 进行呼叫的用户或机器人的号码。 [E.164](https://en.wikipedia.org/wiki/E.164) 格式，但可能包括其他数据。|
|calleeNumber|String| 收到呼叫的用户或自动程序的数量。 [E.164](https://en.wikipedia.org/wiki/E.164) 格式，但可能包括其他数据。|
|mediaPathLocation|String| 用于非旁路呼叫中的媒体路径的数据中心。|
|signalingLocation|String| 用于对旁路和非旁路呼叫发出信号的数据中心。|
|finalSipCode|Int32| 结束呼叫的代码[RFC 3261。](https://tools.ietf.org/html/rfc3261)|
|callEndSubReason|Int32| 除了 SIP 代码之外，Microsoft 还有自己的指示特定问题的子代码。|
|finalSipCodePhrase|String| SIP 代码和 Microsoft 子代码的说明。|
|trunkFullyQualifiedDomainName|String| 会话边界控制器的完全限定域名。|
|mediaBypassEnabled|布尔| 指示中继是否已启用媒体旁路。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.directRoutingLogRow",
  "id": "String (identifier)",
  "correlationId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "inviteDateTime": "String (timestamp)",
  "failureDateTime": "String (timestamp)",
  "duration": "Integer",
  "callType": "String",
  "successfulCall": "Boolean",
  "callerNumber": "String",
  "calleeNumber": "String",
  "mediaPathLocation": "String",
  "signalingLocation": "String",
  "finalSipCode": "Integer",
  "callEndSubReason": "Integer",
  "finalSipCodePhrase": "String",
  "trunkFullyQualifiedDomainName": "String",
  "mediaBypassEnabled": "Boolean"
}
```


