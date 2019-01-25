---
title: teamsTab 资源类型
description: 'TeamsTab 是一个选项卡的具有固定 （附加） 到团队中的通道。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2db59065f139e2e704c3394f7afb82cba91c33fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509285"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="a0d3b-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0d3b-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d3b-104">TeamsTab 是[选项卡上](../resources/teamstab.md)的具有固定 （附加） 到[团队](team.md)内的[通道](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a0d3b-105">方法</span><span class="sxs-lookup"><span data-stu-id="a0d3b-105">Methods</span></span>

| <span data-ttu-id="a0d3b-106">方法</span><span class="sxs-lookup"><span data-stu-id="a0d3b-106">Method</span></span>       | <span data-ttu-id="a0d3b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0d3b-107">Return Type</span></span>  |<span data-ttu-id="a0d3b-108">说明</span><span class="sxs-lookup"><span data-stu-id="a0d3b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0d3b-109">列表选项卡</span><span class="sxs-lookup"><span data-stu-id="a0d3b-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="a0d3b-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0d3b-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0d3b-111">到通道固定列表选项卡。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a0d3b-112">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="a0d3b-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="a0d3b-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0d3b-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0d3b-114">读取固定到频道的一个选项卡。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a0d3b-115">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="a0d3b-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="a0d3b-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0d3b-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0d3b-117">添加 (pin) 通道向选项卡。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a0d3b-118">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="a0d3b-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="a0d3b-119">无</span><span class="sxs-lookup"><span data-stu-id="a0d3b-119">None</span></span> | <span data-ttu-id="a0d3b-120">删除 （取消锁定） 通道从选项卡。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="a0d3b-121">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="a0d3b-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="a0d3b-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0d3b-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0d3b-123">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="a0d3b-124">属性</span><span class="sxs-lookup"><span data-stu-id="a0d3b-124">Properties</span></span>

|<span data-ttu-id="a0d3b-125">属性</span><span class="sxs-lookup"><span data-stu-id="a0d3b-125">Property</span></span>|<span data-ttu-id="a0d3b-126">类型</span><span class="sxs-lookup"><span data-stu-id="a0d3b-126">Type</span></span>|<span data-ttu-id="a0d3b-127">说明</span><span class="sxs-lookup"><span data-stu-id="a0d3b-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a0d3b-128">id</span><span class="sxs-lookup"><span data-stu-id="a0d3b-128">id</span></span>              |   <span data-ttu-id="a0d3b-129">string</span><span class="sxs-lookup"><span data-stu-id="a0d3b-129">string</span></span>                  |  <span data-ttu-id="a0d3b-130">唯一标识通道选项读取仅的特定实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a0d3b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a0d3b-131">displayName</span></span>            |   <span data-ttu-id="a0d3b-132">string</span><span class="sxs-lookup"><span data-stu-id="a0d3b-132">string</span></span>                  |  <span data-ttu-id="a0d3b-133">Tab 的名称。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="a0d3b-134">name</span><span class="sxs-lookup"><span data-stu-id="a0d3b-134">name</span></span>            |   <span data-ttu-id="a0d3b-135">string</span><span class="sxs-lookup"><span data-stu-id="a0d3b-135">string</span></span>                  |  <span data-ttu-id="a0d3b-136">（已过时）Tab 的名称。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="a0d3b-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="a0d3b-137">teamsAppId</span></span>           |   <span data-ttu-id="a0d3b-138">string</span><span class="sxs-lookup"><span data-stu-id="a0d3b-138">string</span></span>             |  <span data-ttu-id="a0d3b-139">应用程序定义的选项卡的标识符。选项卡创建后，无法更改此值。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="a0d3b-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="a0d3b-140">sortOrderIndex</span></span>  |   <span data-ttu-id="a0d3b-141">int</span><span class="sxs-lookup"><span data-stu-id="a0d3b-141">int</span></span>                     |  <span data-ttu-id="a0d3b-142">用于排序选项卡的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="a0d3b-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="a0d3b-143">webUrl</span></span>          |   <span data-ttu-id="a0d3b-144">string</span><span class="sxs-lookup"><span data-stu-id="a0d3b-144">string</span></span>                  |  <span data-ttu-id="a0d3b-145">深度链接的选项卡实例的 url。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="a0d3b-146">只读。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-146">Read only.</span></span>     |
|  <span data-ttu-id="a0d3b-147">configuration</span><span class="sxs-lookup"><span data-stu-id="a0d3b-147">configuration</span></span>        |   [<span data-ttu-id="a0d3b-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0d3b-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a0d3b-149">应用于选项卡的自定义设置的容器。配置仅后设置此属性时，才视为选项卡。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a0d3b-150">关系</span><span class="sxs-lookup"><span data-stu-id="a0d3b-150">Relationships</span></span>

| <span data-ttu-id="a0d3b-151">关系</span><span class="sxs-lookup"><span data-stu-id="a0d3b-151">Relationship</span></span> | <span data-ttu-id="a0d3b-152">类型</span><span class="sxs-lookup"><span data-stu-id="a0d3b-152">Type</span></span>   | <span data-ttu-id="a0d3b-153">说明</span><span class="sxs-lookup"><span data-stu-id="a0d3b-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a0d3b-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0d3b-154">teamsApp</span></span>|[<span data-ttu-id="a0d3b-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0d3b-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a0d3b-156">应用程序的链接到选项卡。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0d3b-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0d3b-157">JSON representation</span></span>

<span data-ttu-id="a0d3b-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0d3b-158">The following is a JSON representation of the resource.</span></span>


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
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstab.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="a0d3b-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a0d3b-159">See also</span></span>

[<span data-ttu-id="a0d3b-160">配置到内置选项卡的类型</span><span class="sxs-lookup"><span data-stu-id="a0d3b-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
