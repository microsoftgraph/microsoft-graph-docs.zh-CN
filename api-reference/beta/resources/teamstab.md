---
title: teamsTab 资源类型
description: 'TeamsTab 是一个选项卡的具有固定 （附加） 到团队中的通道。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3c5cf5ef33f53cfaca7189df24e5dfd880a77241
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947146"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="48960-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="48960-103">teamsTab resource type</span></span>

> <span data-ttu-id="48960-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="48960-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48960-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48960-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48960-106">TeamsTab 是[选项卡上](../resources/teamstab.md)的具有固定 （附加） 到[团队](team.md)内的[通道](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="48960-106">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="48960-107">方法</span><span class="sxs-lookup"><span data-stu-id="48960-107">Methods</span></span>

| <span data-ttu-id="48960-108">方法</span><span class="sxs-lookup"><span data-stu-id="48960-108">Method</span></span>       | <span data-ttu-id="48960-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="48960-109">Return Type</span></span>  |<span data-ttu-id="48960-110">说明</span><span class="sxs-lookup"><span data-stu-id="48960-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48960-111">列表选项卡</span><span class="sxs-lookup"><span data-stu-id="48960-111">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="48960-112">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48960-112">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48960-113">到通道固定列表选项卡。</span><span class="sxs-lookup"><span data-stu-id="48960-113">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="48960-114">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="48960-114">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="48960-115">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48960-115">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48960-116">读取固定到频道的一个选项卡。</span><span class="sxs-lookup"><span data-stu-id="48960-116">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="48960-117">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="48960-117">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="48960-118">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48960-118">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48960-119">添加 (pin) 通道向选项卡。</span><span class="sxs-lookup"><span data-stu-id="48960-119">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="48960-120">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="48960-120">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="48960-121">无</span><span class="sxs-lookup"><span data-stu-id="48960-121">None</span></span> | <span data-ttu-id="48960-122">删除 （取消锁定） 通道从选项卡。</span><span class="sxs-lookup"><span data-stu-id="48960-122">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="48960-123">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="48960-123">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="48960-124">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48960-124">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="48960-125">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="48960-125">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="48960-126">属性</span><span class="sxs-lookup"><span data-stu-id="48960-126">Properties</span></span>

|<span data-ttu-id="48960-127">属性</span><span class="sxs-lookup"><span data-stu-id="48960-127">Property</span></span>|<span data-ttu-id="48960-128">类型</span><span class="sxs-lookup"><span data-stu-id="48960-128">Type</span></span>|<span data-ttu-id="48960-129">说明</span><span class="sxs-lookup"><span data-stu-id="48960-129">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="48960-130">ID</span><span class="sxs-lookup"><span data-stu-id="48960-130">id</span></span>              |   <span data-ttu-id="48960-131">string</span><span class="sxs-lookup"><span data-stu-id="48960-131">string</span></span>                  |  <span data-ttu-id="48960-132">唯一标识通道选项读取仅的特定实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="48960-132">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="48960-133">displayName</span><span class="sxs-lookup"><span data-stu-id="48960-133">displayName</span></span>            |   <span data-ttu-id="48960-134">string</span><span class="sxs-lookup"><span data-stu-id="48960-134">string</span></span>                  |  <span data-ttu-id="48960-135">Tab 的名称。</span><span class="sxs-lookup"><span data-stu-id="48960-135">Name of the tab.</span></span>     |
|  <span data-ttu-id="48960-136">name</span><span class="sxs-lookup"><span data-stu-id="48960-136">name</span></span>            |   <span data-ttu-id="48960-137">string</span><span class="sxs-lookup"><span data-stu-id="48960-137">string</span></span>                  |  <span data-ttu-id="48960-138">（已过时）Tab 的名称。</span><span class="sxs-lookup"><span data-stu-id="48960-138">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="48960-139">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="48960-139">teamsAppId</span></span>           |   <span data-ttu-id="48960-140">string</span><span class="sxs-lookup"><span data-stu-id="48960-140">string</span></span>             |  <span data-ttu-id="48960-141">应用程序定义的选项卡的标识符。选项卡创建后，无法更改此值。</span><span class="sxs-lookup"><span data-stu-id="48960-141">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="48960-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="48960-142">sortOrderIndex</span></span>  |   <span data-ttu-id="48960-143">int</span><span class="sxs-lookup"><span data-stu-id="48960-143">int</span></span>                     |  <span data-ttu-id="48960-144">用于排序选项卡的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="48960-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="48960-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="48960-145">webUrl</span></span>          |   <span data-ttu-id="48960-146">string</span><span class="sxs-lookup"><span data-stu-id="48960-146">string</span></span>                  |  <span data-ttu-id="48960-147">深度链接的选项卡实例的 url。</span><span class="sxs-lookup"><span data-stu-id="48960-147">Deep link url of the tab instance.</span></span> <span data-ttu-id="48960-148">只读。</span><span class="sxs-lookup"><span data-stu-id="48960-148">Read only.</span></span>     |
|  <span data-ttu-id="48960-149">configuration</span><span class="sxs-lookup"><span data-stu-id="48960-149">configuration</span></span>        |   [<span data-ttu-id="48960-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="48960-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="48960-151">应用于选项卡的自定义设置的容器。配置仅后设置此属性时，才视为选项卡。</span><span class="sxs-lookup"><span data-stu-id="48960-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="48960-152">Relationships</span><span class="sxs-lookup"><span data-stu-id="48960-152">Relationships</span></span>

| <span data-ttu-id="48960-153">关系</span><span class="sxs-lookup"><span data-stu-id="48960-153">Relationship</span></span> | <span data-ttu-id="48960-154">类型</span><span class="sxs-lookup"><span data-stu-id="48960-154">Type</span></span>   | <span data-ttu-id="48960-155">说明</span><span class="sxs-lookup"><span data-stu-id="48960-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="48960-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="48960-156">teamsApp</span></span>|[<span data-ttu-id="48960-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="48960-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="48960-158">应用程序的链接到选项卡。</span><span class="sxs-lookup"><span data-stu-id="48960-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48960-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48960-159">JSON representation</span></span>

<span data-ttu-id="48960-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48960-160">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="48960-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="48960-161">See also</span></span>

[<span data-ttu-id="48960-162">配置到内置选项卡的类型</span><span class="sxs-lookup"><span data-stu-id="48960-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
