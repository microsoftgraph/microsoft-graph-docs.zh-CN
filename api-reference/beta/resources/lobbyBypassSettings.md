---
title: lobbyBypassSettings 资源类型
description: 指定哪些参与者可以绕过会议厅。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c6d530765e1bc356486f0b8893c69c445c07181f
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896681"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="d718e-103">lobbyBypassSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d718e-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="d718e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d718e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d718e-105">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="d718e-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="d718e-106">属性</span><span class="sxs-lookup"><span data-stu-id="d718e-106">Properties</span></span>

| <span data-ttu-id="d718e-107">属性</span><span class="sxs-lookup"><span data-stu-id="d718e-107">Property</span></span>              | <span data-ttu-id="d718e-108">类型</span><span class="sxs-lookup"><span data-stu-id="d718e-108">Type</span></span>    | <span data-ttu-id="d718e-109">说明</span><span class="sxs-lookup"><span data-stu-id="d718e-109">Description</span></span>                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| <span data-ttu-id="d718e-110">scope</span><span class="sxs-lookup"><span data-stu-id="d718e-110">scope</span></span>                 | [<span data-ttu-id="d718e-111">lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="d718e-111">lobbyBypassScope</span></span>](#lobbybypassscope-values)  | <span data-ttu-id="d718e-112">指定自动获准加入会议、绕过会议厅的参与者类型。</span><span class="sxs-lookup"><span data-stu-id="d718e-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="d718e-113">下表列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="d718e-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="d718e-114">可选。</span><span class="sxs-lookup"><span data-stu-id="d718e-114">Optional.</span></span>|
| <span data-ttu-id="d718e-115">isDialInBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="d718e-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="d718e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d718e-116">Boolean</span></span> | <span data-ttu-id="d718e-117">指定是否始终允许拨入呼叫者绕过大厅。</span><span class="sxs-lookup"><span data-stu-id="d718e-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="d718e-118">可选。</span><span class="sxs-lookup"><span data-stu-id="d718e-118">Optional.</span></span> | 

### <a name="lobbybypassscope-values"></a><span data-ttu-id="d718e-119">lobbyBypassScope 值</span><span class="sxs-lookup"><span data-stu-id="d718e-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="d718e-120">值</span><span class="sxs-lookup"><span data-stu-id="d718e-120">Value</span></span>                    | <span data-ttu-id="d718e-121">说明</span><span class="sxs-lookup"><span data-stu-id="d718e-121">Description</span></span>                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d718e-122">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="d718e-122">organizer</span></span>                | <span data-ttu-id="d718e-123">仅组织者可以进入会议，绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="d718e-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="d718e-124">所有其他参与者都放置在会议厅中。</span><span class="sxs-lookup"><span data-stu-id="d718e-124">All other participants are placed in the meeting lobby.</span></span>                                                                                                         |
| <span data-ttu-id="d718e-125">组织</span><span class="sxs-lookup"><span data-stu-id="d718e-125">organization</span></span>             | <span data-ttu-id="d718e-126">只有来自同一公司的参与者可以绕过会议厅参加会议。</span><span class="sxs-lookup"><span data-stu-id="d718e-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="d718e-127">所有其他参与者都放置在会议厅中。</span><span class="sxs-lookup"><span data-stu-id="d718e-127">All other participants are placed in the meeting lobby.</span></span>                                                                              |
| <span data-ttu-id="d718e-128">organizationAndFederated</span><span class="sxs-lookup"><span data-stu-id="d718e-128">organizationAndFederated</span></span> | <span data-ttu-id="d718e-129">只有来自同一公司或受信任组织的参与者可以绕过会议厅参加会议。</span><span class="sxs-lookup"><span data-stu-id="d718e-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="d718e-130">所有其他参与者都放置在会议厅中。</span><span class="sxs-lookup"><span data-stu-id="d718e-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="d718e-131">everyone</span><span class="sxs-lookup"><span data-stu-id="d718e-131">everyone</span></span>                 | <span data-ttu-id="d718e-132">每个人都可以参加会议。</span><span class="sxs-lookup"><span data-stu-id="d718e-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="d718e-133">会议厅中不放置任何参与者。</span><span class="sxs-lookup"><span data-stu-id="d718e-133">No participants are placed in the meeting lobby.</span></span>                                                                                                                   |
| <span data-ttu-id="d718e-134">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="d718e-134">unknownFutureValue</span></span>       | <span data-ttu-id="d718e-135">不知情未来值。</span><span class="sxs-lookup"><span data-stu-id="d718e-135">Unknow future value.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="d718e-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d718e-136">JSON representation</span></span>

<span data-ttu-id="d718e-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d718e-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
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
