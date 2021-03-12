---
title: schedulingGroup 资源类型
description: 计划中成员的逻辑分组（通常按角色）。
author: akumar39
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 018359ab0dd6702a2fda40bf5f0b29c639211f4a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719302"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="537ce-103">schedulingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="537ce-103">schedulingGroup resource type</span></span>

<span data-ttu-id="537ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="537ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="537ce-105">[计划](schedule.md)中成员的逻辑分组（通常按角色）。</span><span class="sxs-lookup"><span data-stu-id="537ce-105">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="537ce-106">方法</span><span class="sxs-lookup"><span data-stu-id="537ce-106">Methods</span></span>

| <span data-ttu-id="537ce-107">方法</span><span class="sxs-lookup"><span data-stu-id="537ce-107">Method</span></span>       | <span data-ttu-id="537ce-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="537ce-108">Return Type</span></span>  |<span data-ttu-id="537ce-109">Description</span><span class="sxs-lookup"><span data-stu-id="537ce-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="537ce-110">List</span><span class="sxs-lookup"><span data-stu-id="537ce-110">List</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="537ce-111">[schedulingGroup](schedulinggroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="537ce-111">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="537ce-112">获取计划中的 **schedulingGroups** 列表。</span><span class="sxs-lookup"><span data-stu-id="537ce-112">Get the list of **schedulingGroups** in a schedule.</span></span>|
|[<span data-ttu-id="537ce-113">Create</span><span class="sxs-lookup"><span data-stu-id="537ce-113">Create</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="537ce-114">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="537ce-114">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="537ce-115">新建 **schedulingGroup**。</span><span class="sxs-lookup"><span data-stu-id="537ce-115">Create a new **schedulingGroup**.</span></span>|
|[<span data-ttu-id="537ce-116">Get</span><span class="sxs-lookup"><span data-stu-id="537ce-116">Get</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="537ce-117">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="537ce-117">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="537ce-118">按 ID 获取 **schedulingGroup**。</span><span class="sxs-lookup"><span data-stu-id="537ce-118">Get a **schedulingGroup** by ID.</span></span>|
|[<span data-ttu-id="537ce-119">删除</span><span class="sxs-lookup"><span data-stu-id="537ce-119">Delete</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="537ce-120">无</span><span class="sxs-lookup"><span data-stu-id="537ce-120">None</span></span> | <span data-ttu-id="537ce-121">将 **schedulingGroup** 标记为非活动。</span><span class="sxs-lookup"><span data-stu-id="537ce-121">Mark **schedulingGroup** as inactive.</span></span>|
|[<span data-ttu-id="537ce-122">Replace</span><span class="sxs-lookup"><span data-stu-id="537ce-122">Replace</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="537ce-123">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="537ce-123">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="537ce-124">替换 **schedulingGroup**。</span><span class="sxs-lookup"><span data-stu-id="537ce-124">Replace a **schedulingGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="537ce-125">属性</span><span class="sxs-lookup"><span data-stu-id="537ce-125">Properties</span></span>
|<span data-ttu-id="537ce-126">名称</span><span class="sxs-lookup"><span data-stu-id="537ce-126">Name</span></span>          |<span data-ttu-id="537ce-127">类型</span><span class="sxs-lookup"><span data-stu-id="537ce-127">Type</span></span>           |<span data-ttu-id="537ce-128">说明</span><span class="sxs-lookup"><span data-stu-id="537ce-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="537ce-129">id</span><span class="sxs-lookup"><span data-stu-id="537ce-129">id</span></span>            | `string`      |<span data-ttu-id="537ce-130">**schedulingGroup** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="537ce-130">ID of the **schedulingGroup**.</span></span>|
| <span data-ttu-id="537ce-131">displayName</span><span class="sxs-lookup"><span data-stu-id="537ce-131">displayName</span></span>   | `string`      | <span data-ttu-id="537ce-132">**schedulingGroup** 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="537ce-132">The display name for the **schedulingGroup**.</span></span> <span data-ttu-id="537ce-133">必填。</span><span class="sxs-lookup"><span data-stu-id="537ce-133">Required.</span></span> |
| <span data-ttu-id="537ce-134">isActive</span><span class="sxs-lookup"><span data-stu-id="537ce-134">isActive</span></span>          |`bool`      | <span data-ttu-id="537ce-135">指示在新建实体或更新现有实体时是否可以使用 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="537ce-135">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="537ce-136">必需。</span><span class="sxs-lookup"><span data-stu-id="537ce-136">Required.</span></span> |
| <span data-ttu-id="537ce-137">userIds</span><span class="sxs-lookup"><span data-stu-id="537ce-137">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="537ce-138">属于 **schedulingGroup** 成员的用户 ID 的列表。</span><span class="sxs-lookup"><span data-stu-id="537ce-138">The list of user IDs that are a member of the **schedulingGroup**.</span></span> <span data-ttu-id="537ce-139">必填。</span><span class="sxs-lookup"><span data-stu-id="537ce-139">Required.</span></span> |
| <span data-ttu-id="537ce-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="537ce-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="537ce-141">此 **schedulingGroup** 的首次创建时间戳。</span><span class="sxs-lookup"><span data-stu-id="537ce-141">The time stamp in which this **schedulingGroup** was first created.</span></span> <span data-ttu-id="537ce-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="537ce-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="537ce-143">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="537ce-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="537ce-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="537ce-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="537ce-145">此 **schedulingGroup** 的最后更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="537ce-145">The time stamp in which this **schedulingGroup** was last updated.</span></span> <span data-ttu-id="537ce-146">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="537ce-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="537ce-147">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="537ce-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="537ce-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="537ce-148">lastModifiedBy</span></span>        | [<span data-ttu-id="537ce-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="537ce-149">identitySet</span></span>](identityset.md) |<span data-ttu-id="537ce-150">最后更新此 **schedulingGroup** 的标识。</span><span class="sxs-lookup"><span data-stu-id="537ce-150">The identity that last updated this **schedulingGroup**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="537ce-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="537ce-151">JSON representation</span></span>

<span data-ttu-id="537ce-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="537ce-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "isActive": true,
  "userIds": ["String (identifier)"],
  "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

