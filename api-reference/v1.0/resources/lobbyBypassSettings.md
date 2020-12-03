---
title: lobbyBypassSettings 资源类型
description: 指定哪些参与者可以绕过会议厅。
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 761a45ce5c4e29d06287edb18aa8d79256c08923
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523159"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="ac3dc-103">lobbyBypassSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac3dc-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="ac3dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac3dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac3dc-105">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="ac3dc-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac3dc-106">Properties</span></span>

| <span data-ttu-id="ac3dc-107">属性</span><span class="sxs-lookup"><span data-stu-id="ac3dc-107">Property</span></span>              | <span data-ttu-id="ac3dc-108">类型</span><span class="sxs-lookup"><span data-stu-id="ac3dc-108">Type</span></span>             | <span data-ttu-id="ac3dc-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac3dc-109">Description</span></span>                                                                                                                                                          |
| --------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ac3dc-110">scope</span><span class="sxs-lookup"><span data-stu-id="ac3dc-110">scope</span></span>                 | <span data-ttu-id="ac3dc-111">lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="ac3dc-111">lobbyBypassScope</span></span> | <span data-ttu-id="ac3dc-112">指定自动获准加入会议的参与者的类型（绕会议厅）。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="ac3dc-113">下表中列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="ac3dc-114">可选。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-114">Optional.</span></span> |
| <span data-ttu-id="ac3dc-115">isDialInBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="ac3dc-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="ac3dc-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="ac3dc-116">Boolean</span></span>          | <span data-ttu-id="ac3dc-117">指定是否始终让拨入呼叫者绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="ac3dc-118">可选。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-118">Optional.</span></span>                                                                                   |

### <a name="lobbybypassscope-values"></a><span data-ttu-id="ac3dc-119">lobbyBypassScope 值</span><span class="sxs-lookup"><span data-stu-id="ac3dc-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="ac3dc-120">值</span><span class="sxs-lookup"><span data-stu-id="ac3dc-120">Value</span></span>                    | <span data-ttu-id="ac3dc-121">说明</span><span class="sxs-lookup"><span data-stu-id="ac3dc-121">Description</span></span>                                                                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ac3dc-122">组织者</span><span class="sxs-lookup"><span data-stu-id="ac3dc-122">organizer</span></span>                | <span data-ttu-id="ac3dc-123">绕过会议厅，仅允许组织者进入会议。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="ac3dc-124">所有其他参与者都将放入会议厅中。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-124">All other participants are placed in the meeting lobby.</span></span>                                                   |
| <span data-ttu-id="ac3dc-125">组织</span><span class="sxs-lookup"><span data-stu-id="ac3dc-125">organization</span></span>             | <span data-ttu-id="ac3dc-126">只有来自同一公司的参与者才会绕过大厅获准参加会议。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="ac3dc-127">所有其他参与者都将放入会议厅中。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-127">All other participants are placed in the meeting lobby.</span></span>                         |
| <span data-ttu-id="ac3dc-128">organizationAndFederated</span><span class="sxs-lookup"><span data-stu-id="ac3dc-128">organizationAndFederated</span></span> | <span data-ttu-id="ac3dc-129">只有来自同一家公司或受信任组织的参与者才会被允许加入会议，从而绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="ac3dc-130">所有其他参与者都将放入会议厅中。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="ac3dc-131">成员</span><span class="sxs-lookup"><span data-stu-id="ac3dc-131">everyone</span></span>                 | <span data-ttu-id="ac3dc-132">允许所有人参加会议。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="ac3dc-133">不会在会议厅中放置任何参与者。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-133">No participants are placed in the meeting lobby.</span></span>                                                                                         |
| <span data-ttu-id="ac3dc-134">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="ac3dc-134">unknownFutureValue</span></span>       | <span data-ttu-id="ac3dc-135">Unknow 未来值。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-135">Unknow future value.</span></span>                                                                                                                                                            |

## <a name="json-representation"></a><span data-ttu-id="ac3dc-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac3dc-136">JSON representation</span></span>

<span data-ttu-id="ac3dc-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac3dc-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "String",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
