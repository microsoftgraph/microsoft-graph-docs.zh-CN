---
title: schedulingGroup 资源类型
description: 计划中成员的逻辑分组（通常按角色）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: db86b22f61b7293683a775460cb3678af7ca4f5a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985803"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="8c3d9-103">schedulingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c3d9-103">schedulingGroup resource type</span></span>

<span data-ttu-id="8c3d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c3d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c3d9-105">[计划](schedule.md)中成员的逻辑分组（通常按角色）。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-105">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="8c3d9-106">方法</span><span class="sxs-lookup"><span data-stu-id="8c3d9-106">Methods</span></span>

| <span data-ttu-id="8c3d9-107">方法</span><span class="sxs-lookup"><span data-stu-id="8c3d9-107">Method</span></span>       | <span data-ttu-id="8c3d9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c3d9-108">Return Type</span></span>  |<span data-ttu-id="8c3d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="8c3d9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c3d9-110">创建 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8c3d9-110">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="8c3d9-111">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8c3d9-111">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="8c3d9-112">新建 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-112">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="8c3d9-113">列出 schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="8c3d9-113">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="8c3d9-114">[schedulingGroup](schedulinggroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8c3d9-114">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="8c3d9-115">获取计划中 `schedulingGroups` 的列表。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-115">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="8c3d9-116">获取 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8c3d9-116">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="8c3d9-117">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8c3d9-117">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="8c3d9-118">按 ID 获取 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-118">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="8c3d9-119">更换 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8c3d9-119">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="8c3d9-120">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8c3d9-120">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="8c3d9-121">更换 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-121">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="8c3d9-122">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8c3d9-122">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="8c3d9-123">无</span><span class="sxs-lookup"><span data-stu-id="8c3d9-123">None</span></span> | <span data-ttu-id="8c3d9-124">将 `schedulingGroup` 标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-124">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c3d9-125">属性</span><span class="sxs-lookup"><span data-stu-id="8c3d9-125">Properties</span></span>
|<span data-ttu-id="8c3d9-126">名称</span><span class="sxs-lookup"><span data-stu-id="8c3d9-126">Name</span></span>          |<span data-ttu-id="8c3d9-127">类型</span><span class="sxs-lookup"><span data-stu-id="8c3d9-127">Type</span></span>           |<span data-ttu-id="8c3d9-128">说明</span><span class="sxs-lookup"><span data-stu-id="8c3d9-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="8c3d9-129">id</span><span class="sxs-lookup"><span data-stu-id="8c3d9-129">id</span></span>            | `string`      |<span data-ttu-id="8c3d9-130">`schedulingGroup` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-130">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="8c3d9-131">displayName</span><span class="sxs-lookup"><span data-stu-id="8c3d9-131">displayName</span></span>   | `string`      | <span data-ttu-id="8c3d9-132">`schedulingGroup` 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-132">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="8c3d9-133">必需。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-133">Required.</span></span> |
| <span data-ttu-id="8c3d9-134">isActive</span><span class="sxs-lookup"><span data-stu-id="8c3d9-134">isActive</span></span>          |`bool`      | <span data-ttu-id="8c3d9-135">指示在新建实体或更新现有实体时是否可以使用 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-135">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="8c3d9-136">必需。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-136">Required.</span></span> |
| <span data-ttu-id="8c3d9-137">userIds</span><span class="sxs-lookup"><span data-stu-id="8c3d9-137">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="8c3d9-138">`schedulingGroup` 成员的用户 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-138">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="8c3d9-139">必需。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-139">Required.</span></span> |
| <span data-ttu-id="8c3d9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c3d9-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="8c3d9-141">首次创建 `schedulingGroup` 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-141">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="8c3d9-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8c3d9-143">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8c3d9-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c3d9-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="8c3d9-145">上次更新 `schedulingGroup` 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-145">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="8c3d9-146">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8c3d9-147">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8c3d9-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8c3d9-148">lastModifiedBy</span></span>        | [<span data-ttu-id="8c3d9-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="8c3d9-149">identitySet</span></span>](identityset.md) |<span data-ttu-id="8c3d9-150">上次更新 `schedulingGroup` 的标识。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-150">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c3d9-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c3d9-151">JSON representation</span></span>

<span data-ttu-id="8c3d9-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c3d9-152">Here is a JSON representation of the resource.</span></span>

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


