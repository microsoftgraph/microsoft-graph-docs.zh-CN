---
title: participantJoiningNotification 资源类型
description: 包含有关加入呼叫的基于策略的参与者的详细信息。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e915697ba01e8968d7833e8701eaf1914984c28f
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430831"
---
# <a name="participantjoiningnotification-resource-type"></a><span data-ttu-id="28cea-103">participantJoiningNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="28cea-103">participantJoiningNotification resource type</span></span>

<span data-ttu-id="28cea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28cea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28cea-105">包含有关加入呼叫的基于策略的参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="28cea-105">Contains details about the policy-based participant joining a call.</span></span>

<span data-ttu-id="28cea-106">在基于 [策略](/microsoftteams/teams-recording-policy)的录制方案下，在策略下的参与者加入呼叫之前，会向与具有处理新参与者的可用容量的策略关联的自动程序 `participantJoiningNotification` 发送 。</span><span class="sxs-lookup"><span data-stu-id="28cea-106">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under the policy joins a call, a `participantJoiningNotification` will be sent to the bot associated with the policy that has available capacity to handle the new participant.</span></span>

<span data-ttu-id="28cea-107">响应 [负载中的 participantJoiningResponse](participantjoiningResponse.md) 应来自机器人。</span><span class="sxs-lookup"><span data-stu-id="28cea-107">A [participantJoiningResponse](participantjoiningResponse.md) in the response payload is expected from the bot.</span></span>

## <a name="properties"></a><span data-ttu-id="28cea-108">属性</span><span class="sxs-lookup"><span data-stu-id="28cea-108">Properties</span></span>
| <span data-ttu-id="28cea-109">属性</span><span class="sxs-lookup"><span data-stu-id="28cea-109">Property</span></span>       | <span data-ttu-id="28cea-110">类型</span><span class="sxs-lookup"><span data-stu-id="28cea-110">Type</span></span>            | <span data-ttu-id="28cea-111">说明</span><span class="sxs-lookup"><span data-stu-id="28cea-111">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="28cea-112">通话</span><span class="sxs-lookup"><span data-stu-id="28cea-112">call</span></span>           | [<span data-ttu-id="28cea-113">call</span><span class="sxs-lookup"><span data-stu-id="28cea-113">call</span></span>](call.md) | <span data-ttu-id="28cea-114">包含有关参与者加入事件的详细信息的 call 对象。</span><span class="sxs-lookup"><span data-stu-id="28cea-114">The call object that contains details about the participant joining event.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28cea-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28cea-115">JSON representation</span></span>

<span data-ttu-id="28cea-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28cea-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantJoiningNotification"
}-->
```json
{
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
