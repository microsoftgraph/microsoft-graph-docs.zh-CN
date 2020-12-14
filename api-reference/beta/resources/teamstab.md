---
title: teamsTab 资源类型
description: 'teamsTab 是固定到团队 () 频道的选项卡。 '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 38351b0bde174b03f0e01392e7c8ec9c4df0db44
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660112"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="64f33-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="64f33-103">teamsTab resource type</span></span>

<span data-ttu-id="64f33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f33-105">teamsTab[是固定](../resources/teamstab.md)到团队 () 频道的[](channel.md)[选项卡](team.md)。</span><span class="sxs-lookup"><span data-stu-id="64f33-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="64f33-106">方法</span><span class="sxs-lookup"><span data-stu-id="64f33-106">Methods</span></span>

| <span data-ttu-id="64f33-107">方法</span><span class="sxs-lookup"><span data-stu-id="64f33-107">Method</span></span>       | <span data-ttu-id="64f33-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="64f33-108">Return Type</span></span>  |<span data-ttu-id="64f33-109">说明</span><span class="sxs-lookup"><span data-stu-id="64f33-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64f33-110">列出频道中的选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-110">List tabs in channel</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="64f33-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-112">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="64f33-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="64f33-113">获取频道中的选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-113">Get tab in channel</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="64f33-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-115">获取固定到频道的特定选项卡。</span><span class="sxs-lookup"><span data-stu-id="64f33-115">Get a specific tab pinned to a channel.</span></span>|
|[<span data-ttu-id="64f33-116">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="64f33-116">Add tab to channel</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="64f33-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-118">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="64f33-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="64f33-119">更新频道中的选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-119">Update tab in channel</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="64f33-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-121">更新频道中的选项卡的属性。</span><span class="sxs-lookup"><span data-stu-id="64f33-121">Updates the properties of a tab in a channel.</span></span>|
|[<span data-ttu-id="64f33-122">从频道中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-122">Remove tab from channel</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="64f33-123">无</span><span class="sxs-lookup"><span data-stu-id="64f33-123">None</span></span> | <span data-ttu-id="64f33-124">从频道中删除（取消固定）选项卡。</span><span class="sxs-lookup"><span data-stu-id="64f33-124">Remove (unpin) a tab from a channel.</span></span>|
|[<span data-ttu-id="64f33-125">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-125">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="64f33-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-126">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-127">列出固定到聊天的选项卡。</span><span class="sxs-lookup"><span data-stu-id="64f33-127">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="64f33-128">获取聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-128">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="64f33-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-129">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-130">获取固定到聊天的特定选项卡。</span><span class="sxs-lookup"><span data-stu-id="64f33-130">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="64f33-131">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-131">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="64f33-132">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-132">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-133">将 (固定) 选项卡添加到聊天中。</span><span class="sxs-lookup"><span data-stu-id="64f33-133">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="64f33-134">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-134">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="64f33-135">teamsTab</span><span class="sxs-lookup"><span data-stu-id="64f33-135">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="64f33-136">更新聊天中选项卡的属性。</span><span class="sxs-lookup"><span data-stu-id="64f33-136">Update the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="64f33-137">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="64f33-137">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="64f33-138">无</span><span class="sxs-lookup"><span data-stu-id="64f33-138">None</span></span> | <span data-ttu-id="64f33-139">从 (选项卡) 取消固定。</span><span class="sxs-lookup"><span data-stu-id="64f33-139">Remove (unpin) a tab from a chat.</span></span>|



## <a name="properties"></a><span data-ttu-id="64f33-140">属性</span><span class="sxs-lookup"><span data-stu-id="64f33-140">Properties</span></span>

|<span data-ttu-id="64f33-141">属性</span><span class="sxs-lookup"><span data-stu-id="64f33-141">Property</span></span>|<span data-ttu-id="64f33-142">类型</span><span class="sxs-lookup"><span data-stu-id="64f33-142">Type</span></span>|<span data-ttu-id="64f33-143">说明</span><span class="sxs-lookup"><span data-stu-id="64f33-143">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="64f33-144">id</span><span class="sxs-lookup"><span data-stu-id="64f33-144">id</span></span>              |   <span data-ttu-id="64f33-145">string</span><span class="sxs-lookup"><span data-stu-id="64f33-145">string</span></span>                  |  <span data-ttu-id="64f33-146">唯一标识通道选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="64f33-146">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="64f33-147">displayName</span><span class="sxs-lookup"><span data-stu-id="64f33-147">displayName</span></span>            |   <span data-ttu-id="64f33-148">string</span><span class="sxs-lookup"><span data-stu-id="64f33-148">string</span></span>                  |  <span data-ttu-id="64f33-149">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="64f33-149">Name of the tab.</span></span>     |
|  <span data-ttu-id="64f33-150">名称 (已弃) </span><span class="sxs-lookup"><span data-stu-id="64f33-150">name (deprecated)</span></span>      |   <span data-ttu-id="64f33-151">string</span><span class="sxs-lookup"><span data-stu-id="64f33-151">string</span></span>                  |  <span data-ttu-id="64f33-152">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="64f33-152">Name of the tab.</span></span>     |
|  <span data-ttu-id="64f33-153">teamsAppId (已弃用) </span><span class="sxs-lookup"><span data-stu-id="64f33-153">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="64f33-154">string</span><span class="sxs-lookup"><span data-stu-id="64f33-154">string</span></span>             |  <span data-ttu-id="64f33-155">选项卡的应用定义标识符。创建选项卡后无法更改此值。</span><span class="sxs-lookup"><span data-stu-id="64f33-155">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="64f33-156">由于此属性已弃用，我们建议扩展 **teamsApp** 以检索链接到选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="64f33-156">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="64f33-157">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="64f33-157">sortOrderIndex</span></span>  |   <span data-ttu-id="64f33-158">string</span><span class="sxs-lookup"><span data-stu-id="64f33-158">string</span></span>                  |  <span data-ttu-id="64f33-159">用于对选项卡进行排序的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="64f33-159">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="64f33-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="64f33-160">webUrl</span></span>          |   <span data-ttu-id="64f33-161">string</span><span class="sxs-lookup"><span data-stu-id="64f33-161">string</span></span>                  |  <span data-ttu-id="64f33-162">选项卡实例的深层链接 URL。</span><span class="sxs-lookup"><span data-stu-id="64f33-162">Deep link URL of the tab instance.</span></span> <span data-ttu-id="64f33-163">只读。</span><span class="sxs-lookup"><span data-stu-id="64f33-163">Read only.</span></span>     |
|  <span data-ttu-id="64f33-164">configuration</span><span class="sxs-lookup"><span data-stu-id="64f33-164">configuration</span></span>        |   [<span data-ttu-id="64f33-165">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="64f33-165">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="64f33-166">应用于选项卡的自定义设置的容器。只有在设置此属性后，选项卡才被视为已配置。</span><span class="sxs-lookup"><span data-stu-id="64f33-166">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="64f33-167">关系</span><span class="sxs-lookup"><span data-stu-id="64f33-167">Relationships</span></span>

| <span data-ttu-id="64f33-168">关系</span><span class="sxs-lookup"><span data-stu-id="64f33-168">Relationship</span></span> | <span data-ttu-id="64f33-169">类型</span><span class="sxs-lookup"><span data-stu-id="64f33-169">Type</span></span>   | <span data-ttu-id="64f33-170">说明</span><span class="sxs-lookup"><span data-stu-id="64f33-170">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="64f33-171">teamsApp</span><span class="sxs-lookup"><span data-stu-id="64f33-171">teamsApp</span></span>|[<span data-ttu-id="64f33-172">teamsApp</span><span class="sxs-lookup"><span data-stu-id="64f33-172">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="64f33-173">链接到选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="64f33-173">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64f33-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64f33-174">JSON representation</span></span>

<span data-ttu-id="64f33-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64f33-175">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration": "teamsTabConfiguration",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="64f33-176">另请参阅</span><span class="sxs-lookup"><span data-stu-id="64f33-176">See also</span></span>

[<span data-ttu-id="64f33-177">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="64f33-177">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


