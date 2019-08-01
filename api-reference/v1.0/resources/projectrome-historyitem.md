---
title: historyItem 资源类型
description: 表示应用中的活动的历史记录项。 用户活动表示应用程序中的单个目标, 例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时, 会将该预订作为历史项目进行捕获, 以指示该活动的开始时间和结束时间。 随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 38cba88a5605e1c67ae84b684425db3c71f5d51c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035005"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="45d64-106">historyItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="45d64-106">historyItem resource type</span></span>

<span data-ttu-id="45d64-107">表示应用中的[活动](projectrome-activity.md)的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="45d64-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="45d64-108">用户活动表示应用程序中的单个目标, 例如电视节目、文档或视频游戏中的当前市场活动。</span><span class="sxs-lookup"><span data-stu-id="45d64-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="45d64-109">当用户参与该活动时, 会将该预订作为历史项目进行捕获, 以指示该活动的开始时间和结束时间。</span><span class="sxs-lookup"><span data-stu-id="45d64-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="45d64-110">随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。</span><span class="sxs-lookup"><span data-stu-id="45d64-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="45d64-111">当应用程序创建会话时, 应将一个**historyItem**对象添加到**活动**对象, 以反映用户参与的时段。</span><span class="sxs-lookup"><span data-stu-id="45d64-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="45d64-112">用户每次重新参与活动时, 都会向活动中添加一个新的**historyItem**以计入用户约定。</span><span class="sxs-lookup"><span data-stu-id="45d64-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="45d64-113">方法</span><span class="sxs-lookup"><span data-stu-id="45d64-113">Methods</span></span>

|<span data-ttu-id="45d64-114">方法</span><span class="sxs-lookup"><span data-stu-id="45d64-114">Method</span></span> | <span data-ttu-id="45d64-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="45d64-115">Return Type</span></span> | <span data-ttu-id="45d64-116">说明</span><span class="sxs-lookup"><span data-stu-id="45d64-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="45d64-117">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="45d64-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="45d64-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="45d64-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="45d64-119">创建或替换该活动的现有**historyItem** (upsert)。</span><span class="sxs-lookup"><span data-stu-id="45d64-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="45d64-120">ID 必须是 GUID。</span><span class="sxs-lookup"><span data-stu-id="45d64-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="45d64-121">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="45d64-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="45d64-122">无内容</span><span class="sxs-lookup"><span data-stu-id="45d64-122">No Content</span></span> | <span data-ttu-id="45d64-123">删除该活动的指定**historyItem** 。</span><span class="sxs-lookup"><span data-stu-id="45d64-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="45d64-124">属性</span><span class="sxs-lookup"><span data-stu-id="45d64-124">Properties</span></span>

|<span data-ttu-id="45d64-125">名称</span><span class="sxs-lookup"><span data-stu-id="45d64-125">Name</span></span> | <span data-ttu-id="45d64-126">类型</span><span class="sxs-lookup"><span data-stu-id="45d64-126">Type</span></span> | <span data-ttu-id="45d64-127">说明</span><span class="sxs-lookup"><span data-stu-id="45d64-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="45d64-128">状态</span><span class="sxs-lookup"><span data-stu-id="45d64-128">status</span></span> | <span data-ttu-id="45d64-129">status</span><span class="sxs-lookup"><span data-stu-id="45d64-129">status</span></span> | <span data-ttu-id="45d64-130">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="45d64-130">Set by the server.</span></span> <span data-ttu-id="45d64-131">用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="45d64-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="45d64-132">值: 活动、已更新、已删除、已忽略。</span><span class="sxs-lookup"><span data-stu-id="45d64-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="45d64-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="45d64-133">userTimezone</span></span> | <span data-ttu-id="45d64-134">String</span><span class="sxs-lookup"><span data-stu-id="45d64-134">String</span></span> | <span data-ttu-id="45d64-135">可选。</span><span class="sxs-lookup"><span data-stu-id="45d64-135">Optional.</span></span> <span data-ttu-id="45d64-136">用于生成活动的用户设备所在的时区位于活动创建时间。</span><span class="sxs-lookup"><span data-stu-id="45d64-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="45d64-137">作为 Olson Id 提供的值, 以便支持跨平台表示形式。</span><span class="sxs-lookup"><span data-stu-id="45d64-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="45d64-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45d64-138">createdDateTime</span></span> | <span data-ttu-id="45d64-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45d64-139">DateTimeOffset</span></span> | <span data-ttu-id="45d64-140">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="45d64-140">Set by the server.</span></span> <span data-ttu-id="45d64-141">在服务器上创建对象时的 UTC 时间 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="45d64-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="45d64-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45d64-142">lastModifiedDateTime</span></span> | <span data-ttu-id="45d64-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45d64-143">DateTimeOffset</span></span> | <span data-ttu-id="45d64-144">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="45d64-144">Set by the server.</span></span> <span data-ttu-id="45d64-145">在服务器上修改对象时的 UTC 时间 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="45d64-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="45d64-146">id</span><span class="sxs-lookup"><span data-stu-id="45d64-146">id</span></span> | <span data-ttu-id="45d64-147">String</span><span class="sxs-lookup"><span data-stu-id="45d64-147">String</span></span> | <span data-ttu-id="45d64-148">必需。</span><span class="sxs-lookup"><span data-stu-id="45d64-148">Required.</span></span> <span data-ttu-id="45d64-149">客户端集的**historyItem**对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="45d64-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="45d64-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="45d64-150">startedDateTime</span></span> | <span data-ttu-id="45d64-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45d64-151">DateTimeOffset</span></span> | <span data-ttu-id="45d64-152">必需。</span><span class="sxs-lookup"><span data-stu-id="45d64-152">Required.</span></span> <span data-ttu-id="45d64-153">**HistoryItem** (活动会话) 启动时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="45d64-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="45d64-154">对于时间线历史记录是必需的。</span><span class="sxs-lookup"><span data-stu-id="45d64-154">Required for timeline history.</span></span>|
|<span data-ttu-id="45d64-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="45d64-155">lastActiveDateTime</span></span> | <span data-ttu-id="45d64-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45d64-156">DateTimeOffset</span></span> | <span data-ttu-id="45d64-157">可选。</span><span class="sxs-lookup"><span data-stu-id="45d64-157">Optional.</span></span> <span data-ttu-id="45d64-158">UTC DateTime 如果**historyItem** (活动会话) 上次被视为活动或已完成-如果为 null, 则**historyItem**状态应为 "正在进行"。</span><span class="sxs-lookup"><span data-stu-id="45d64-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="45d64-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="45d64-159">expirationDateTime</span></span> | <span data-ttu-id="45d64-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45d64-160">DateTimeOffset</span></span> | <span data-ttu-id="45d64-161">可选。</span><span class="sxs-lookup"><span data-stu-id="45d64-161">Optional.</span></span> <span data-ttu-id="45d64-162">**HistoryItem**将被硬删除时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="45d64-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="45d64-163">可由客户端进行设置。</span><span class="sxs-lookup"><span data-stu-id="45d64-163">Can be set by the client.</span></span>|
|<span data-ttu-id="45d64-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="45d64-164">activeDurationSeconds</span></span> | <span data-ttu-id="45d64-165">int</span><span class="sxs-lookup"><span data-stu-id="45d64-165">int</span></span> | <span data-ttu-id="45d64-166">可选。</span><span class="sxs-lookup"><span data-stu-id="45d64-166">Optional.</span></span> <span data-ttu-id="45d64-167">活动用户约定的持续时间。</span><span class="sxs-lookup"><span data-stu-id="45d64-167">The duration of active user engagement.</span></span> <span data-ttu-id="45d64-168">如果未提供, 则从**startedDateTime**和**lastActiveDateTime**计算。</span><span class="sxs-lookup"><span data-stu-id="45d64-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45d64-169">关系</span><span class="sxs-lookup"><span data-stu-id="45d64-169">Relationships</span></span>

|<span data-ttu-id="45d64-170">关系</span><span class="sxs-lookup"><span data-stu-id="45d64-170">Relationship</span></span> | <span data-ttu-id="45d64-171">类型</span><span class="sxs-lookup"><span data-stu-id="45d64-171">Type</span></span> | <span data-ttu-id="45d64-172">说明</span><span class="sxs-lookup"><span data-stu-id="45d64-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="45d64-173">activity</span><span class="sxs-lookup"><span data-stu-id="45d64-173">activity</span></span>| [<span data-ttu-id="45d64-174">Useractivity.readwrite.createdbyapp</span><span class="sxs-lookup"><span data-stu-id="45d64-174">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="45d64-175">可选。</span><span class="sxs-lookup"><span data-stu-id="45d64-175">Optional.</span></span> <span data-ttu-id="45d64-176">NavigationProperty/包含;指向关联活动的导航属性。</span><span class="sxs-lookup"><span data-stu-id="45d64-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45d64-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45d64-177">JSON representation</span></span>

<span data-ttu-id="45d64-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45d64-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
