---
title: teamsTab 资源类型
description: 'teamsTab 是固定 (附加) 到团队中的频道的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 6666fbcd69ac46e778ef46380c426c4e94a129fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345675"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="66a05-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="66a05-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66a05-104">teamsTab 是固定 (附加) 到[团队](team.md)中的[频道](channel.md)的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="66a05-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="66a05-105">方法</span><span class="sxs-lookup"><span data-stu-id="66a05-105">Methods</span></span>

| <span data-ttu-id="66a05-106">方法</span><span class="sxs-lookup"><span data-stu-id="66a05-106">Method</span></span>       | <span data-ttu-id="66a05-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="66a05-107">Return Type</span></span>  |<span data-ttu-id="66a05-108">说明</span><span class="sxs-lookup"><span data-stu-id="66a05-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66a05-109">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="66a05-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="66a05-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="66a05-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="66a05-111">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="66a05-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="66a05-112">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="66a05-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="66a05-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="66a05-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="66a05-114">读取固定到通道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="66a05-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="66a05-115">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="66a05-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="66a05-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="66a05-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="66a05-117">将选项卡添加 (插针) 到频道。</span><span class="sxs-lookup"><span data-stu-id="66a05-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="66a05-118">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="66a05-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="66a05-119">无</span><span class="sxs-lookup"><span data-stu-id="66a05-119">None</span></span> | <span data-ttu-id="66a05-120">从频道中删除 (unpins) 选项卡。</span><span class="sxs-lookup"><span data-stu-id="66a05-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="66a05-121">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="66a05-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="66a05-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="66a05-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="66a05-123">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="66a05-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="66a05-124">属性</span><span class="sxs-lookup"><span data-stu-id="66a05-124">Properties</span></span>

|<span data-ttu-id="66a05-125">属性</span><span class="sxs-lookup"><span data-stu-id="66a05-125">Property</span></span>|<span data-ttu-id="66a05-126">类型</span><span class="sxs-lookup"><span data-stu-id="66a05-126">Type</span></span>|<span data-ttu-id="66a05-127">说明</span><span class="sxs-lookup"><span data-stu-id="66a05-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="66a05-128">id</span><span class="sxs-lookup"><span data-stu-id="66a05-128">id</span></span>              |   <span data-ttu-id="66a05-129">字符串</span><span class="sxs-lookup"><span data-stu-id="66a05-129">string</span></span>                  |  <span data-ttu-id="66a05-130">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="66a05-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="66a05-131">displayName</span><span class="sxs-lookup"><span data-stu-id="66a05-131">displayName</span></span>            |   <span data-ttu-id="66a05-132">string</span><span class="sxs-lookup"><span data-stu-id="66a05-132">string</span></span>                  |  <span data-ttu-id="66a05-133">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="66a05-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="66a05-134">name</span><span class="sxs-lookup"><span data-stu-id="66a05-134">name</span></span>            |   <span data-ttu-id="66a05-135">string</span><span class="sxs-lookup"><span data-stu-id="66a05-135">string</span></span>                  |  <span data-ttu-id="66a05-136">被选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="66a05-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="66a05-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="66a05-137">teamsAppId</span></span>           |   <span data-ttu-id="66a05-138">string</span><span class="sxs-lookup"><span data-stu-id="66a05-138">string</span></span>             |  <span data-ttu-id="66a05-139">选项卡的应用程序定义标识符。创建选项卡后, 不能更改此值。</span><span class="sxs-lookup"><span data-stu-id="66a05-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="66a05-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="66a05-140">sortOrderIndex</span></span>  |   <span data-ttu-id="66a05-141">string</span><span class="sxs-lookup"><span data-stu-id="66a05-141">string</span></span>                  |  <span data-ttu-id="66a05-142">用于对选项卡进行排序的顺序的索引。</span><span class="sxs-lookup"><span data-stu-id="66a05-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="66a05-143">WebUrl</span><span class="sxs-lookup"><span data-stu-id="66a05-143">webUrl</span></span>          |   <span data-ttu-id="66a05-144">string</span><span class="sxs-lookup"><span data-stu-id="66a05-144">string</span></span>                  |  <span data-ttu-id="66a05-145">选项卡实例的深层链接 url。</span><span class="sxs-lookup"><span data-stu-id="66a05-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="66a05-146">只读。</span><span class="sxs-lookup"><span data-stu-id="66a05-146">Read only.</span></span>     |
|  <span data-ttu-id="66a05-147">设置</span><span class="sxs-lookup"><span data-stu-id="66a05-147">configuration</span></span>        |   [<span data-ttu-id="66a05-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="66a05-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="66a05-149">应用于选项卡的自定义设置的容器。仅在设置此属性后, 才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="66a05-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="66a05-150">关系</span><span class="sxs-lookup"><span data-stu-id="66a05-150">Relationships</span></span>

| <span data-ttu-id="66a05-151">关系</span><span class="sxs-lookup"><span data-stu-id="66a05-151">Relationship</span></span> | <span data-ttu-id="66a05-152">类型</span><span class="sxs-lookup"><span data-stu-id="66a05-152">Type</span></span>   | <span data-ttu-id="66a05-153">说明</span><span class="sxs-lookup"><span data-stu-id="66a05-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="66a05-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="66a05-154">teamsApp</span></span>|[<span data-ttu-id="66a05-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="66a05-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="66a05-156">链接到该选项卡的应用程序。</span><span class="sxs-lookup"><span data-stu-id="66a05-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66a05-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66a05-157">JSON representation</span></span>

<span data-ttu-id="66a05-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66a05-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="66a05-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="66a05-159">See also</span></span>

[<span data-ttu-id="66a05-160">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="66a05-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
