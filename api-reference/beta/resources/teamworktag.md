---
title: teamworkTag 资源类型
description: 表示与团队关联的标记。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: fc732ce340f8ab8a3460c16900c4aff2d381744e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059881"
---
# <a name="teamworktag-resource-type"></a><span data-ttu-id="e2ab3-103">teamworkTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2ab3-103">teamworkTag resource type</span></span>

<span data-ttu-id="e2ab3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2ab3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2ab3-105">表示与团队关联的标记。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-105">Represents a tag associated with a team.</span></span> 

<span data-ttu-id="e2ab3-106">标签为客户提供了一种灵活的方法，可以基于团队中的常见属性对用户或组进行分类。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-106">Tags provide a flexible way for customers to classify users or groups based on a common attribute within a team.</span></span> <span data-ttu-id="e2ab3-107">例如，通过一个"百年"或"经理"或"设计器"标记，用户可以访问 Teams 中的各组人员，而无需键入每个名称。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-107">For example, a Nurse or Manager or Designer tag will enable users to reach groups of people in Teams without having to type every single name.</span></span>

<span data-ttu-id="e2ab3-108">添加标记后，用户可以在@mention添加标记。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-108">When a tag is added, users can @mention it in a channel.</span></span> <span data-ttu-id="e2ab3-109">分配了该标记的每个人都将收到通知，就像他们单独接收@mentioned一样。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-109">Everyone who has been assigned that tag will receive a notification just as they would if they were @mentioned individually.</span></span> <span data-ttu-id="e2ab3-110">用户还可使用 标记启动具有该标记成员的新聊天。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-110">Users can also use a tag is to start a new chat with the members of that tag.</span></span>

## <a name="methods"></a><span data-ttu-id="e2ab3-111">方法</span><span class="sxs-lookup"><span data-stu-id="e2ab3-111">Methods</span></span>
|<span data-ttu-id="e2ab3-112">方法</span><span class="sxs-lookup"><span data-stu-id="e2ab3-112">Method</span></span>|<span data-ttu-id="e2ab3-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2ab3-113">Return type</span></span>|<span data-ttu-id="e2ab3-114">说明</span><span class="sxs-lookup"><span data-stu-id="e2ab3-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2ab3-115">列出团队合作标记</span><span class="sxs-lookup"><span data-stu-id="e2ab3-115">List teamworkTags</span></span>](../api/teamworktag-list.md)|<span data-ttu-id="e2ab3-116">**teamworkTag** 集合</span><span class="sxs-lookup"><span data-stu-id="e2ab3-116">**teamworkTag** collection</span></span>|<span data-ttu-id="e2ab3-117">获取 **teamworkTag 对象** 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-117">Get a list of the **teamworkTag** objects and their properties.</span></span>|
|[<span data-ttu-id="e2ab3-118">创建团队合作标记</span><span class="sxs-lookup"><span data-stu-id="e2ab3-118">Create teamworkTag</span></span>](../api/teamworktag-post.md)|<span data-ttu-id="e2ab3-119">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="e2ab3-119">**teamworkTag**</span></span>|<span data-ttu-id="e2ab3-120">创建新的 **团队合作标记** 对象。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-120">Create a new **teamworkTag** object.</span></span>|
|[<span data-ttu-id="e2ab3-121">获取团队合作标记</span><span class="sxs-lookup"><span data-stu-id="e2ab3-121">Get teamworkTag</span></span>](../api/teamworktag-get.md)|<span data-ttu-id="e2ab3-122">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="e2ab3-122">**teamworkTag**</span></span>|<span data-ttu-id="e2ab3-123">读取团队合作Tag 对象 **的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-123">Read the properties and relationships of a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="e2ab3-124">更新团队合作标记</span><span class="sxs-lookup"><span data-stu-id="e2ab3-124">Update teamworkTag</span></span>](../api/teamworktag-update.md)|<span data-ttu-id="e2ab3-125">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="e2ab3-125">**teamworkTag**</span></span>|<span data-ttu-id="e2ab3-126">更新团队合作 **Tag 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-126">Update the properties of a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="e2ab3-127">删除团队合作标记</span><span class="sxs-lookup"><span data-stu-id="e2ab3-127">Delete teamworkTag</span></span>](../api/teamworktag-delete.md)|<span data-ttu-id="e2ab3-128">无</span><span class="sxs-lookup"><span data-stu-id="e2ab3-128">None</span></span>|<span data-ttu-id="e2ab3-129">删除 **团队合作标记** 对象。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-129">Delete a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="e2ab3-130">列出 teamworkTagMembers</span><span class="sxs-lookup"><span data-stu-id="e2ab3-130">List teamworkTagMembers</span></span>](../api/teamworktagmember-list.md)|<span data-ttu-id="e2ab3-131">**teamworkTagMember** 集合</span><span class="sxs-lookup"><span data-stu-id="e2ab3-131">**teamworkTagMember** collection</span></span>|<span data-ttu-id="e2ab3-132">获取团队中标准标记的成员及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-132">Get a list of the members of a standard tag in a team and their properties.</span></span>|
|[<span data-ttu-id="e2ab3-133">获取 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="e2ab3-133">Get teamworkTagMember</span></span>](../api/teamworktagmember-get.md)|<span data-ttu-id="e2ab3-134">**teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="e2ab3-134">**teamworkTagMember**</span></span>|<span data-ttu-id="e2ab3-135">获取团队中标准标记的成员的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-135">Get the properties and relationships of a member of a standard tag in a team.</span></span>|
|[<span data-ttu-id="e2ab3-136">删除 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="e2ab3-136">Delete teamworkTagMember</span></span>](../api/teamworktagmember-delete.md)|<span data-ttu-id="e2ab3-137">无</span><span class="sxs-lookup"><span data-stu-id="e2ab3-137">None</span></span>|<span data-ttu-id="e2ab3-138">从团队中的标准标记中删除成员。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-138">Delete a member from a standard tag in the team.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2ab3-139">属性</span><span class="sxs-lookup"><span data-stu-id="e2ab3-139">Properties</span></span>
|<span data-ttu-id="e2ab3-140">属性</span><span class="sxs-lookup"><span data-stu-id="e2ab3-140">Property</span></span>|<span data-ttu-id="e2ab3-141">类型</span><span class="sxs-lookup"><span data-stu-id="e2ab3-141">Type</span></span>|<span data-ttu-id="e2ab3-142">说明</span><span class="sxs-lookup"><span data-stu-id="e2ab3-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ab3-143">说明</span><span class="sxs-lookup"><span data-stu-id="e2ab3-143">description</span></span>|<span data-ttu-id="e2ab3-144">String</span><span class="sxs-lookup"><span data-stu-id="e2ab3-144">String</span></span>|<span data-ttu-id="e2ab3-145">标记说明，因为它将显示在用户Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-145">Tag description as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="e2ab3-146">displayName</span><span class="sxs-lookup"><span data-stu-id="e2ab3-146">displayName</span></span>|<span data-ttu-id="e2ab3-147">String</span><span class="sxs-lookup"><span data-stu-id="e2ab3-147">String</span></span>|<span data-ttu-id="e2ab3-148">标记名称，因为它将显示在用户Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-148">Tag name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="e2ab3-149">id</span><span class="sxs-lookup"><span data-stu-id="e2ab3-149">id</span></span>|<span data-ttu-id="e2ab3-150">String</span><span class="sxs-lookup"><span data-stu-id="e2ab3-150">String</span></span>|<span data-ttu-id="e2ab3-151">标记的 ID。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-151">ID of the tag.</span></span>|
|<span data-ttu-id="e2ab3-152">memberCount</span><span class="sxs-lookup"><span data-stu-id="e2ab3-152">memberCount</span></span>|<span data-ttu-id="e2ab3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ab3-153">Int32</span></span>|<span data-ttu-id="e2ab3-154">分配给标记的用户数。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-154">The number of users assigned to the tag.</span></span>|
|<span data-ttu-id="e2ab3-155">tagType</span><span class="sxs-lookup"><span data-stu-id="e2ab3-155">tagType</span></span>|<span data-ttu-id="e2ab3-156">teamworkTagType</span><span class="sxs-lookup"><span data-stu-id="e2ab3-156">teamworkTagType</span></span>|<span data-ttu-id="e2ab3-157">标记的类型。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-157">The type of tag.</span></span> <span data-ttu-id="e2ab3-158">默认值为标准。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-158">Default is standard.</span></span>|
|<span data-ttu-id="e2ab3-159">teamId</span><span class="sxs-lookup"><span data-stu-id="e2ab3-159">teamId</span></span>|<span data-ttu-id="e2ab3-160">String</span><span class="sxs-lookup"><span data-stu-id="e2ab3-160">String</span></span>|<span data-ttu-id="e2ab3-161">定义标记的团队的 ID。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-161">ID of the team in which the tag is defined.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ab3-162">关系</span><span class="sxs-lookup"><span data-stu-id="e2ab3-162">Relationships</span></span>
|<span data-ttu-id="e2ab3-163">关系</span><span class="sxs-lookup"><span data-stu-id="e2ab3-163">Relationship</span></span>|<span data-ttu-id="e2ab3-164">类型</span><span class="sxs-lookup"><span data-stu-id="e2ab3-164">Type</span></span>|<span data-ttu-id="e2ab3-165">说明</span><span class="sxs-lookup"><span data-stu-id="e2ab3-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ab3-166">成员</span><span class="sxs-lookup"><span data-stu-id="e2ab3-166">members</span></span>|<span data-ttu-id="e2ab3-167">[teamworkTagMember](../resources/teamworktagmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2ab3-167">[teamworkTagMember](../resources/teamworktagmember.md) collection</span></span>|<span data-ttu-id="e2ab3-168">分配给标记的用户。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-168">Users assigned to the tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2ab3-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2ab3-169">JSON representation</span></span>
<span data-ttu-id="e2ab3-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2ab3-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkTag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "String (identifier)",
  "teamId": "String",
  "displayName": "String",
  "memberCount": "Integer",
  "tagType": "String"
}
```

