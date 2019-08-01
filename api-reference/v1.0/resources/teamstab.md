---
title: teamsTab 资源类型
description: 'TeamsTab 是固定 (附加) 到团队中的频道的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bf07770d920ee05c7856f89e2e099bcc958ad50c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033689"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="c88e6-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="c88e6-103">teamsTab resource type</span></span>



<span data-ttu-id="c88e6-104">TeamsTab 是固定 (附加) 到[团队](team.md)中的[频道](channel.md)的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="c88e6-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="c88e6-105">方法</span><span class="sxs-lookup"><span data-stu-id="c88e6-105">Methods</span></span>

| <span data-ttu-id="c88e6-106">方法</span><span class="sxs-lookup"><span data-stu-id="c88e6-106">Method</span></span>       | <span data-ttu-id="c88e6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c88e6-107">Return Type</span></span>  |<span data-ttu-id="c88e6-108">说明</span><span class="sxs-lookup"><span data-stu-id="c88e6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c88e6-109">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="c88e6-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="c88e6-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c88e6-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c88e6-111">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="c88e6-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="c88e6-112">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="c88e6-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="c88e6-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c88e6-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c88e6-114">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="c88e6-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="c88e6-115">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="c88e6-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="c88e6-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c88e6-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c88e6-117">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="c88e6-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="c88e6-118">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="c88e6-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="c88e6-119">无</span><span class="sxs-lookup"><span data-stu-id="c88e6-119">None</span></span> | <span data-ttu-id="c88e6-120">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="c88e6-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="c88e6-121">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="c88e6-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="c88e6-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c88e6-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c88e6-123">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="c88e6-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="c88e6-124">属性</span><span class="sxs-lookup"><span data-stu-id="c88e6-124">Properties</span></span>

|<span data-ttu-id="c88e6-125">属性</span><span class="sxs-lookup"><span data-stu-id="c88e6-125">Property</span></span>|<span data-ttu-id="c88e6-126">类型</span><span class="sxs-lookup"><span data-stu-id="c88e6-126">Type</span></span>|<span data-ttu-id="c88e6-127">说明</span><span class="sxs-lookup"><span data-stu-id="c88e6-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="c88e6-128">id</span><span class="sxs-lookup"><span data-stu-id="c88e6-128">id</span></span>              |   <span data-ttu-id="c88e6-129">字符串</span><span class="sxs-lookup"><span data-stu-id="c88e6-129">string</span></span>                  |  <span data-ttu-id="c88e6-130">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="c88e6-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="c88e6-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c88e6-131">displayName</span></span>            |   <span data-ttu-id="c88e6-132">string</span><span class="sxs-lookup"><span data-stu-id="c88e6-132">string</span></span>                  |  <span data-ttu-id="c88e6-133">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="c88e6-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="c88e6-134">WebUrl</span><span class="sxs-lookup"><span data-stu-id="c88e6-134">webUrl</span></span>          |   <span data-ttu-id="c88e6-135">string</span><span class="sxs-lookup"><span data-stu-id="c88e6-135">string</span></span>                  |  <span data-ttu-id="c88e6-136">选项卡实例的深层链接 url。</span><span class="sxs-lookup"><span data-stu-id="c88e6-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="c88e6-137">只读。</span><span class="sxs-lookup"><span data-stu-id="c88e6-137">Read only.</span></span>     |
|  <span data-ttu-id="c88e6-138">设置</span><span class="sxs-lookup"><span data-stu-id="c88e6-138">configuration</span></span>        |   [<span data-ttu-id="c88e6-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="c88e6-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="c88e6-140">应用于选项卡的自定义设置的容器。仅在设置此属性后, 才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="c88e6-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="c88e6-141">关系</span><span class="sxs-lookup"><span data-stu-id="c88e6-141">Relationships</span></span>

| <span data-ttu-id="c88e6-142">关系</span><span class="sxs-lookup"><span data-stu-id="c88e6-142">Relationship</span></span> | <span data-ttu-id="c88e6-143">类型</span><span class="sxs-lookup"><span data-stu-id="c88e6-143">Type</span></span>   | <span data-ttu-id="c88e6-144">说明</span><span class="sxs-lookup"><span data-stu-id="c88e6-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c88e6-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c88e6-145">teamsApp</span></span>|[<span data-ttu-id="c88e6-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c88e6-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="c88e6-147">链接到该选项卡的应用程序。创建选项卡后, 不能更改此选项。</span><span class="sxs-lookup"><span data-stu-id="c88e6-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c88e6-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c88e6-148">JSON representation</span></span>

<span data-ttu-id="c88e6-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c88e6-149">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="c88e6-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c88e6-150">See also</span></span>

[<span data-ttu-id="c88e6-151">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="c88e6-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
