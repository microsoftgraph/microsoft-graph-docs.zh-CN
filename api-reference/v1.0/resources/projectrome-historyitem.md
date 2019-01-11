---
title: historyItem 资源类型
description: 表示为活动应用程序中的历史记录项。 用户活动表示单个目标应用程序-例如，TV 显示、 文档或视频游戏中当前市场活动中。 当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。
localization_priority: Normal
ms.openlocfilehash: 510913be6a3f70190c7cf657d9540d75f481c3a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882913"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="f5e36-106">historyItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5e36-106">historyItem resource type</span></span>

<span data-ttu-id="f5e36-107">表示为[活动](projectrome-activity.md)应用程序中的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="f5e36-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="f5e36-108">用户活动表示单个目标应用程序-例如，TV 显示、 文档或视频游戏中当前市场活动中。</span><span class="sxs-lookup"><span data-stu-id="f5e36-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="f5e36-109">当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。</span><span class="sxs-lookup"><span data-stu-id="f5e36-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="f5e36-110">根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。</span><span class="sxs-lookup"><span data-stu-id="f5e36-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="f5e36-111">当应用程序创建会话时，应是**historyItem**对象添加到**活动**对象以反映用户工作效率期。</span><span class="sxs-lookup"><span data-stu-id="f5e36-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="f5e36-112">每次用户重新启动与活动，新**historyItem**添加到活动以应计用户工作效率。</span><span class="sxs-lookup"><span data-stu-id="f5e36-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="f5e36-113">方法</span><span class="sxs-lookup"><span data-stu-id="f5e36-113">Methods</span></span>

|<span data-ttu-id="f5e36-114">方法</span><span class="sxs-lookup"><span data-stu-id="f5e36-114">Method</span></span> | <span data-ttu-id="f5e36-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5e36-115">Return Type</span></span> | <span data-ttu-id="f5e36-116">说明</span><span class="sxs-lookup"><span data-stu-id="f5e36-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="f5e36-117">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="f5e36-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="f5e36-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="f5e36-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="f5e36-119">创建或替换现有**historyItem**为该活动 (upsert)。</span><span class="sxs-lookup"><span data-stu-id="f5e36-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="f5e36-120">ID 需要一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="f5e36-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="f5e36-121">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="f5e36-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="f5e36-122">无内容</span><span class="sxs-lookup"><span data-stu-id="f5e36-122">No Content</span></span> | <span data-ttu-id="f5e36-123">删除指定的**historyItem**为该活动。</span><span class="sxs-lookup"><span data-stu-id="f5e36-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5e36-124">属性</span><span class="sxs-lookup"><span data-stu-id="f5e36-124">Properties</span></span>

|<span data-ttu-id="f5e36-125">名称</span><span class="sxs-lookup"><span data-stu-id="f5e36-125">Name</span></span> | <span data-ttu-id="f5e36-126">类型</span><span class="sxs-lookup"><span data-stu-id="f5e36-126">Type</span></span> | <span data-ttu-id="f5e36-127">说明</span><span class="sxs-lookup"><span data-stu-id="f5e36-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f5e36-128">状态</span><span class="sxs-lookup"><span data-stu-id="f5e36-128">status</span></span> | <span data-ttu-id="f5e36-129">status</span><span class="sxs-lookup"><span data-stu-id="f5e36-129">status</span></span> | <span data-ttu-id="f5e36-130">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="f5e36-130">Set by the server.</span></span> <span data-ttu-id="f5e36-131">一个用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="f5e36-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="f5e36-132">值： 活动更新、 删除、 忽略。</span><span class="sxs-lookup"><span data-stu-id="f5e36-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="f5e36-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="f5e36-133">userTimezone</span></span> | <span data-ttu-id="f5e36-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f5e36-134">String</span></span> | <span data-ttu-id="f5e36-135">可选。</span><span class="sxs-lookup"><span data-stu-id="f5e36-135">Optional.</span></span> <span data-ttu-id="f5e36-136">在其中用户的设备用来生成活动位于在活动创建时间的时区。</span><span class="sxs-lookup"><span data-stu-id="f5e36-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="f5e36-137">为了支持跨平台表示形式作为 Olson Id 提供的值。</span><span class="sxs-lookup"><span data-stu-id="f5e36-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="f5e36-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5e36-138">createdDateTime</span></span> | <span data-ttu-id="f5e36-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5e36-139">DateTimeOffset</span></span> | <span data-ttu-id="f5e36-140">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="f5e36-140">Set by the server.</span></span> <span data-ttu-id="f5e36-141">采用 UTC 的服务器上创建对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f5e36-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="f5e36-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5e36-142">lastModifiedDateTime</span></span> | <span data-ttu-id="f5e36-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5e36-143">DateTimeOffset</span></span> | <span data-ttu-id="f5e36-144">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="f5e36-144">Set by the server.</span></span> <span data-ttu-id="f5e36-145">采用 UTC 的服务器上修改对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f5e36-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="f5e36-146">id</span><span class="sxs-lookup"><span data-stu-id="f5e36-146">id</span></span> | <span data-ttu-id="f5e36-147">字符串</span><span class="sxs-lookup"><span data-stu-id="f5e36-147">String</span></span> | <span data-ttu-id="f5e36-148">必需。</span><span class="sxs-lookup"><span data-stu-id="f5e36-148">Required.</span></span> <span data-ttu-id="f5e36-149">**HistoryItem**对象的客户端集 GUID。</span><span class="sxs-lookup"><span data-stu-id="f5e36-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="f5e36-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5e36-150">startedDateTime</span></span> | <span data-ttu-id="f5e36-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5e36-151">DateTimeOffset</span></span> | <span data-ttu-id="f5e36-152">必填。</span><span class="sxs-lookup"><span data-stu-id="f5e36-152">Required.</span></span> <span data-ttu-id="f5e36-153">启动**historyItem** （活动会话） 时，日期 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f5e36-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="f5e36-154">所需的时间线历史记录。</span><span class="sxs-lookup"><span data-stu-id="f5e36-154">Required for timeline history.</span></span>|
|<span data-ttu-id="f5e36-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="f5e36-155">lastActiveDateTime</span></span> | <span data-ttu-id="f5e36-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5e36-156">DateTimeOffset</span></span> | <span data-ttu-id="f5e36-157">可选。</span><span class="sxs-lookup"><span data-stu-id="f5e36-157">Optional.</span></span> <span data-ttu-id="f5e36-158">UTC DateTime **historyItem** （活动会话） 的最后一个了解作为活动或完成-如果为空， **historyItem**状态时应日常。</span><span class="sxs-lookup"><span data-stu-id="f5e36-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="f5e36-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f5e36-159">expirationDateTime</span></span> | <span data-ttu-id="f5e36-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5e36-160">DateTimeOffset</span></span> | <span data-ttu-id="f5e36-161">可选。</span><span class="sxs-lookup"><span data-stu-id="f5e36-161">Optional.</span></span> <span data-ttu-id="f5e36-162">**HistoryItem**会经过硬删除时，日期 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f5e36-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="f5e36-163">可以由客户端设置。</span><span class="sxs-lookup"><span data-stu-id="f5e36-163">Can be set by the client.</span></span>|
|<span data-ttu-id="f5e36-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="f5e36-164">activeDurationSeconds</span></span> | <span data-ttu-id="f5e36-165">int</span><span class="sxs-lookup"><span data-stu-id="f5e36-165">int</span></span> | <span data-ttu-id="f5e36-166">可选。</span><span class="sxs-lookup"><span data-stu-id="f5e36-166">Optional.</span></span> <span data-ttu-id="f5e36-167">活动用户工作效率的持续时间。</span><span class="sxs-lookup"><span data-stu-id="f5e36-167">The duration of active user engagement.</span></span> <span data-ttu-id="f5e36-168">如果未提供，则从**startedDateTime**和**lastActiveDateTime**计算此。</span><span class="sxs-lookup"><span data-stu-id="f5e36-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5e36-169">Relationships</span><span class="sxs-lookup"><span data-stu-id="f5e36-169">Relationships</span></span>

|<span data-ttu-id="f5e36-170">关系</span><span class="sxs-lookup"><span data-stu-id="f5e36-170">Relationship</span></span> | <span data-ttu-id="f5e36-171">类型</span><span class="sxs-lookup"><span data-stu-id="f5e36-171">Type</span></span> | <span data-ttu-id="f5e36-172">Description</span><span class="sxs-lookup"><span data-stu-id="f5e36-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="f5e36-173">activity</span><span class="sxs-lookup"><span data-stu-id="f5e36-173">activity</span></span>| [<span data-ttu-id="f5e36-174">userActivity</span><span class="sxs-lookup"><span data-stu-id="f5e36-174">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="f5e36-175">可选。</span><span class="sxs-lookup"><span data-stu-id="f5e36-175">Optional.</span></span> <span data-ttu-id="f5e36-176">NavigationProperty/包容;导航到关联的活动的属性。</span><span class="sxs-lookup"><span data-stu-id="f5e36-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5e36-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5e36-177">JSON representation</span></span>

<span data-ttu-id="f5e36-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5e36-178">Here is a JSON representation of the resource.</span></span>

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
