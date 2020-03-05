---
title: teamsTab 资源类型
description: 'TeamsTab 是固定（附加）到团队中的频道的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 74dfe42bc48757ffe8799a033dfebf2df61f913d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519846"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="9f9f3-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f9f3-103">teamsTab resource type</span></span>

<span data-ttu-id="9f9f3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9f9f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f9f3-105">TeamsTab 是固定（附加）到[团队](team.md)中的[频道](channel.md)的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="9f9f3-106">方法</span><span class="sxs-lookup"><span data-stu-id="9f9f3-106">Methods</span></span>

| <span data-ttu-id="9f9f3-107">方法</span><span class="sxs-lookup"><span data-stu-id="9f9f3-107">Method</span></span>       | <span data-ttu-id="9f9f3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f9f3-108">Return Type</span></span>  |<span data-ttu-id="9f9f3-109">说明</span><span class="sxs-lookup"><span data-stu-id="9f9f3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f9f3-110">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="9f9f3-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="9f9f3-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f9f3-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f9f3-112">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="9f9f3-113">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="9f9f3-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="9f9f3-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f9f3-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f9f3-115">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="9f9f3-116">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="9f9f3-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="9f9f3-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f9f3-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f9f3-118">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="9f9f3-119">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="9f9f3-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="9f9f3-120">无</span><span class="sxs-lookup"><span data-stu-id="9f9f3-120">None</span></span> | <span data-ttu-id="9f9f3-121">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="9f9f3-122">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="9f9f3-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="9f9f3-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f9f3-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f9f3-124">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="9f9f3-125">属性</span><span class="sxs-lookup"><span data-stu-id="9f9f3-125">Properties</span></span>

|<span data-ttu-id="9f9f3-126">属性</span><span class="sxs-lookup"><span data-stu-id="9f9f3-126">Property</span></span>|<span data-ttu-id="9f9f3-127">类型</span><span class="sxs-lookup"><span data-stu-id="9f9f3-127">Type</span></span>|<span data-ttu-id="9f9f3-128">说明</span><span class="sxs-lookup"><span data-stu-id="9f9f3-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="9f9f3-129">id</span><span class="sxs-lookup"><span data-stu-id="9f9f3-129">id</span></span>              |   <span data-ttu-id="9f9f3-130">字符串</span><span class="sxs-lookup"><span data-stu-id="9f9f3-130">string</span></span>                  |  <span data-ttu-id="9f9f3-131">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="9f9f3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9f9f3-132">displayName</span></span>            |   <span data-ttu-id="9f9f3-133">string</span><span class="sxs-lookup"><span data-stu-id="9f9f3-133">string</span></span>                  |  <span data-ttu-id="9f9f3-134">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="9f9f3-135">name</span><span class="sxs-lookup"><span data-stu-id="9f9f3-135">name</span></span>            |   <span data-ttu-id="9f9f3-136">string</span><span class="sxs-lookup"><span data-stu-id="9f9f3-136">string</span></span>                  |  <span data-ttu-id="9f9f3-137">被选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-137">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="9f9f3-138">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="9f9f3-138">teamsAppId</span></span>           |   <span data-ttu-id="9f9f3-139">string</span><span class="sxs-lookup"><span data-stu-id="9f9f3-139">string</span></span>             |  <span data-ttu-id="9f9f3-140">选项卡的应用程序定义标识符。创建选项卡后，不能更改此值。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="9f9f3-141">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="9f9f3-141">sortOrderIndex</span></span>  |   <span data-ttu-id="9f9f3-142">string</span><span class="sxs-lookup"><span data-stu-id="9f9f3-142">string</span></span>                  |  <span data-ttu-id="9f9f3-143">用于对选项卡进行排序的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-143">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="9f9f3-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="9f9f3-144">webUrl</span></span>          |   <span data-ttu-id="9f9f3-145">string</span><span class="sxs-lookup"><span data-stu-id="9f9f3-145">string</span></span>                  |  <span data-ttu-id="9f9f3-146">选项卡实例的深层链接 url。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-146">Deep link url of the tab instance.</span></span> <span data-ttu-id="9f9f3-147">只读。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-147">Read only.</span></span>     |
|  <span data-ttu-id="9f9f3-148">设置</span><span class="sxs-lookup"><span data-stu-id="9f9f3-148">configuration</span></span>        |   [<span data-ttu-id="9f9f3-149">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f9f3-149">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="9f9f3-150">应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-150">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="9f9f3-151">关系</span><span class="sxs-lookup"><span data-stu-id="9f9f3-151">Relationships</span></span>

| <span data-ttu-id="9f9f3-152">关系</span><span class="sxs-lookup"><span data-stu-id="9f9f3-152">Relationship</span></span> | <span data-ttu-id="9f9f3-153">类型</span><span class="sxs-lookup"><span data-stu-id="9f9f3-153">Type</span></span>   | <span data-ttu-id="9f9f3-154">说明</span><span class="sxs-lookup"><span data-stu-id="9f9f3-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9f9f3-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9f9f3-155">teamsApp</span></span>|[<span data-ttu-id="9f9f3-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9f9f3-156">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="9f9f3-157">链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-157">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f9f3-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f9f3-158">JSON representation</span></span>

<span data-ttu-id="9f9f3-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f9f3-159">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="9f9f3-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9f9f3-160">See also</span></span>

[<span data-ttu-id="9f9f3-161">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="9f9f3-161">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
