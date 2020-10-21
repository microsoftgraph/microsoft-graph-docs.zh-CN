---
title: teamsTab 资源类型
description: 'TeamsTab 是一个固定在团队中的频道 (附加) 的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c60e47a65c9d5b17433891161fe5c16ca182a5ca
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634660"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="e56b2-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="e56b2-103">teamsTab resource type</span></span>

<span data-ttu-id="e56b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e56b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e56b2-105">TeamsTab 是一个固定在[团队](team.md)中的[频道](channel.md) (附加) 的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="e56b2-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="e56b2-106">方法</span><span class="sxs-lookup"><span data-stu-id="e56b2-106">Methods</span></span>

| <span data-ttu-id="e56b2-107">方法</span><span class="sxs-lookup"><span data-stu-id="e56b2-107">Method</span></span>       | <span data-ttu-id="e56b2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e56b2-108">Return Type</span></span>  |<span data-ttu-id="e56b2-109">说明</span><span class="sxs-lookup"><span data-stu-id="e56b2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e56b2-110">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="e56b2-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="e56b2-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e56b2-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e56b2-112">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="e56b2-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="e56b2-113">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="e56b2-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="e56b2-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e56b2-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e56b2-115">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="e56b2-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="e56b2-116">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="e56b2-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e56b2-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e56b2-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e56b2-118">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="e56b2-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="e56b2-119">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="e56b2-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="e56b2-120">无</span><span class="sxs-lookup"><span data-stu-id="e56b2-120">None</span></span> | <span data-ttu-id="e56b2-121">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="e56b2-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="e56b2-122">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="e56b2-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="e56b2-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e56b2-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e56b2-124">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="e56b2-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="e56b2-125">属性</span><span class="sxs-lookup"><span data-stu-id="e56b2-125">Properties</span></span>

|<span data-ttu-id="e56b2-126">属性</span><span class="sxs-lookup"><span data-stu-id="e56b2-126">Property</span></span>|<span data-ttu-id="e56b2-127">类型</span><span class="sxs-lookup"><span data-stu-id="e56b2-127">Type</span></span>|<span data-ttu-id="e56b2-128">说明</span><span class="sxs-lookup"><span data-stu-id="e56b2-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="e56b2-129">id</span><span class="sxs-lookup"><span data-stu-id="e56b2-129">id</span></span>              |   <span data-ttu-id="e56b2-130">string</span><span class="sxs-lookup"><span data-stu-id="e56b2-130">string</span></span>                  |  <span data-ttu-id="e56b2-131">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e56b2-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="e56b2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e56b2-132">displayName</span></span>            |   <span data-ttu-id="e56b2-133">string</span><span class="sxs-lookup"><span data-stu-id="e56b2-133">string</span></span>                  |  <span data-ttu-id="e56b2-134">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="e56b2-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="e56b2-135">名称 (弃用) </span><span class="sxs-lookup"><span data-stu-id="e56b2-135">name (deprecated)</span></span>      |   <span data-ttu-id="e56b2-136">string</span><span class="sxs-lookup"><span data-stu-id="e56b2-136">string</span></span>                  |  <span data-ttu-id="e56b2-137">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="e56b2-137">Name of the tab.</span></span>     |
|  <span data-ttu-id="e56b2-138">teamsAppId (弃用) </span><span class="sxs-lookup"><span data-stu-id="e56b2-138">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="e56b2-139">string</span><span class="sxs-lookup"><span data-stu-id="e56b2-139">string</span></span>             |  <span data-ttu-id="e56b2-140">选项卡的应用程序定义标识符。创建选项卡后，不能更改此值。</span><span class="sxs-lookup"><span data-stu-id="e56b2-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="e56b2-141">由于此属性已弃用，因此我们建议扩展 **teamsApp** 以检索链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e56b2-141">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="e56b2-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="e56b2-142">sortOrderIndex</span></span>  |   <span data-ttu-id="e56b2-143">string</span><span class="sxs-lookup"><span data-stu-id="e56b2-143">string</span></span>                  |  <span data-ttu-id="e56b2-144">用于对选项卡进行排序的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="e56b2-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="e56b2-145">WebUrl</span><span class="sxs-lookup"><span data-stu-id="e56b2-145">webUrl</span></span>          |   <span data-ttu-id="e56b2-146">string</span><span class="sxs-lookup"><span data-stu-id="e56b2-146">string</span></span>                  |  <span data-ttu-id="e56b2-147">选项卡实例的深层链接 URL。</span><span class="sxs-lookup"><span data-stu-id="e56b2-147">Deep link URL of the tab instance.</span></span> <span data-ttu-id="e56b2-148">只读。</span><span class="sxs-lookup"><span data-stu-id="e56b2-148">Read only.</span></span>     |
|  <span data-ttu-id="e56b2-149">configuration</span><span class="sxs-lookup"><span data-stu-id="e56b2-149">configuration</span></span>        |   [<span data-ttu-id="e56b2-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="e56b2-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="e56b2-151">应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="e56b2-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="e56b2-152">关系</span><span class="sxs-lookup"><span data-stu-id="e56b2-152">Relationships</span></span>

| <span data-ttu-id="e56b2-153">关系</span><span class="sxs-lookup"><span data-stu-id="e56b2-153">Relationship</span></span> | <span data-ttu-id="e56b2-154">类型</span><span class="sxs-lookup"><span data-stu-id="e56b2-154">Type</span></span>   | <span data-ttu-id="e56b2-155">说明</span><span class="sxs-lookup"><span data-stu-id="e56b2-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e56b2-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e56b2-156">teamsApp</span></span>|[<span data-ttu-id="e56b2-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e56b2-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="e56b2-158">链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e56b2-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e56b2-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e56b2-159">JSON representation</span></span>

<span data-ttu-id="e56b2-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e56b2-160">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="e56b2-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e56b2-161">See also</span></span>

[<span data-ttu-id="e56b2-162">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="e56b2-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


