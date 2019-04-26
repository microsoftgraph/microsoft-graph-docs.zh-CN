---
title: historyItem 资源类型
description: 表示应用中的活动的历史记录项。 用户活动表示应用程序中的单个目标, 例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时, 会将该预订作为历史项目进行捕获, 以指示该活动的开始时间和结束时间。 随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: c43a4f0515f8d61625e11abe8bbdbe2464c729f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344059"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="7bf82-106">historyItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7bf82-106">historyItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bf82-107">表示应用中的[活动](projectrome-activity.md)的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="7bf82-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="7bf82-108">用户活动表示应用程序中的单个目标, 例如电视节目、文档或视频游戏中的当前市场活动。</span><span class="sxs-lookup"><span data-stu-id="7bf82-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="7bf82-109">当用户参与该活动时, 会将该预订作为历史项目进行捕获, 以指示该活动的开始时间和结束时间。</span><span class="sxs-lookup"><span data-stu-id="7bf82-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="7bf82-110">随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。</span><span class="sxs-lookup"><span data-stu-id="7bf82-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="7bf82-111">当应用程序创建会话时, 应将一个**historyItem**对象添加到**活动**对象, 以反映用户参与的时段。</span><span class="sxs-lookup"><span data-stu-id="7bf82-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="7bf82-112">用户每次重新参与活动时, 都会向活动中添加一个新的**historyItem**以计入用户约定。</span><span class="sxs-lookup"><span data-stu-id="7bf82-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="7bf82-113">方法</span><span class="sxs-lookup"><span data-stu-id="7bf82-113">Methods</span></span>

|<span data-ttu-id="7bf82-114">方法</span><span class="sxs-lookup"><span data-stu-id="7bf82-114">Method</span></span> | <span data-ttu-id="7bf82-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="7bf82-115">Return Type</span></span> | <span data-ttu-id="7bf82-116">说明</span><span class="sxs-lookup"><span data-stu-id="7bf82-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="7bf82-117">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="7bf82-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="7bf82-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="7bf82-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="7bf82-119">创建或替换该活动的现有**historyItem** (upsert)。</span><span class="sxs-lookup"><span data-stu-id="7bf82-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="7bf82-120">ID 必须是 GUID。</span><span class="sxs-lookup"><span data-stu-id="7bf82-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="7bf82-121">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="7bf82-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="7bf82-122">无内容</span><span class="sxs-lookup"><span data-stu-id="7bf82-122">No Content</span></span> | <span data-ttu-id="7bf82-123">删除该活动的指定**historyItem** 。</span><span class="sxs-lookup"><span data-stu-id="7bf82-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="7bf82-124">属性</span><span class="sxs-lookup"><span data-stu-id="7bf82-124">Properties</span></span>

|<span data-ttu-id="7bf82-125">名称</span><span class="sxs-lookup"><span data-stu-id="7bf82-125">Name</span></span> | <span data-ttu-id="7bf82-126">类型</span><span class="sxs-lookup"><span data-stu-id="7bf82-126">Type</span></span> | <span data-ttu-id="7bf82-127">说明</span><span class="sxs-lookup"><span data-stu-id="7bf82-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7bf82-128">状态</span><span class="sxs-lookup"><span data-stu-id="7bf82-128">status</span></span> | <span data-ttu-id="7bf82-129">string</span><span class="sxs-lookup"><span data-stu-id="7bf82-129">string</span></span> | <span data-ttu-id="7bf82-130">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="7bf82-130">Set by the server.</span></span> <span data-ttu-id="7bf82-131">用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="7bf82-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="7bf82-132">值: 活动、已更新、已删除、已忽略。</span><span class="sxs-lookup"><span data-stu-id="7bf82-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="7bf82-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="7bf82-133">userTimezone</span></span> | <span data-ttu-id="7bf82-134">String</span><span class="sxs-lookup"><span data-stu-id="7bf82-134">String</span></span> | <span data-ttu-id="7bf82-135">可选。</span><span class="sxs-lookup"><span data-stu-id="7bf82-135">Optional.</span></span> <span data-ttu-id="7bf82-136">用于生成活动的用户设备所在的时区位于活动创建时间。</span><span class="sxs-lookup"><span data-stu-id="7bf82-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="7bf82-137">作为 Olson id 提供的值, 以便支持跨平台表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bf82-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="7bf82-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf82-138">createdDateTime</span></span> | <span data-ttu-id="7bf82-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf82-139">DateTimeOffset</span></span> | <span data-ttu-id="7bf82-140">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="7bf82-140">Set by the server.</span></span> <span data-ttu-id="7bf82-141">在服务器上创建对象时的 UTC 时间 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="7bf82-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="7bf82-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf82-142">lastModifiedDateTime</span></span> | <span data-ttu-id="7bf82-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf82-143">DateTimeOffset</span></span> | <span data-ttu-id="7bf82-144">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="7bf82-144">Set by the server.</span></span> <span data-ttu-id="7bf82-145">在服务器上修改对象时的 UTC 时间 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="7bf82-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="7bf82-146">id</span><span class="sxs-lookup"><span data-stu-id="7bf82-146">id</span></span> | <span data-ttu-id="7bf82-147">String</span><span class="sxs-lookup"><span data-stu-id="7bf82-147">String</span></span> | <span data-ttu-id="7bf82-148">必需。</span><span class="sxs-lookup"><span data-stu-id="7bf82-148">Required.</span></span> <span data-ttu-id="7bf82-149">客户端集的**historyItem**对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="7bf82-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="7bf82-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf82-150">startedDateTime</span></span> | <span data-ttu-id="7bf82-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf82-151">DateTimeOffset</span></span> | <span data-ttu-id="7bf82-152">必需。</span><span class="sxs-lookup"><span data-stu-id="7bf82-152">Required.</span></span> <span data-ttu-id="7bf82-153">**historyItem** (活动会话) 启动时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="7bf82-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="7bf82-154">对于时间线历史记录是必需的。</span><span class="sxs-lookup"><span data-stu-id="7bf82-154">Required for timeline history.</span></span>|
|<span data-ttu-id="7bf82-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf82-155">lastActiveDateTime</span></span> | <span data-ttu-id="7bf82-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf82-156">DateTimeOffset</span></span> | <span data-ttu-id="7bf82-157">可选。</span><span class="sxs-lookup"><span data-stu-id="7bf82-157">Optional.</span></span> <span data-ttu-id="7bf82-158">UTC DateTime 如果**historyItem** (活动会话) 上次被视为活动或已完成-如果为 null, 则**historyItem**状态应为 "正在进行"。</span><span class="sxs-lookup"><span data-stu-id="7bf82-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="7bf82-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf82-159">expirationDateTime</span></span> | <span data-ttu-id="7bf82-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf82-160">DateTimeOffset</span></span> | <span data-ttu-id="7bf82-161">可选。</span><span class="sxs-lookup"><span data-stu-id="7bf82-161">Optional.</span></span> <span data-ttu-id="7bf82-162">**historyItem**将被硬删除时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="7bf82-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="7bf82-163">可由客户端进行设置。</span><span class="sxs-lookup"><span data-stu-id="7bf82-163">Can be set by the client.</span></span>|
|<span data-ttu-id="7bf82-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="7bf82-164">activeDurationSeconds</span></span> | <span data-ttu-id="7bf82-165">int</span><span class="sxs-lookup"><span data-stu-id="7bf82-165">int</span></span> | <span data-ttu-id="7bf82-166">可选。</span><span class="sxs-lookup"><span data-stu-id="7bf82-166">Optional.</span></span> <span data-ttu-id="7bf82-167">活动用户约定的持续时间。</span><span class="sxs-lookup"><span data-stu-id="7bf82-167">The duration of active user engagement.</span></span> <span data-ttu-id="7bf82-168">如果未提供, 则从**startedDateTime**和**lastActiveDateTime**计算。</span><span class="sxs-lookup"><span data-stu-id="7bf82-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bf82-169">关系</span><span class="sxs-lookup"><span data-stu-id="7bf82-169">Relationships</span></span>

|<span data-ttu-id="7bf82-170">关系</span><span class="sxs-lookup"><span data-stu-id="7bf82-170">Relationship</span></span> | <span data-ttu-id="7bf82-171">类型</span><span class="sxs-lookup"><span data-stu-id="7bf82-171">Type</span></span> | <span data-ttu-id="7bf82-172">说明</span><span class="sxs-lookup"><span data-stu-id="7bf82-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="7bf82-173">activity</span><span class="sxs-lookup"><span data-stu-id="7bf82-173">activity</span></span>| [<span data-ttu-id="7bf82-174">活动</span><span class="sxs-lookup"><span data-stu-id="7bf82-174">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="7bf82-175">可选。</span><span class="sxs-lookup"><span data-stu-id="7bf82-175">Optional.</span></span> <span data-ttu-id="7bf82-176">NavigationProperty/包含;指向关联活动的导航属性。</span><span class="sxs-lookup"><span data-stu-id="7bf82-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bf82-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7bf82-177">JSON representation</span></span>

<span data-ttu-id="7bf82-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bf82-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
<!--
{
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
