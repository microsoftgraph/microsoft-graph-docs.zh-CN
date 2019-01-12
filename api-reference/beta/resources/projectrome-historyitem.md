---
title: historyItem 资源类型
description: 表示为活动应用程序中的历史记录项。 用户活动表示单个目标应用程序-例如，TV 显示、 文档或视频游戏中当前市场活动中。 当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 168587aa54446aeee78107deaa9087c6bffb8586
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976952"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="253b8-106">historyItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="253b8-106">historyItem resource type</span></span>

> <span data-ttu-id="253b8-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="253b8-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="253b8-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="253b8-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="253b8-109">表示为[活动](projectrome-activity.md)应用程序中的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="253b8-109">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="253b8-110">用户活动表示单个目标应用程序-例如，TV 显示、 文档或视频游戏中当前市场活动中。</span><span class="sxs-lookup"><span data-stu-id="253b8-110">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="253b8-111">当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。</span><span class="sxs-lookup"><span data-stu-id="253b8-111">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="253b8-112">根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。</span><span class="sxs-lookup"><span data-stu-id="253b8-112">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="253b8-113">当应用程序创建会话时，应是**historyItem**对象添加到**活动**对象以反映用户工作效率期。</span><span class="sxs-lookup"><span data-stu-id="253b8-113">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="253b8-114">每次用户重新启动与活动，新**historyItem**添加到活动以应计用户工作效率。</span><span class="sxs-lookup"><span data-stu-id="253b8-114">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="253b8-115">方法</span><span class="sxs-lookup"><span data-stu-id="253b8-115">Methods</span></span>

|<span data-ttu-id="253b8-116">方法</span><span class="sxs-lookup"><span data-stu-id="253b8-116">Method</span></span> | <span data-ttu-id="253b8-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="253b8-117">Return Type</span></span> | <span data-ttu-id="253b8-118">说明</span><span class="sxs-lookup"><span data-stu-id="253b8-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="253b8-119">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="253b8-119">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="253b8-120">historyItem</span><span class="sxs-lookup"><span data-stu-id="253b8-120">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="253b8-121">创建或替换现有**historyItem**为该活动 (upsert)。</span><span class="sxs-lookup"><span data-stu-id="253b8-121">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="253b8-122">ID 需要一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="253b8-122">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="253b8-123">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="253b8-123">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="253b8-124">无内容</span><span class="sxs-lookup"><span data-stu-id="253b8-124">No Content</span></span> | <span data-ttu-id="253b8-125">删除指定的**historyItem**为该活动。</span><span class="sxs-lookup"><span data-stu-id="253b8-125">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="253b8-126">属性</span><span class="sxs-lookup"><span data-stu-id="253b8-126">Properties</span></span>

|<span data-ttu-id="253b8-127">名称</span><span class="sxs-lookup"><span data-stu-id="253b8-127">Name</span></span> | <span data-ttu-id="253b8-128">类型</span><span class="sxs-lookup"><span data-stu-id="253b8-128">Type</span></span> | <span data-ttu-id="253b8-129">说明</span><span class="sxs-lookup"><span data-stu-id="253b8-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="253b8-130">状态</span><span class="sxs-lookup"><span data-stu-id="253b8-130">status</span></span> | <span data-ttu-id="253b8-131">EnumType</span><span class="sxs-lookup"><span data-stu-id="253b8-131">EnumType</span></span> | <span data-ttu-id="253b8-132">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="253b8-132">Set by the server.</span></span> <span data-ttu-id="253b8-133">一个用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="253b8-133">A status code used to identify valid objects.</span></span> <span data-ttu-id="253b8-134">值： 活动更新、 删除、 忽略。</span><span class="sxs-lookup"><span data-stu-id="253b8-134">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="253b8-135">userTimezone</span><span class="sxs-lookup"><span data-stu-id="253b8-135">userTimezone</span></span> | <span data-ttu-id="253b8-136">字符串</span><span class="sxs-lookup"><span data-stu-id="253b8-136">String</span></span> | <span data-ttu-id="253b8-137">可选。</span><span class="sxs-lookup"><span data-stu-id="253b8-137">Optional.</span></span> <span data-ttu-id="253b8-138">在其中用户的设备用来生成活动位于在活动创建时间的时区。</span><span class="sxs-lookup"><span data-stu-id="253b8-138">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="253b8-139">为了支持跨平台表示形式作为 Olson Id 提供的值。</span><span class="sxs-lookup"><span data-stu-id="253b8-139">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="253b8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="253b8-140">createdDateTime</span></span> | <span data-ttu-id="253b8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="253b8-141">DateTimeOffset</span></span> | <span data-ttu-id="253b8-142">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="253b8-142">Set by the server.</span></span> <span data-ttu-id="253b8-143">采用 UTC 的服务器上创建对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="253b8-143">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="253b8-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="253b8-144">lastModifiedDateTime</span></span> | <span data-ttu-id="253b8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="253b8-145">DateTimeOffset</span></span> | <span data-ttu-id="253b8-146">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="253b8-146">Set by the server.</span></span> <span data-ttu-id="253b8-147">采用 UTC 的服务器上修改对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="253b8-147">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="253b8-148">id</span><span class="sxs-lookup"><span data-stu-id="253b8-148">id</span></span> | <span data-ttu-id="253b8-149">字符串</span><span class="sxs-lookup"><span data-stu-id="253b8-149">String</span></span> | <span data-ttu-id="253b8-150">必需。</span><span class="sxs-lookup"><span data-stu-id="253b8-150">Required.</span></span> <span data-ttu-id="253b8-151">**HistoryItem**对象的客户端集 GUID。</span><span class="sxs-lookup"><span data-stu-id="253b8-151">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="253b8-152">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="253b8-152">startedDateTime</span></span> | <span data-ttu-id="253b8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="253b8-153">DateTimeOffset</span></span> | <span data-ttu-id="253b8-154">必需。</span><span class="sxs-lookup"><span data-stu-id="253b8-154">Required.</span></span> <span data-ttu-id="253b8-155">启动**historyItem** （活动会话） 时，日期 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="253b8-155">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="253b8-156">所需的时间线历史记录。</span><span class="sxs-lookup"><span data-stu-id="253b8-156">Required for timeline history.</span></span>|
|<span data-ttu-id="253b8-157">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="253b8-157">lastActiveDateTime</span></span> | <span data-ttu-id="253b8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="253b8-158">DateTimeOffset</span></span> | <span data-ttu-id="253b8-159">可选。</span><span class="sxs-lookup"><span data-stu-id="253b8-159">Optional.</span></span> <span data-ttu-id="253b8-160">UTC DateTime **historyItem** （活动会话） 的最后一个了解作为活动或完成-如果为空， **historyItem**状态时应日常。</span><span class="sxs-lookup"><span data-stu-id="253b8-160">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="253b8-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="253b8-161">expirationDateTime</span></span> | <span data-ttu-id="253b8-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="253b8-162">DateTimeOffset</span></span> | <span data-ttu-id="253b8-163">可选。</span><span class="sxs-lookup"><span data-stu-id="253b8-163">Optional.</span></span> <span data-ttu-id="253b8-164">**HistoryItem**会经过硬删除时，日期 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="253b8-164">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="253b8-165">可以由客户端设置。</span><span class="sxs-lookup"><span data-stu-id="253b8-165">Can be set by the client.</span></span>|
|<span data-ttu-id="253b8-166">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="253b8-166">activeDurationSeconds</span></span> | <span data-ttu-id="253b8-167">int</span><span class="sxs-lookup"><span data-stu-id="253b8-167">int</span></span> | <span data-ttu-id="253b8-168">可选。</span><span class="sxs-lookup"><span data-stu-id="253b8-168">Optional.</span></span> <span data-ttu-id="253b8-169">活动用户工作效率的持续时间。</span><span class="sxs-lookup"><span data-stu-id="253b8-169">The duration of active user engagement.</span></span> <span data-ttu-id="253b8-170">如果未提供，则从**startedDateTime**和**lastActiveDateTime**计算此。</span><span class="sxs-lookup"><span data-stu-id="253b8-170">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="253b8-171">Relationships</span><span class="sxs-lookup"><span data-stu-id="253b8-171">Relationships</span></span>

|<span data-ttu-id="253b8-172">关系</span><span class="sxs-lookup"><span data-stu-id="253b8-172">Relationship</span></span> | <span data-ttu-id="253b8-173">类型</span><span class="sxs-lookup"><span data-stu-id="253b8-173">Type</span></span> | <span data-ttu-id="253b8-174">说明</span><span class="sxs-lookup"><span data-stu-id="253b8-174">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="253b8-175">activity</span><span class="sxs-lookup"><span data-stu-id="253b8-175">activity</span></span>| [<span data-ttu-id="253b8-176">活动</span><span class="sxs-lookup"><span data-stu-id="253b8-176">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="253b8-177">可选。</span><span class="sxs-lookup"><span data-stu-id="253b8-177">Optional.</span></span> <span data-ttu-id="253b8-178">NavigationProperty/包容;导航到关联的活动的属性。</span><span class="sxs-lookup"><span data-stu-id="253b8-178">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="253b8-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="253b8-179">JSON representation</span></span>

<span data-ttu-id="253b8-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="253b8-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
