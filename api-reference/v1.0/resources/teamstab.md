---
title: teamsTab 资源类型
description: 'TeamsTab 是一个固定在团队中的频道 (附加) 的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d81c9f21d04690bcaa7360fb83595a13c7be156
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607026"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="dcc0d-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcc0d-103">teamsTab resource type</span></span>

<span data-ttu-id="dcc0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcc0d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="dcc0d-105">TeamsTab 是一个固定在[团队](team.md)中的[频道](channel.md) (附加) 的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="dcc0d-106">方法</span><span class="sxs-lookup"><span data-stu-id="dcc0d-106">Methods</span></span>

| <span data-ttu-id="dcc0d-107">方法</span><span class="sxs-lookup"><span data-stu-id="dcc0d-107">Method</span></span>       | <span data-ttu-id="dcc0d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dcc0d-108">Return Type</span></span>  |<span data-ttu-id="dcc0d-109">Description</span><span class="sxs-lookup"><span data-stu-id="dcc0d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dcc0d-110">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="dcc0d-110">List tabs</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="dcc0d-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dcc0d-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dcc0d-112">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="dcc0d-113">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="dcc0d-113">Get tab</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="dcc0d-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dcc0d-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dcc0d-115">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="dcc0d-116">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="dcc0d-116">Add tab</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="dcc0d-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dcc0d-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dcc0d-118">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="dcc0d-119">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="dcc0d-119">Update tab</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="dcc0d-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dcc0d-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dcc0d-121">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-121">Updates the tab properties.</span></span>|
|[<span data-ttu-id="dcc0d-122">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="dcc0d-122">Remove tab</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="dcc0d-123">无</span><span class="sxs-lookup"><span data-stu-id="dcc0d-123">None</span></span> | <span data-ttu-id="dcc0d-124">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-124">Removes (unpins) a tab from a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="dcc0d-125">属性</span><span class="sxs-lookup"><span data-stu-id="dcc0d-125">Properties</span></span>

|<span data-ttu-id="dcc0d-126">属性</span><span class="sxs-lookup"><span data-stu-id="dcc0d-126">Property</span></span>|<span data-ttu-id="dcc0d-127">类型</span><span class="sxs-lookup"><span data-stu-id="dcc0d-127">Type</span></span>|<span data-ttu-id="dcc0d-128">说明</span><span class="sxs-lookup"><span data-stu-id="dcc0d-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="dcc0d-129">id</span><span class="sxs-lookup"><span data-stu-id="dcc0d-129">id</span></span>              |   <span data-ttu-id="dcc0d-130">string</span><span class="sxs-lookup"><span data-stu-id="dcc0d-130">string</span></span>                  |  <span data-ttu-id="dcc0d-131">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="dcc0d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dcc0d-132">displayName</span></span>            |   <span data-ttu-id="dcc0d-133">string</span><span class="sxs-lookup"><span data-stu-id="dcc0d-133">string</span></span>                  |  <span data-ttu-id="dcc0d-134">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="dcc0d-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="dcc0d-135">webUrl</span></span>          |   <span data-ttu-id="dcc0d-136">string</span><span class="sxs-lookup"><span data-stu-id="dcc0d-136">string</span></span>                  |  <span data-ttu-id="dcc0d-137">选项卡实例的深层链接 URL。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="dcc0d-138">只读。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-138">Read only.</span></span>     |
|  <span data-ttu-id="dcc0d-139">configuration</span><span class="sxs-lookup"><span data-stu-id="dcc0d-139">configuration</span></span>        |   [<span data-ttu-id="dcc0d-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="dcc0d-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="dcc0d-141">应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="dcc0d-142">关系</span><span class="sxs-lookup"><span data-stu-id="dcc0d-142">Relationships</span></span>

| <span data-ttu-id="dcc0d-143">关系</span><span class="sxs-lookup"><span data-stu-id="dcc0d-143">Relationship</span></span> | <span data-ttu-id="dcc0d-144">类型</span><span class="sxs-lookup"><span data-stu-id="dcc0d-144">Type</span></span>   | <span data-ttu-id="dcc0d-145">Description</span><span class="sxs-lookup"><span data-stu-id="dcc0d-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dcc0d-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dcc0d-146">teamsApp</span></span>|[<span data-ttu-id="dcc0d-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dcc0d-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="dcc0d-148">链接到该选项卡的应用程序。创建选项卡后，不能更改此选项。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dcc0d-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcc0d-149">JSON representation</span></span>

<span data-ttu-id="dcc0d-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcc0d-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="dcc0d-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dcc0d-151">See also</span></span>

[<span data-ttu-id="dcc0d-152">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="dcc0d-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

