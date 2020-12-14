---
title: teamsTab 资源类型
description: 'teamsTab 是固定到团队 () 频道的选项卡。 '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8314604d6ed15eeb154ff46c8e3b90f4be4f5cde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658546"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="8570f-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="8570f-103">teamsTab resource type</span></span>

<span data-ttu-id="8570f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8570f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8570f-105">teamsTab[是固定](../resources/teamstab.md)到团队 () 频道的[](channel.md)[选项卡](team.md)。</span><span class="sxs-lookup"><span data-stu-id="8570f-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="8570f-106">方法</span><span class="sxs-lookup"><span data-stu-id="8570f-106">Methods</span></span>

| <span data-ttu-id="8570f-107">方法</span><span class="sxs-lookup"><span data-stu-id="8570f-107">Method</span></span>       | <span data-ttu-id="8570f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8570f-108">Return Type</span></span>  |<span data-ttu-id="8570f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8570f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8570f-110">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="8570f-110">List tabs</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="8570f-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8570f-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8570f-112">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="8570f-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="8570f-113">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="8570f-113">Get tab</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="8570f-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8570f-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8570f-115">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="8570f-115">Read a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="8570f-116">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="8570f-116">Add tab</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="8570f-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8570f-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8570f-118">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="8570f-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="8570f-119">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="8570f-119">Update tab</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="8570f-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8570f-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="8570f-121">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="8570f-121">Update the tab properties.</span></span>|
|[<span data-ttu-id="8570f-122">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="8570f-122">Remove tab</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="8570f-123">无</span><span class="sxs-lookup"><span data-stu-id="8570f-123">None</span></span> | <span data-ttu-id="8570f-124">从频道中删除（取消固定）选项卡。</span><span class="sxs-lookup"><span data-stu-id="8570f-124">Remove (unpin) a tab from a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="8570f-125">属性</span><span class="sxs-lookup"><span data-stu-id="8570f-125">Properties</span></span>

|<span data-ttu-id="8570f-126">属性</span><span class="sxs-lookup"><span data-stu-id="8570f-126">Property</span></span>|<span data-ttu-id="8570f-127">类型</span><span class="sxs-lookup"><span data-stu-id="8570f-127">Type</span></span>|<span data-ttu-id="8570f-128">说明</span><span class="sxs-lookup"><span data-stu-id="8570f-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="8570f-129">id</span><span class="sxs-lookup"><span data-stu-id="8570f-129">id</span></span>              |   <span data-ttu-id="8570f-130">string</span><span class="sxs-lookup"><span data-stu-id="8570f-130">string</span></span>                  |  <span data-ttu-id="8570f-131">唯一标识通道选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8570f-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="8570f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8570f-132">displayName</span></span>            |   <span data-ttu-id="8570f-133">string</span><span class="sxs-lookup"><span data-stu-id="8570f-133">string</span></span>                  |  <span data-ttu-id="8570f-134">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="8570f-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="8570f-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="8570f-135">webUrl</span></span>          |   <span data-ttu-id="8570f-136">string</span><span class="sxs-lookup"><span data-stu-id="8570f-136">string</span></span>                  |  <span data-ttu-id="8570f-137">选项卡实例的深层链接 URL。</span><span class="sxs-lookup"><span data-stu-id="8570f-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="8570f-138">只读。</span><span class="sxs-lookup"><span data-stu-id="8570f-138">Read only.</span></span>     |
|  <span data-ttu-id="8570f-139">configuration</span><span class="sxs-lookup"><span data-stu-id="8570f-139">configuration</span></span>        |   [<span data-ttu-id="8570f-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="8570f-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="8570f-141">应用于选项卡的自定义设置的容器。只有在设置此属性后，选项卡才被视为已配置。</span><span class="sxs-lookup"><span data-stu-id="8570f-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="8570f-142">关系</span><span class="sxs-lookup"><span data-stu-id="8570f-142">Relationships</span></span>

| <span data-ttu-id="8570f-143">关系</span><span class="sxs-lookup"><span data-stu-id="8570f-143">Relationship</span></span> | <span data-ttu-id="8570f-144">类型</span><span class="sxs-lookup"><span data-stu-id="8570f-144">Type</span></span>   | <span data-ttu-id="8570f-145">说明</span><span class="sxs-lookup"><span data-stu-id="8570f-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8570f-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8570f-146">teamsApp</span></span>|[<span data-ttu-id="8570f-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8570f-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8570f-148">链接到选项卡的应用程序。这无法在选项卡创建后更改。</span><span class="sxs-lookup"><span data-stu-id="8570f-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8570f-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8570f-149">JSON representation</span></span>

<span data-ttu-id="8570f-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8570f-150">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="8570f-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8570f-151">See also</span></span>

[<span data-ttu-id="8570f-152">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="8570f-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

