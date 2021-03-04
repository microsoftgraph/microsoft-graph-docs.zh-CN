---
title: participantLeftNotification 资源类型
description: 包含有关已离开呼叫的基于策略的参与者的详细信息。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2730cd68e8d7ff6c5c238caeaee91fb4a821c836
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446634"
---
# <a name="participantleftnotification-resource-type"></a><span data-ttu-id="55f7f-103">participantLeftNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="55f7f-103">participantLeftNotification resource type</span></span>

<span data-ttu-id="55f7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55f7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55f7f-105">包含有关已离开呼叫的基于策略的参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="55f7f-105">Contains details about the policy-based participant who has left the call.</span></span>

<span data-ttu-id="55f7f-106">在基于 [策略](/microsoftteams/teams-recording-policy) 的录制方案下，当机器人呼叫管理的参与者离开会议时，系统将会向机器人发送一个通知机器人，告知机器人有关参与者离开事件 `participantLeftNotification` 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="55f7f-106">Under the [Policy-based recording](/microsoftteams/teams-recording-policy) scenario, when a participant who is managed by the bot call has left the meeting, a `participantLeftNotification` will be sent to the bot to notify the bot with details of the participant left event.</span></span>

## <a name="properties"></a><span data-ttu-id="55f7f-107">属性</span><span class="sxs-lookup"><span data-stu-id="55f7f-107">Properties</span></span>
| <span data-ttu-id="55f7f-108">属性</span><span class="sxs-lookup"><span data-stu-id="55f7f-108">Property</span></span>       | <span data-ttu-id="55f7f-109">类型</span><span class="sxs-lookup"><span data-stu-id="55f7f-109">Type</span></span>            | <span data-ttu-id="55f7f-110">说明</span><span class="sxs-lookup"><span data-stu-id="55f7f-110">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="55f7f-111">通话</span><span class="sxs-lookup"><span data-stu-id="55f7f-111">call</span></span>           | [<span data-ttu-id="55f7f-112">call</span><span class="sxs-lookup"><span data-stu-id="55f7f-112">call</span></span>](call.md) | <span data-ttu-id="55f7f-113">包含有关参与者加入事件的详细信息的调用对象。</span><span class="sxs-lookup"><span data-stu-id="55f7f-113">The call object that contains details about the participant joining event.</span></span> |
| <span data-ttu-id="55f7f-114">participantId</span><span class="sxs-lookup"><span data-stu-id="55f7f-114">participantId</span></span>  | <span data-ttu-id="55f7f-115">String</span><span class="sxs-lookup"><span data-stu-id="55f7f-115">String</span></span>          | <span data-ttu-id="55f7f-116">策略下已离开会议的参与者的 ID。</span><span class="sxs-lookup"><span data-stu-id="55f7f-116">ID of the participant under the policy who has left the meeting.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="55f7f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55f7f-117">JSON representation</span></span>

<span data-ttu-id="55f7f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55f7f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantLeftNotification"
}-->
```json
{
  "participantId": "String",
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantLeftNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

