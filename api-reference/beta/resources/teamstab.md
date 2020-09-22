---
title: teamsTab 资源类型
description: 'TeamsTab 是一个固定在团队中的频道 (附加) 的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5684c98f15ed039fbba36b1df517a6d7d1d5d8c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046445"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="2b6e2-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b6e2-103">teamsTab resource type</span></span>

<span data-ttu-id="2b6e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b6e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b6e2-105">TeamsTab 是一个固定在[团队](team.md)中的[频道](channel.md) (附加) 的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="2b6e2-106">方法</span><span class="sxs-lookup"><span data-stu-id="2b6e2-106">Methods</span></span>

| <span data-ttu-id="2b6e2-107">方法</span><span class="sxs-lookup"><span data-stu-id="2b6e2-107">Method</span></span>       | <span data-ttu-id="2b6e2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2b6e2-108">Return Type</span></span>  |<span data-ttu-id="2b6e2-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b6e2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b6e2-110">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="2b6e2-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="2b6e2-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2b6e2-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2b6e2-112">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="2b6e2-113">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="2b6e2-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="2b6e2-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2b6e2-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2b6e2-115">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="2b6e2-116">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="2b6e2-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="2b6e2-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2b6e2-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2b6e2-118">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="2b6e2-119">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="2b6e2-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="2b6e2-120">无</span><span class="sxs-lookup"><span data-stu-id="2b6e2-120">None</span></span> | <span data-ttu-id="2b6e2-121">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="2b6e2-122">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="2b6e2-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="2b6e2-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2b6e2-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2b6e2-124">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="2b6e2-125">属性</span><span class="sxs-lookup"><span data-stu-id="2b6e2-125">Properties</span></span>

|<span data-ttu-id="2b6e2-126">属性</span><span class="sxs-lookup"><span data-stu-id="2b6e2-126">Property</span></span>|<span data-ttu-id="2b6e2-127">类型</span><span class="sxs-lookup"><span data-stu-id="2b6e2-127">Type</span></span>|<span data-ttu-id="2b6e2-128">说明</span><span class="sxs-lookup"><span data-stu-id="2b6e2-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="2b6e2-129">id</span><span class="sxs-lookup"><span data-stu-id="2b6e2-129">id</span></span>              |   <span data-ttu-id="2b6e2-130">string</span><span class="sxs-lookup"><span data-stu-id="2b6e2-130">string</span></span>                  |  <span data-ttu-id="2b6e2-131">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="2b6e2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2b6e2-132">displayName</span></span>            |   <span data-ttu-id="2b6e2-133">string</span><span class="sxs-lookup"><span data-stu-id="2b6e2-133">string</span></span>                  |  <span data-ttu-id="2b6e2-134">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="2b6e2-135">name</span><span class="sxs-lookup"><span data-stu-id="2b6e2-135">name</span></span>            |   <span data-ttu-id="2b6e2-136">string</span><span class="sxs-lookup"><span data-stu-id="2b6e2-136">string</span></span>                  |  <span data-ttu-id="2b6e2-137"> (已弃用) 选项卡名称。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-137">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="2b6e2-138">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="2b6e2-138">teamsAppId</span></span>           |   <span data-ttu-id="2b6e2-139">string</span><span class="sxs-lookup"><span data-stu-id="2b6e2-139">string</span></span>             |  <span data-ttu-id="2b6e2-140">选项卡的应用程序定义标识符。创建选项卡后，不能更改此值。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="2b6e2-141">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="2b6e2-141">sortOrderIndex</span></span>  |   <span data-ttu-id="2b6e2-142">string</span><span class="sxs-lookup"><span data-stu-id="2b6e2-142">string</span></span>                  |  <span data-ttu-id="2b6e2-143">用于对选项卡进行排序的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-143">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="2b6e2-144">WebUrl</span><span class="sxs-lookup"><span data-stu-id="2b6e2-144">webUrl</span></span>          |   <span data-ttu-id="2b6e2-145">string</span><span class="sxs-lookup"><span data-stu-id="2b6e2-145">string</span></span>                  |  <span data-ttu-id="2b6e2-146">选项卡实例的深层链接 URL。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-146">Deep link URL of the tab instance.</span></span> <span data-ttu-id="2b6e2-147">只读。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-147">Read only.</span></span>     |
|  <span data-ttu-id="2b6e2-148">configuration</span><span class="sxs-lookup"><span data-stu-id="2b6e2-148">configuration</span></span>        |   [<span data-ttu-id="2b6e2-149">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b6e2-149">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="2b6e2-150">应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-150">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="2b6e2-151">关系</span><span class="sxs-lookup"><span data-stu-id="2b6e2-151">Relationships</span></span>

| <span data-ttu-id="2b6e2-152">关系</span><span class="sxs-lookup"><span data-stu-id="2b6e2-152">Relationship</span></span> | <span data-ttu-id="2b6e2-153">类型</span><span class="sxs-lookup"><span data-stu-id="2b6e2-153">Type</span></span>   | <span data-ttu-id="2b6e2-154">说明</span><span class="sxs-lookup"><span data-stu-id="2b6e2-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2b6e2-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2b6e2-155">teamsApp</span></span>|[<span data-ttu-id="2b6e2-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2b6e2-156">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="2b6e2-157">链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-157">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b6e2-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b6e2-158">JSON representation</span></span>

<span data-ttu-id="2b6e2-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-159">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="2b6e2-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2b6e2-160">See also</span></span>

[<span data-ttu-id="2b6e2-161">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="2b6e2-161">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


