---
title: teamsTab 资源类型
description: 'TeamsTab 是固定（附加）到团队中的频道的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d4b8bf73499bc2cca2a7497e57e3cce6c8cbe5b9
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2020
ms.locfileid: "41559038"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="527f5-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="527f5-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="527f5-104">TeamsTab 是固定（附加）到[团队](team.md)中的[频道](channel.md)的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="527f5-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="527f5-105">方法</span><span class="sxs-lookup"><span data-stu-id="527f5-105">Methods</span></span>

| <span data-ttu-id="527f5-106">方法</span><span class="sxs-lookup"><span data-stu-id="527f5-106">Method</span></span>       | <span data-ttu-id="527f5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="527f5-107">Return Type</span></span>  |<span data-ttu-id="527f5-108">说明</span><span class="sxs-lookup"><span data-stu-id="527f5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="527f5-109">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="527f5-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="527f5-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="527f5-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="527f5-111">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="527f5-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="527f5-112">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="527f5-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="527f5-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="527f5-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="527f5-114">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="527f5-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="527f5-115">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="527f5-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="527f5-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="527f5-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="527f5-117">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="527f5-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="527f5-118">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="527f5-118">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="527f5-119">无</span><span class="sxs-lookup"><span data-stu-id="527f5-119">None</span></span> | <span data-ttu-id="527f5-120">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="527f5-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="527f5-121">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="527f5-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="527f5-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="527f5-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="527f5-123">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="527f5-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="527f5-124">属性</span><span class="sxs-lookup"><span data-stu-id="527f5-124">Properties</span></span>

|<span data-ttu-id="527f5-125">属性</span><span class="sxs-lookup"><span data-stu-id="527f5-125">Property</span></span>|<span data-ttu-id="527f5-126">类型</span><span class="sxs-lookup"><span data-stu-id="527f5-126">Type</span></span>|<span data-ttu-id="527f5-127">说明</span><span class="sxs-lookup"><span data-stu-id="527f5-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="527f5-128">id</span><span class="sxs-lookup"><span data-stu-id="527f5-128">id</span></span>              |   <span data-ttu-id="527f5-129">字符串</span><span class="sxs-lookup"><span data-stu-id="527f5-129">string</span></span>                  |  <span data-ttu-id="527f5-130">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="527f5-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="527f5-131">displayName</span><span class="sxs-lookup"><span data-stu-id="527f5-131">displayName</span></span>            |   <span data-ttu-id="527f5-132">string</span><span class="sxs-lookup"><span data-stu-id="527f5-132">string</span></span>                  |  <span data-ttu-id="527f5-133">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="527f5-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="527f5-134">name</span><span class="sxs-lookup"><span data-stu-id="527f5-134">name</span></span>            |   <span data-ttu-id="527f5-135">string</span><span class="sxs-lookup"><span data-stu-id="527f5-135">string</span></span>                  |  <span data-ttu-id="527f5-136">被选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="527f5-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="527f5-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="527f5-137">teamsAppId</span></span>           |   <span data-ttu-id="527f5-138">string</span><span class="sxs-lookup"><span data-stu-id="527f5-138">string</span></span>             |  <span data-ttu-id="527f5-139">选项卡的应用程序定义标识符。创建选项卡后，不能更改此值。</span><span class="sxs-lookup"><span data-stu-id="527f5-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="527f5-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="527f5-140">sortOrderIndex</span></span>  |   <span data-ttu-id="527f5-141">string</span><span class="sxs-lookup"><span data-stu-id="527f5-141">string</span></span>                  |  <span data-ttu-id="527f5-142">用于对选项卡进行排序的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="527f5-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="527f5-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="527f5-143">webUrl</span></span>          |   <span data-ttu-id="527f5-144">string</span><span class="sxs-lookup"><span data-stu-id="527f5-144">string</span></span>                  |  <span data-ttu-id="527f5-145">选项卡实例的深层链接 url。</span><span class="sxs-lookup"><span data-stu-id="527f5-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="527f5-146">只读。</span><span class="sxs-lookup"><span data-stu-id="527f5-146">Read only.</span></span>     |
|  <span data-ttu-id="527f5-147">设置</span><span class="sxs-lookup"><span data-stu-id="527f5-147">configuration</span></span>        |   [<span data-ttu-id="527f5-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="527f5-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="527f5-149">应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="527f5-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="527f5-150">关系</span><span class="sxs-lookup"><span data-stu-id="527f5-150">Relationships</span></span>

| <span data-ttu-id="527f5-151">关系</span><span class="sxs-lookup"><span data-stu-id="527f5-151">Relationship</span></span> | <span data-ttu-id="527f5-152">类型</span><span class="sxs-lookup"><span data-stu-id="527f5-152">Type</span></span>   | <span data-ttu-id="527f5-153">说明</span><span class="sxs-lookup"><span data-stu-id="527f5-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="527f5-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="527f5-154">teamsApp</span></span>|[<span data-ttu-id="527f5-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="527f5-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="527f5-156">链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="527f5-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="527f5-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="527f5-157">JSON representation</span></span>

<span data-ttu-id="527f5-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="527f5-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="527f5-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="527f5-159">See also</span></span>

[<span data-ttu-id="527f5-160">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="527f5-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
