---
title: schedulingGroup 资源类型
description: 计划中成员的逻辑分组（通常按角色）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 9f4f494b21a1139ba9a9e0771dcbc41d363bab2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965297"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="07e10-103">schedulingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="07e10-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e10-104">[计划](schedule.md)中成员的逻辑分组（通常按角色）。</span><span class="sxs-lookup"><span data-stu-id="07e10-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="07e10-105">方法</span><span class="sxs-lookup"><span data-stu-id="07e10-105">Methods</span></span>

| <span data-ttu-id="07e10-106">方法</span><span class="sxs-lookup"><span data-stu-id="07e10-106">Method</span></span>       | <span data-ttu-id="07e10-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="07e10-107">Return Type</span></span>  |<span data-ttu-id="07e10-108">说明</span><span class="sxs-lookup"><span data-stu-id="07e10-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07e10-109">创建 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="07e10-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="07e10-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="07e10-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="07e10-111">新建 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="07e10-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="07e10-112">列出 schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="07e10-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="07e10-113">[schedulingGroup](schedulinggroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07e10-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="07e10-114">获取计划中 `schedulingGroups` 的列表。</span><span class="sxs-lookup"><span data-stu-id="07e10-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="07e10-115">获取 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="07e10-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="07e10-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="07e10-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="07e10-117">按 ID 获取 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="07e10-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="07e10-118">更换 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="07e10-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="07e10-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="07e10-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="07e10-120">更换 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="07e10-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="07e10-121">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="07e10-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="07e10-122">无</span><span class="sxs-lookup"><span data-stu-id="07e10-122">None</span></span> | <span data-ttu-id="07e10-123">将 `schedulingGroup` 标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="07e10-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="07e10-124">属性</span><span class="sxs-lookup"><span data-stu-id="07e10-124">Properties</span></span>
|<span data-ttu-id="07e10-125">名称</span><span class="sxs-lookup"><span data-stu-id="07e10-125">Name</span></span>          |<span data-ttu-id="07e10-126">类型</span><span class="sxs-lookup"><span data-stu-id="07e10-126">Type</span></span>           |<span data-ttu-id="07e10-127">说明</span><span class="sxs-lookup"><span data-stu-id="07e10-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="07e10-128">id</span><span class="sxs-lookup"><span data-stu-id="07e10-128">id</span></span>            | `string`      |<span data-ttu-id="07e10-129">`schedulingGroup` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="07e10-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="07e10-130">displayName</span><span class="sxs-lookup"><span data-stu-id="07e10-130">displayName</span></span>   | `string`      | <span data-ttu-id="07e10-131">`schedulingGroup` 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="07e10-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="07e10-132">必需。</span><span class="sxs-lookup"><span data-stu-id="07e10-132">Required.</span></span> |
| <span data-ttu-id="07e10-133">isActive</span><span class="sxs-lookup"><span data-stu-id="07e10-133">isActive</span></span>          |`bool`      | <span data-ttu-id="07e10-134">指示在新建实体或更新现有实体时是否可以使用 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="07e10-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="07e10-135">必需。</span><span class="sxs-lookup"><span data-stu-id="07e10-135">Required.</span></span> |
| <span data-ttu-id="07e10-136">userIds</span><span class="sxs-lookup"><span data-stu-id="07e10-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="07e10-137">`schedulingGroup` 成员的用户 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="07e10-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="07e10-138">必需。</span><span class="sxs-lookup"><span data-stu-id="07e10-138">Required.</span></span> |
| <span data-ttu-id="07e10-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07e10-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="07e10-140">首次创建 `schedulingGroup` 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="07e10-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="07e10-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="07e10-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07e10-142">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="07e10-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="07e10-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07e10-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="07e10-144">上次更新 `schedulingGroup` 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="07e10-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="07e10-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="07e10-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07e10-146">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="07e10-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="07e10-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="07e10-147">lastModifiedBy</span></span>        | [<span data-ttu-id="07e10-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="07e10-148">identitySet</span></span>](identityset.md) |<span data-ttu-id="07e10-149">上次更新 `schedulingGroup` 的标识。</span><span class="sxs-lookup"><span data-stu-id="07e10-149">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07e10-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07e10-150">JSON representation</span></span>

<span data-ttu-id="07e10-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07e10-151">Here is a JSON representation of the resource.</span></span>

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
