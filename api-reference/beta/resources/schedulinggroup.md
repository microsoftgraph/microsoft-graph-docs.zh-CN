---
title: schedulingGroup 资源类型
description: 计划中成员的逻辑分组（通常按角色）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562946"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="ca27f-103">schedulingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca27f-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca27f-104">[计划](schedule.md)中成员的逻辑分组（通常按角色）。</span><span class="sxs-lookup"><span data-stu-id="ca27f-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="ca27f-105">方法</span><span class="sxs-lookup"><span data-stu-id="ca27f-105">Methods</span></span>

| <span data-ttu-id="ca27f-106">方法</span><span class="sxs-lookup"><span data-stu-id="ca27f-106">Method</span></span>       | <span data-ttu-id="ca27f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca27f-107">Return Type</span></span>  |<span data-ttu-id="ca27f-108">说明</span><span class="sxs-lookup"><span data-stu-id="ca27f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca27f-109">创建 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ca27f-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="ca27f-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ca27f-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="ca27f-111">新建 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="ca27f-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="ca27f-112">列出 schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="ca27f-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="ca27f-113">[schedulingGroup](schedulinggroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca27f-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="ca27f-114">获取计划中 `schedulingGroups` 的列表。</span><span class="sxs-lookup"><span data-stu-id="ca27f-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="ca27f-115">获取 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ca27f-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="ca27f-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ca27f-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="ca27f-117">按 ID 获取 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="ca27f-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="ca27f-118">更换 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ca27f-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="ca27f-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ca27f-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="ca27f-120">更换 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="ca27f-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="ca27f-121">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ca27f-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="ca27f-122">无</span><span class="sxs-lookup"><span data-stu-id="ca27f-122">None</span></span> | <span data-ttu-id="ca27f-123">将 `schedulingGroup` 标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="ca27f-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca27f-124">属性</span><span class="sxs-lookup"><span data-stu-id="ca27f-124">Properties</span></span>
|<span data-ttu-id="ca27f-125">名称</span><span class="sxs-lookup"><span data-stu-id="ca27f-125">Name</span></span>          |<span data-ttu-id="ca27f-126">类型</span><span class="sxs-lookup"><span data-stu-id="ca27f-126">Type</span></span>           |<span data-ttu-id="ca27f-127">说明</span><span class="sxs-lookup"><span data-stu-id="ca27f-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="ca27f-128">id</span><span class="sxs-lookup"><span data-stu-id="ca27f-128">id</span></span>            | `string`      |<span data-ttu-id="ca27f-129">`schedulingGroup` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="ca27f-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="ca27f-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ca27f-130">displayName</span></span>   | `string`      | <span data-ttu-id="ca27f-131">`schedulingGroup` 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ca27f-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="ca27f-132">必需。</span><span class="sxs-lookup"><span data-stu-id="ca27f-132">Required.</span></span> |
| <span data-ttu-id="ca27f-133">isActive</span><span class="sxs-lookup"><span data-stu-id="ca27f-133">isActive</span></span>          |`bool`      | <span data-ttu-id="ca27f-134">指示在新建实体或更新现有实体时是否可以使用 `schedulingGroup`。</span><span class="sxs-lookup"><span data-stu-id="ca27f-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="ca27f-135">必需。</span><span class="sxs-lookup"><span data-stu-id="ca27f-135">Required.</span></span> |
| <span data-ttu-id="ca27f-136">userIds</span><span class="sxs-lookup"><span data-stu-id="ca27f-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="ca27f-137">`schedulingGroup` 成员的用户 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="ca27f-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="ca27f-138">必需。</span><span class="sxs-lookup"><span data-stu-id="ca27f-138">Required.</span></span> |
| <span data-ttu-id="ca27f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca27f-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="ca27f-140">首次创建 `schedulingGroup` 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ca27f-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="ca27f-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ca27f-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ca27f-142">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="ca27f-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ca27f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca27f-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="ca27f-144">上次更新 `schedulingGroup` 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ca27f-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="ca27f-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ca27f-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ca27f-146">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="ca27f-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ca27f-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ca27f-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="ca27f-148">上次更新 `schedulingGroup` 的标识。</span><span class="sxs-lookup"><span data-stu-id="ca27f-148">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca27f-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca27f-149">JSON representation</span></span>

<span data-ttu-id="ca27f-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca27f-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
