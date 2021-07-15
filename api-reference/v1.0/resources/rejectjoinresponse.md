---
title: rejectJoinResponse 资源类型
description: 包含拒绝尝试加入会议的参与者的响应。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c917b2c5ba0ed273af1c8e89c78b07a80d6c45fc
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53428856"
---
# <a name="rejectjoinresponse-resource-type"></a><span data-ttu-id="8c816-103">rejectJoinResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c816-103">rejectJoinResponse resource type</span></span>

<span data-ttu-id="8c816-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c816-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c816-105">包含拒绝尝试加入会议的参与者的响应。</span><span class="sxs-lookup"><span data-stu-id="8c816-105">Contains a response to reject a participant who tries to join the meeting.</span></span>

<span data-ttu-id="8c816-106">这具有与拒绝使用 [reject-call](../api/call-reject.md) 方法记录传入呼叫通知的策略相同的效果。</span><span class="sxs-lookup"><span data-stu-id="8c816-106">This has the same effect as rejecting a policy recording incoming call notification using the [reject-call](../api/call-reject.md) method.</span></span> <span data-ttu-id="8c816-107">机器人将继续接收新用户加入的参与者加入通知，直到达到其容量。</span><span class="sxs-lookup"><span data-stu-id="8c816-107">The bot will continue to receive a participant joining notification for a new user joining until its capacity has been reached.</span></span>

## <a name="properties"></a><span data-ttu-id="8c816-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c816-108">Properties</span></span>

| <span data-ttu-id="8c816-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c816-109">Property</span></span>         | <span data-ttu-id="8c816-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c816-110">Type</span></span>                            | <span data-ttu-id="8c816-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c816-111">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8c816-112">reason</span><span class="sxs-lookup"><span data-stu-id="8c816-112">reason</span></span>           | <span data-ttu-id="8c816-113">String</span><span class="sxs-lookup"><span data-stu-id="8c816-113">String</span></span>                          | <span data-ttu-id="8c816-114">拒绝原因。</span><span class="sxs-lookup"><span data-stu-id="8c816-114">The rejection reason.</span></span> <span data-ttu-id="8c816-115">可取值为：`None`、`Busy` 和 `Forbidden`。</span><span class="sxs-lookup"><span data-stu-id="8c816-115">Possible values are `None`, `Busy`, and `Forbidden`.</span></span>                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="8c816-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c816-116">JSON representation</span></span>

<span data-ttu-id="8c816-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c816-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.rejectJoinResponse"
}-->
```json
{
  "reason": "None | Busy | Forbidden" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rejectJoinResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
