---
title: teamsTab 资源类型
description: 'TeamsTab 是一个固定在团队中的频道 (附加) 的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa675992401c8953b5611739ba69cb0d5688f833
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606949"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="cd886-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd886-103">teamsTab resource type</span></span>

<span data-ttu-id="cd886-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd886-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd886-105">TeamsTab 是一个固定在[团队](team.md)中的[频道](channel.md) (附加) 的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="cd886-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="cd886-106">方法</span><span class="sxs-lookup"><span data-stu-id="cd886-106">Methods</span></span>

| <span data-ttu-id="cd886-107">方法</span><span class="sxs-lookup"><span data-stu-id="cd886-107">Method</span></span>       | <span data-ttu-id="cd886-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd886-108">Return Type</span></span>  |<span data-ttu-id="cd886-109">Description</span><span class="sxs-lookup"><span data-stu-id="cd886-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd886-110">通道中的列表选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-110">List tabs in channel</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="cd886-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-112">固定到频道的列表选项卡。</span><span class="sxs-lookup"><span data-stu-id="cd886-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="cd886-113">通道中的获取选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-113">Get tab in channel</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="cd886-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-115">获取固定到频道的特定选项卡。</span><span class="sxs-lookup"><span data-stu-id="cd886-115">Get a specific tab pinned to a channel.</span></span>|
|[<span data-ttu-id="cd886-116">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="cd886-116">Add tab to channel</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="cd886-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-118">将选项卡 (插) 到频道。</span><span class="sxs-lookup"><span data-stu-id="cd886-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="cd886-119">通道中的 "更新" 选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-119">Update tab in channel</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="cd886-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-121">更新通道中的选项卡的属性。</span><span class="sxs-lookup"><span data-stu-id="cd886-121">Updates the properties of a tab in a channel.</span></span>|
|[<span data-ttu-id="cd886-122">从频道中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-122">Remove tab from channel</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="cd886-123">无</span><span class="sxs-lookup"><span data-stu-id="cd886-123">None</span></span> | <span data-ttu-id="cd886-124">从频道) 选项卡中删除 ("取消固定"。</span><span class="sxs-lookup"><span data-stu-id="cd886-124">Remove (unpin) a tab from a channel.</span></span>|
|[<span data-ttu-id="cd886-125">聊天中的列表选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-125">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="cd886-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-126">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-127">固定到聊天的列表选项卡。</span><span class="sxs-lookup"><span data-stu-id="cd886-127">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="cd886-128">聊天中的 "获取" 选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-128">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="cd886-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-129">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-130">获取固定到聊天的特定选项卡。</span><span class="sxs-lookup"><span data-stu-id="cd886-130">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="cd886-131">将选项卡添加到聊天</span><span class="sxs-lookup"><span data-stu-id="cd886-131">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="cd886-132">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-132">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-133">向聊天添加 (pin) 选项卡。</span><span class="sxs-lookup"><span data-stu-id="cd886-133">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="cd886-134">聊天中的更新选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-134">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="cd886-135">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd886-135">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cd886-136">更新聊天中的选项卡的属性。</span><span class="sxs-lookup"><span data-stu-id="cd886-136">Updates the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="cd886-137">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="cd886-137">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="cd886-138">无</span><span class="sxs-lookup"><span data-stu-id="cd886-138">None</span></span> | <span data-ttu-id="cd886-139">) 聊天中的选项卡删除 (的 "取消固定"。</span><span class="sxs-lookup"><span data-stu-id="cd886-139">Remove (unpin) a tab from a chat.</span></span>|



## <a name="properties"></a><span data-ttu-id="cd886-140">属性</span><span class="sxs-lookup"><span data-stu-id="cd886-140">Properties</span></span>

|<span data-ttu-id="cd886-141">属性</span><span class="sxs-lookup"><span data-stu-id="cd886-141">Property</span></span>|<span data-ttu-id="cd886-142">类型</span><span class="sxs-lookup"><span data-stu-id="cd886-142">Type</span></span>|<span data-ttu-id="cd886-143">说明</span><span class="sxs-lookup"><span data-stu-id="cd886-143">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="cd886-144">id</span><span class="sxs-lookup"><span data-stu-id="cd886-144">id</span></span>              |   <span data-ttu-id="cd886-145">string</span><span class="sxs-lookup"><span data-stu-id="cd886-145">string</span></span>                  |  <span data-ttu-id="cd886-146">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cd886-146">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="cd886-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cd886-147">displayName</span></span>            |   <span data-ttu-id="cd886-148">string</span><span class="sxs-lookup"><span data-stu-id="cd886-148">string</span></span>                  |  <span data-ttu-id="cd886-149">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="cd886-149">Name of the tab.</span></span>     |
|  <span data-ttu-id="cd886-150">名称 (弃用) </span><span class="sxs-lookup"><span data-stu-id="cd886-150">name (deprecated)</span></span>      |   <span data-ttu-id="cd886-151">string</span><span class="sxs-lookup"><span data-stu-id="cd886-151">string</span></span>                  |  <span data-ttu-id="cd886-152">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="cd886-152">Name of the tab.</span></span>     |
|  <span data-ttu-id="cd886-153">teamsAppId (弃用) </span><span class="sxs-lookup"><span data-stu-id="cd886-153">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="cd886-154">string</span><span class="sxs-lookup"><span data-stu-id="cd886-154">string</span></span>             |  <span data-ttu-id="cd886-155">选项卡的应用程序定义标识符。创建选项卡后，不能更改此值。</span><span class="sxs-lookup"><span data-stu-id="cd886-155">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="cd886-156">由于此属性已弃用，因此我们建议扩展 **teamsApp** 以检索链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="cd886-156">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="cd886-157">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="cd886-157">sortOrderIndex</span></span>  |   <span data-ttu-id="cd886-158">string</span><span class="sxs-lookup"><span data-stu-id="cd886-158">string</span></span>                  |  <span data-ttu-id="cd886-159">用于对选项卡进行排序的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="cd886-159">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="cd886-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="cd886-160">webUrl</span></span>          |   <span data-ttu-id="cd886-161">string</span><span class="sxs-lookup"><span data-stu-id="cd886-161">string</span></span>                  |  <span data-ttu-id="cd886-162">选项卡实例的深层链接 URL。</span><span class="sxs-lookup"><span data-stu-id="cd886-162">Deep link URL of the tab instance.</span></span> <span data-ttu-id="cd886-163">只读。</span><span class="sxs-lookup"><span data-stu-id="cd886-163">Read only.</span></span>     |
|  <span data-ttu-id="cd886-164">configuration</span><span class="sxs-lookup"><span data-stu-id="cd886-164">configuration</span></span>        |   [<span data-ttu-id="cd886-165">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd886-165">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="cd886-166">应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="cd886-166">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="cd886-167">关系</span><span class="sxs-lookup"><span data-stu-id="cd886-167">Relationships</span></span>

| <span data-ttu-id="cd886-168">关系</span><span class="sxs-lookup"><span data-stu-id="cd886-168">Relationship</span></span> | <span data-ttu-id="cd886-169">类型</span><span class="sxs-lookup"><span data-stu-id="cd886-169">Type</span></span>   | <span data-ttu-id="cd886-170">Description</span><span class="sxs-lookup"><span data-stu-id="cd886-170">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cd886-171">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cd886-171">teamsApp</span></span>|[<span data-ttu-id="cd886-172">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cd886-172">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="cd886-173">链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="cd886-173">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd886-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd886-174">JSON representation</span></span>

<span data-ttu-id="cd886-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd886-175">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="cd886-176">另请参阅</span><span class="sxs-lookup"><span data-stu-id="cd886-176">See also</span></span>

[<span data-ttu-id="cd886-177">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="cd886-177">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


