---
title: participantJoiningNotification 资源类型
description: 包含有关加入呼叫的基于策略的参与者的详细信息。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a0067f5632e34a30da7f6f4ec2e8df70995fa88
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446639"
---
# <a name="participantjoiningnotification-resource-type"></a><span data-ttu-id="649a8-103">participantJoiningNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="649a8-103">participantJoiningNotification resource type</span></span>

<span data-ttu-id="649a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="649a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="649a8-105">包含有关加入呼叫的基于策略的参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="649a8-105">Contains details about the policy-based participant joining a call.</span></span>

<span data-ttu-id="649a8-106">在基于 [策略的](/microsoftteams/teams-recording-policy)录制方案中，在策略下的参与者加入呼叫之前，会向与具有处理新参与者能力的策略关联的自动程序 `participantJoiningNotification` 发送 a。</span><span class="sxs-lookup"><span data-stu-id="649a8-106">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under the policy joins a call, a `participantJoiningNotification` will be sent to the bot associated with the policy that has available capacity to handle the new participant.</span></span>

<span data-ttu-id="649a8-107">响应 [负载中的 participantJoiningResponse](participantjoiningResponse.md) 应来自机器人。</span><span class="sxs-lookup"><span data-stu-id="649a8-107">A [participantJoiningResponse](participantjoiningResponse.md) in the response payload is expected from the bot.</span></span>

## <a name="properties"></a><span data-ttu-id="649a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="649a8-108">Properties</span></span>
| <span data-ttu-id="649a8-109">属性</span><span class="sxs-lookup"><span data-stu-id="649a8-109">Property</span></span>       | <span data-ttu-id="649a8-110">类型</span><span class="sxs-lookup"><span data-stu-id="649a8-110">Type</span></span>            | <span data-ttu-id="649a8-111">说明</span><span class="sxs-lookup"><span data-stu-id="649a8-111">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="649a8-112">通话</span><span class="sxs-lookup"><span data-stu-id="649a8-112">call</span></span>           | [<span data-ttu-id="649a8-113">call</span><span class="sxs-lookup"><span data-stu-id="649a8-113">call</span></span>](call.md) | <span data-ttu-id="649a8-114">包含有关参与者加入事件的详细信息的调用对象。</span><span class="sxs-lookup"><span data-stu-id="649a8-114">The call object that contains details about the participant joining event.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="649a8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="649a8-115">JSON representation</span></span>

<span data-ttu-id="649a8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="649a8-116">The following is a JSON representation of the resource.</span></span>

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

