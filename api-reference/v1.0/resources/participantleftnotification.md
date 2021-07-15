---
title: participantLeftNotification 资源类型
description: 包含有关已离开呼叫的基于策略的参与者的详细信息。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ee2526ceef6aaf377003f6e802093ec103059c06
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430829"
---
# <a name="participantleftnotification-resource-type"></a><span data-ttu-id="1b3bf-103">participantLeftNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b3bf-103">participantLeftNotification resource type</span></span>

<span data-ttu-id="1b3bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b3bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b3bf-105">包含有关已离开呼叫的基于策略的参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1b3bf-105">Contains details about the policy-based participant who has left the call.</span></span>

<span data-ttu-id="1b3bf-106">在基于 [策略的](/microsoftteams/teams-recording-policy) 录制方案中，当由机器人呼叫管理的参与者离开会议时，会向机器人发送 ，以通知机器人有关参与者离开事件 `participantLeftNotification` 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1b3bf-106">Under the [Policy-based recording](/microsoftteams/teams-recording-policy) scenario, when a participant who is managed by the bot call has left the meeting, a `participantLeftNotification` will be sent to the bot to notify the bot with details of the participant left event.</span></span>

## <a name="properties"></a><span data-ttu-id="1b3bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b3bf-107">Properties</span></span>
| <span data-ttu-id="1b3bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b3bf-108">Property</span></span>       | <span data-ttu-id="1b3bf-109">类型</span><span class="sxs-lookup"><span data-stu-id="1b3bf-109">Type</span></span>            | <span data-ttu-id="1b3bf-110">说明</span><span class="sxs-lookup"><span data-stu-id="1b3bf-110">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="1b3bf-111">通话</span><span class="sxs-lookup"><span data-stu-id="1b3bf-111">call</span></span>           | [<span data-ttu-id="1b3bf-112">call</span><span class="sxs-lookup"><span data-stu-id="1b3bf-112">call</span></span>](call.md) | <span data-ttu-id="1b3bf-113">包含有关参与者加入事件的详细信息的 call 对象。</span><span class="sxs-lookup"><span data-stu-id="1b3bf-113">The call object that contains details about the participant joining event.</span></span> |
| <span data-ttu-id="1b3bf-114">participantId</span><span class="sxs-lookup"><span data-stu-id="1b3bf-114">participantId</span></span>  | <span data-ttu-id="1b3bf-115">String</span><span class="sxs-lookup"><span data-stu-id="1b3bf-115">String</span></span>          | <span data-ttu-id="1b3bf-116">已离开会议的策略下的参与者的 ID。</span><span class="sxs-lookup"><span data-stu-id="1b3bf-116">ID of the participant under the policy who has left the meeting.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="1b3bf-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b3bf-117">JSON representation</span></span>

<span data-ttu-id="1b3bf-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b3bf-118">The following is a JSON representation of the resource.</span></span>

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
