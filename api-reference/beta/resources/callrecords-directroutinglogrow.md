---
title: directRoutingLogRow 资源类型
description: 表示直接路由呼叫日志中的数据行。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5baf5768c7cee9e0525373bb4f7139f6a145acb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601196"
---
# <a name="directroutinglogrow-resource-type"></a>directRoutingLogRow 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示直接路由呼叫日志中的数据行。 每行都映射到一个调用。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一的呼叫标识符。 Containerparentjob.|
|correlationId|String|调用 Microsoft 支持时可使用的呼叫的标识符。 Containerparentjob.|
|userId|String|在 Graph 中调用用户的 ID。 对于 bot 呼叫类型，此信息和其他用户信息将为 null/空。 Containerparentjob.|
|userPrincipalName|String|在 Azure Active Directory 中) 的 UserPrincipalName (登录名。 这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。|
|userDisplayName|String|用户的显示名称。|
|startDateTime|DateTimeOffset|呼叫开始时间。<br/>对于失败和未应答的呼叫，这可能等于 "邀请" 或 "失败时间"。|
|inviteDateTime|DateTimeOffset| 发送初始邀请时。|
|failureDateTime|DateTimeOffset| 仅存在失败的 (未完全建立) 调用的情况。|
|endDateTime|DateTimeOffset| 仅存在成功 (完全建立的) 调用的情况。 呼叫结束的时间。|
|duration|Int32| 呼叫的持续时间（以秒为单位）。|
|callType|String| 呼叫类型和方向。|
|successfulCall|布尔| 成功或尝试。|
|callerNumber|String| 发出呼叫的用户或机器人的号码。 E.164[格式，](https://en.wikipedia.org/wiki/E.164)但可能包含其他数据。|
|calleeNumber|String| 接收呼叫的用户或机器人的号码。 E.164[格式，](https://en.wikipedia.org/wiki/E.164)但可能包含其他数据。|
|mediaPathLocation|String| 用于非旁路呼叫中的媒体路径的数据中心。|
|signalingLocation|String| 用于对绕过和非绕过呼叫发出信号的数据中心。|
|finalSipCode|Int32| 调用结束的代码（ [RFC 3261](https://tools.ietf.org/html/rfc3261)）。|
|callEndSubReason|Int32| 除了 SIP 代码之外，Microsoft 还提供了指示特定问题的子代码。|
|finalSipCodePhrase|String| SIP 代码和 Microsoft 子代码的说明。|
|trunkFullyQualifiedDomainName|String| 会话边界控制器的完全限定的域名称。|
|mediaBypassEnabled|布尔| 指示是否为媒体旁路启用了中继。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "baseType": "",
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


