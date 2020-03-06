---
title: historyItem 资源类型
description: 表示应用中的活动的历史记录项。 用户活动表示应用程序中的单个目标，例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时，会将该预订作为历史项目进行捕获，以指示该活动的开始时间和结束时间。 随着时间的推移，用户随着时间的推移而重新参与该活动，会为单个用户活动记录多个历史记录项目。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 4053811f1f44621b05830bf40b17d02e0112b455
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533948"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="ad03d-106">historyItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad03d-106">historyItem resource type</span></span>

<span data-ttu-id="ad03d-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad03d-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad03d-108">表示应用中的[活动](projectrome-activity.md)的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="ad03d-108">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="ad03d-109">用户活动表示应用程序中的单个目标，例如电视节目、文档或视频游戏中的当前市场活动。</span><span class="sxs-lookup"><span data-stu-id="ad03d-109">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="ad03d-110">当用户参与该活动时，会将该预订作为历史项目进行捕获，以指示该活动的开始时间和结束时间。</span><span class="sxs-lookup"><span data-stu-id="ad03d-110">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="ad03d-111">随着时间的推移，用户随着时间的推移而重新参与该活动，会为单个用户活动记录多个历史记录项目。</span><span class="sxs-lookup"><span data-stu-id="ad03d-111">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="ad03d-112">当应用程序创建会话时，应将一个**historyItem**对象添加到**活动**对象，以反映用户参与的时段。</span><span class="sxs-lookup"><span data-stu-id="ad03d-112">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="ad03d-113">用户每次重新参与活动时，都会向活动中添加一个新的**historyItem**以计入用户约定。</span><span class="sxs-lookup"><span data-stu-id="ad03d-113">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="ad03d-114">Methods</span><span class="sxs-lookup"><span data-stu-id="ad03d-114">Methods</span></span>

|<span data-ttu-id="ad03d-115">方法</span><span class="sxs-lookup"><span data-stu-id="ad03d-115">Method</span></span> | <span data-ttu-id="ad03d-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="ad03d-116">Return Type</span></span> | <span data-ttu-id="ad03d-117">说明</span><span class="sxs-lookup"><span data-stu-id="ad03d-117">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="ad03d-118">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="ad03d-118">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="ad03d-119">historyItem</span><span class="sxs-lookup"><span data-stu-id="ad03d-119">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="ad03d-120">创建或替换该活动的现有**historyItem** （upsert）。</span><span class="sxs-lookup"><span data-stu-id="ad03d-120">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="ad03d-121">ID 必须是 GUID。</span><span class="sxs-lookup"><span data-stu-id="ad03d-121">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="ad03d-122">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="ad03d-122">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="ad03d-123">无内容</span><span class="sxs-lookup"><span data-stu-id="ad03d-123">No Content</span></span> | <span data-ttu-id="ad03d-124">删除该活动的指定**historyItem** 。</span><span class="sxs-lookup"><span data-stu-id="ad03d-124">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad03d-125">属性</span><span class="sxs-lookup"><span data-stu-id="ad03d-125">Properties</span></span>

|<span data-ttu-id="ad03d-126">名称</span><span class="sxs-lookup"><span data-stu-id="ad03d-126">Name</span></span> | <span data-ttu-id="ad03d-127">类型</span><span class="sxs-lookup"><span data-stu-id="ad03d-127">Type</span></span> | <span data-ttu-id="ad03d-128">说明</span><span class="sxs-lookup"><span data-stu-id="ad03d-128">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ad03d-129">状态</span><span class="sxs-lookup"><span data-stu-id="ad03d-129">status</span></span> | <span data-ttu-id="ad03d-130">状态</span><span class="sxs-lookup"><span data-stu-id="ad03d-130">status</span></span> | <span data-ttu-id="ad03d-131">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="ad03d-131">Set by the server.</span></span> <span data-ttu-id="ad03d-132">用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="ad03d-132">A status code used to identify valid objects.</span></span> <span data-ttu-id="ad03d-133">值：活动、已更新、已删除、已忽略。</span><span class="sxs-lookup"><span data-stu-id="ad03d-133">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="ad03d-134">userTimezone</span><span class="sxs-lookup"><span data-stu-id="ad03d-134">userTimezone</span></span> | <span data-ttu-id="ad03d-135">String</span><span class="sxs-lookup"><span data-stu-id="ad03d-135">String</span></span> | <span data-ttu-id="ad03d-136">可选。</span><span class="sxs-lookup"><span data-stu-id="ad03d-136">Optional.</span></span> <span data-ttu-id="ad03d-137">用于生成活动的用户设备所在的时区位于活动创建时间。</span><span class="sxs-lookup"><span data-stu-id="ad03d-137">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="ad03d-138">作为 Olson Id 提供的值，以便支持跨平台表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad03d-138">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="ad03d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad03d-139">createdDateTime</span></span> | <span data-ttu-id="ad03d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad03d-140">DateTimeOffset</span></span> | <span data-ttu-id="ad03d-141">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="ad03d-141">Set by the server.</span></span> <span data-ttu-id="ad03d-142">在服务器上创建对象时的 UTC 时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="ad03d-142">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="ad03d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad03d-143">lastModifiedDateTime</span></span> | <span data-ttu-id="ad03d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad03d-144">DateTimeOffset</span></span> | <span data-ttu-id="ad03d-145">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="ad03d-145">Set by the server.</span></span> <span data-ttu-id="ad03d-146">在服务器上修改对象时的 UTC 时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="ad03d-146">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="ad03d-147">id</span><span class="sxs-lookup"><span data-stu-id="ad03d-147">id</span></span> | <span data-ttu-id="ad03d-148">字符串</span><span class="sxs-lookup"><span data-stu-id="ad03d-148">String</span></span> | <span data-ttu-id="ad03d-149">必需。</span><span class="sxs-lookup"><span data-stu-id="ad03d-149">Required.</span></span> <span data-ttu-id="ad03d-150">客户端集的**historyItem**对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="ad03d-150">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="ad03d-151">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad03d-151">startedDateTime</span></span> | <span data-ttu-id="ad03d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad03d-152">DateTimeOffset</span></span> | <span data-ttu-id="ad03d-153">必需。</span><span class="sxs-lookup"><span data-stu-id="ad03d-153">Required.</span></span> <span data-ttu-id="ad03d-154">**HistoryItem** （活动会话）启动时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="ad03d-154">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="ad03d-155">对于时间线历史记录是必需的。</span><span class="sxs-lookup"><span data-stu-id="ad03d-155">Required for timeline history.</span></span>|
|<span data-ttu-id="ad03d-156">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="ad03d-156">lastActiveDateTime</span></span> | <span data-ttu-id="ad03d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad03d-157">DateTimeOffset</span></span> | <span data-ttu-id="ad03d-158">可选。</span><span class="sxs-lookup"><span data-stu-id="ad03d-158">Optional.</span></span> <span data-ttu-id="ad03d-159">UTC DateTime 如果**historyItem** （活动会话）上次被视为活动或已完成-如果为 null，则**historyItem**状态应为 "正在进行"。</span><span class="sxs-lookup"><span data-stu-id="ad03d-159">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="ad03d-160">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ad03d-160">expirationDateTime</span></span> | <span data-ttu-id="ad03d-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad03d-161">DateTimeOffset</span></span> | <span data-ttu-id="ad03d-162">可选。</span><span class="sxs-lookup"><span data-stu-id="ad03d-162">Optional.</span></span> <span data-ttu-id="ad03d-163">**HistoryItem**将被硬删除时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="ad03d-163">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="ad03d-164">可由客户端进行设置。</span><span class="sxs-lookup"><span data-stu-id="ad03d-164">Can be set by the client.</span></span>|
|<span data-ttu-id="ad03d-165">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="ad03d-165">activeDurationSeconds</span></span> | <span data-ttu-id="ad03d-166">int</span><span class="sxs-lookup"><span data-stu-id="ad03d-166">int</span></span> | <span data-ttu-id="ad03d-167">可选。</span><span class="sxs-lookup"><span data-stu-id="ad03d-167">Optional.</span></span> <span data-ttu-id="ad03d-168">活动用户约定的持续时间。</span><span class="sxs-lookup"><span data-stu-id="ad03d-168">The duration of active user engagement.</span></span> <span data-ttu-id="ad03d-169">如果未提供，则从**startedDateTime**和**lastActiveDateTime**计算。</span><span class="sxs-lookup"><span data-stu-id="ad03d-169">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad03d-170">关系</span><span class="sxs-lookup"><span data-stu-id="ad03d-170">Relationships</span></span>

|<span data-ttu-id="ad03d-171">关系</span><span class="sxs-lookup"><span data-stu-id="ad03d-171">Relationship</span></span> | <span data-ttu-id="ad03d-172">类型</span><span class="sxs-lookup"><span data-stu-id="ad03d-172">Type</span></span> | <span data-ttu-id="ad03d-173">说明</span><span class="sxs-lookup"><span data-stu-id="ad03d-173">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="ad03d-174">activity</span><span class="sxs-lookup"><span data-stu-id="ad03d-174">activity</span></span>| [<span data-ttu-id="ad03d-175">Useractivity.readwrite.createdbyapp</span><span class="sxs-lookup"><span data-stu-id="ad03d-175">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="ad03d-176">可选。</span><span class="sxs-lookup"><span data-stu-id="ad03d-176">Optional.</span></span> <span data-ttu-id="ad03d-177">NavigationProperty/包含;指向关联活动的导航属性。</span><span class="sxs-lookup"><span data-stu-id="ad03d-177">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad03d-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad03d-178">JSON representation</span></span>

<span data-ttu-id="ad03d-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad03d-179">Here is a JSON representation of the resource.</span></span>

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
