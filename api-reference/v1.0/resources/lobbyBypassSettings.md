---
title: lobbyBypassSettings 资源类型
description: 指定哪些参与者可以绕过会议厅。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: afd51167179d85706b76c0888f9ee745c7f8b3a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959275"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="6bfde-103">lobbyBypassSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bfde-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="6bfde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfde-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6bfde-105">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="6bfde-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="6bfde-106">属性</span><span class="sxs-lookup"><span data-stu-id="6bfde-106">Properties</span></span>

| <span data-ttu-id="6bfde-107">属性</span><span class="sxs-lookup"><span data-stu-id="6bfde-107">Property</span></span>              | <span data-ttu-id="6bfde-108">类型</span><span class="sxs-lookup"><span data-stu-id="6bfde-108">Type</span></span>             | <span data-ttu-id="6bfde-109">说明</span><span class="sxs-lookup"><span data-stu-id="6bfde-109">Description</span></span>                                                                                                                                                          |
| --------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6bfde-110">scope</span><span class="sxs-lookup"><span data-stu-id="6bfde-110">scope</span></span>                 | [<span data-ttu-id="6bfde-111">lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="6bfde-111">lobbyBypassScope</span></span>](#lobbybypassscope-values) | <span data-ttu-id="6bfde-112">指定自动获准加入会议、绕过会议厅的参与者类型。</span><span class="sxs-lookup"><span data-stu-id="6bfde-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="6bfde-113">下表列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="6bfde-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="6bfde-114">可选。</span><span class="sxs-lookup"><span data-stu-id="6bfde-114">Optional.</span></span> |
| <span data-ttu-id="6bfde-115">isDialInBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="6bfde-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="6bfde-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bfde-116">Boolean</span></span>          | <span data-ttu-id="6bfde-117">指定是否始终允许拨入呼叫者绕过大厅。</span><span class="sxs-lookup"><span data-stu-id="6bfde-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="6bfde-118">可选。</span><span class="sxs-lookup"><span data-stu-id="6bfde-118">Optional.</span></span>                                                                                   |

### <a name="lobbybypassscope-values"></a><span data-ttu-id="6bfde-119">lobbyBypassScope 值</span><span class="sxs-lookup"><span data-stu-id="6bfde-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="6bfde-120">值</span><span class="sxs-lookup"><span data-stu-id="6bfde-120">Value</span></span>                    | <span data-ttu-id="6bfde-121">说明</span><span class="sxs-lookup"><span data-stu-id="6bfde-121">Description</span></span>                                                                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6bfde-122">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="6bfde-122">organizer</span></span>                | <span data-ttu-id="6bfde-123">仅组织者可以进入会议，绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="6bfde-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="6bfde-124">所有其他参与者都放置在会议厅中。</span><span class="sxs-lookup"><span data-stu-id="6bfde-124">All other participants are placed in the meeting lobby.</span></span>                                                   |
| <span data-ttu-id="6bfde-125">组织</span><span class="sxs-lookup"><span data-stu-id="6bfde-125">organization</span></span>             | <span data-ttu-id="6bfde-126">只有来自同一公司的参与者可以绕过会议厅参加会议。</span><span class="sxs-lookup"><span data-stu-id="6bfde-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="6bfde-127">所有其他参与者都放置在会议厅中。</span><span class="sxs-lookup"><span data-stu-id="6bfde-127">All other participants are placed in the meeting lobby.</span></span>                         |
| <span data-ttu-id="6bfde-128">organizationAndFederated</span><span class="sxs-lookup"><span data-stu-id="6bfde-128">organizationAndFederated</span></span> | <span data-ttu-id="6bfde-129">只有来自同一公司或受信任组织的参与者可以绕过会议厅参加会议。</span><span class="sxs-lookup"><span data-stu-id="6bfde-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="6bfde-130">所有其他参与者都放置在会议厅中。</span><span class="sxs-lookup"><span data-stu-id="6bfde-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="6bfde-131">everyone</span><span class="sxs-lookup"><span data-stu-id="6bfde-131">everyone</span></span>                 | <span data-ttu-id="6bfde-132">每个人都可以参加会议。</span><span class="sxs-lookup"><span data-stu-id="6bfde-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="6bfde-133">会议厅中不放置任何参与者。</span><span class="sxs-lookup"><span data-stu-id="6bfde-133">No participants are placed in the meeting lobby.</span></span>                                                                                         |
| <span data-ttu-id="6bfde-134">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="6bfde-134">unknownFutureValue</span></span>       | <span data-ttu-id="6bfde-135">不知情未来值。</span><span class="sxs-lookup"><span data-stu-id="6bfde-135">Unknow future value.</span></span>                                                                                                                                                            |

## <a name="json-representation"></a><span data-ttu-id="6bfde-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bfde-136">JSON representation</span></span>

<span data-ttu-id="6bfde-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bfde-137">The following is a JSON representation of the resource.</span></span>

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
