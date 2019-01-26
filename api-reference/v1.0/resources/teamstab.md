---
title: teamsTab 资源类型
description: 'TeamsTab 是一个选项卡的具有固定 （附加） 到团队中的通道。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574668"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="af2c8-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="af2c8-103">teamsTab resource type</span></span>



<span data-ttu-id="af2c8-104">TeamsTab 是[选项卡上](../resources/teamstab.md)的具有固定 （附加） 到[团队](team.md)内的[通道](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="af2c8-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="af2c8-105">方法</span><span class="sxs-lookup"><span data-stu-id="af2c8-105">Methods</span></span>

| <span data-ttu-id="af2c8-106">方法</span><span class="sxs-lookup"><span data-stu-id="af2c8-106">Method</span></span>       | <span data-ttu-id="af2c8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="af2c8-107">Return Type</span></span>  |<span data-ttu-id="af2c8-108">说明</span><span class="sxs-lookup"><span data-stu-id="af2c8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af2c8-109">列表选项卡</span><span class="sxs-lookup"><span data-stu-id="af2c8-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="af2c8-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="af2c8-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="af2c8-111">到通道固定列表选项卡。</span><span class="sxs-lookup"><span data-stu-id="af2c8-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="af2c8-112">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="af2c8-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="af2c8-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="af2c8-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="af2c8-114">读取固定到频道的一个选项卡。</span><span class="sxs-lookup"><span data-stu-id="af2c8-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="af2c8-115">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="af2c8-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="af2c8-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="af2c8-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="af2c8-117">添加 (pin) 通道向选项卡。</span><span class="sxs-lookup"><span data-stu-id="af2c8-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="af2c8-118">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="af2c8-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="af2c8-119">无</span><span class="sxs-lookup"><span data-stu-id="af2c8-119">None</span></span> | <span data-ttu-id="af2c8-120">删除 （取消锁定） 通道从选项卡。</span><span class="sxs-lookup"><span data-stu-id="af2c8-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="af2c8-121">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="af2c8-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="af2c8-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="af2c8-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="af2c8-123">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="af2c8-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="af2c8-124">属性</span><span class="sxs-lookup"><span data-stu-id="af2c8-124">Properties</span></span>

|<span data-ttu-id="af2c8-125">属性</span><span class="sxs-lookup"><span data-stu-id="af2c8-125">Property</span></span>|<span data-ttu-id="af2c8-126">类型</span><span class="sxs-lookup"><span data-stu-id="af2c8-126">Type</span></span>|<span data-ttu-id="af2c8-127">说明</span><span class="sxs-lookup"><span data-stu-id="af2c8-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="af2c8-128">id</span><span class="sxs-lookup"><span data-stu-id="af2c8-128">id</span></span>              |   <span data-ttu-id="af2c8-129">string</span><span class="sxs-lookup"><span data-stu-id="af2c8-129">string</span></span>                  |  <span data-ttu-id="af2c8-130">唯一标识通道选项读取仅的特定实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="af2c8-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="af2c8-131">displayName</span><span class="sxs-lookup"><span data-stu-id="af2c8-131">displayName</span></span>            |   <span data-ttu-id="af2c8-132">string</span><span class="sxs-lookup"><span data-stu-id="af2c8-132">string</span></span>                  |  <span data-ttu-id="af2c8-133">Tab 的名称。</span><span class="sxs-lookup"><span data-stu-id="af2c8-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="af2c8-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="af2c8-134">webUrl</span></span>          |   <span data-ttu-id="af2c8-135">string</span><span class="sxs-lookup"><span data-stu-id="af2c8-135">string</span></span>                  |  <span data-ttu-id="af2c8-136">深度链接的选项卡实例的 url。</span><span class="sxs-lookup"><span data-stu-id="af2c8-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="af2c8-137">只读。</span><span class="sxs-lookup"><span data-stu-id="af2c8-137">Read only.</span></span>     |
|  <span data-ttu-id="af2c8-138">configuration</span><span class="sxs-lookup"><span data-stu-id="af2c8-138">configuration</span></span>        |   [<span data-ttu-id="af2c8-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="af2c8-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="af2c8-140">应用于选项卡的自定义设置的容器。配置仅后设置此属性时，才视为选项卡。</span><span class="sxs-lookup"><span data-stu-id="af2c8-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="af2c8-141">关系</span><span class="sxs-lookup"><span data-stu-id="af2c8-141">Relationships</span></span>

| <span data-ttu-id="af2c8-142">关系</span><span class="sxs-lookup"><span data-stu-id="af2c8-142">Relationship</span></span> | <span data-ttu-id="af2c8-143">类型</span><span class="sxs-lookup"><span data-stu-id="af2c8-143">Type</span></span>   | <span data-ttu-id="af2c8-144">说明</span><span class="sxs-lookup"><span data-stu-id="af2c8-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="af2c8-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="af2c8-145">teamsApp</span></span>|[<span data-ttu-id="af2c8-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="af2c8-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="af2c8-147">应用程序的链接到选项卡。这不能更改选项卡创建后。</span><span class="sxs-lookup"><span data-stu-id="af2c8-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="af2c8-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af2c8-148">JSON representation</span></span>

<span data-ttu-id="af2c8-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af2c8-149">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="af2c8-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="af2c8-150">See also</span></span>

[<span data-ttu-id="af2c8-151">配置到内置选项卡的类型</span><span class="sxs-lookup"><span data-stu-id="af2c8-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
