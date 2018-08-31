# <a name="historyitem-resource-type"></a><span data-ttu-id="e4f94-101">historyItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4f94-101">historyItem resource type</span></span>

<span data-ttu-id="e4f94-102">代表应用程序中[活动](projectrome_activity.md)的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="e4f94-102">Represents a history item for an [activity](projectrome_activity.md) in an app.</span></span> <span data-ttu-id="e4f94-103">用户活动代表应用程序内的单个目标——例如，电视节目、文档或视频游戏中的当前活动。</span><span class="sxs-lookup"><span data-stu-id="e4f94-103">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="e4f94-104">当用户参与那个活动时，将参与作为 历史记录项捕获，显示该活动的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="e4f94-104">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="e4f94-105">经过一段时间后当用户重新参与该活动时，单一用户活动会记录着多个历史记录项。</span><span class="sxs-lookup"><span data-stu-id="e4f94-105">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="e4f94-106">当应用程序创建会话时，应将 **historyItem** 对象添加到**活动**对象以反映用户互动的时间段。</span><span class="sxs-lookup"><span data-stu-id="e4f94-106">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="e4f94-107">每次用户继续参与活动时，新的 **historyItem** 会添加到活动中，以累计用户的互动。</span><span class="sxs-lookup"><span data-stu-id="e4f94-107">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="e4f94-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4f94-108">Methods</span></span>

|<span data-ttu-id="e4f94-109">方法</span><span class="sxs-lookup"><span data-stu-id="e4f94-109">Method</span></span> | <span data-ttu-id="e4f94-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4f94-110">Return Type</span></span> | <span data-ttu-id="e4f94-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4f94-111">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="e4f94-112">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="e4f94-112">Create or replace historyItem</span></span>](../api/projectrome_put_historyitem.md) | <span data-ttu-id="e4f94-113">[historyItem](projectrome_historyitem.md)</span><span class="sxs-lookup"><span data-stu-id="e4f94-113">Added [historyItem](projectrome_historyitem.md)</span></span> | <span data-ttu-id="e4f94-114">为该活动 (upsert) 创建或替换现有的 **historyItem**。</span><span class="sxs-lookup"><span data-stu-id="e4f94-114">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="e4f94-115">ID 必须是 GUID。</span><span class="sxs-lookup"><span data-stu-id="e4f94-115">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="e4f94-116">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="e4f94-116">Delete a historyItem</span></span>](../api/projectrome_delete_historyitem.md) | <span data-ttu-id="e4f94-117">没有内容</span><span class="sxs-lookup"><span data-stu-id="e4f94-117">204 No Content</span></span> | <span data-ttu-id="e4f94-118">为该活动删除指定的 **historyItem**。</span><span class="sxs-lookup"><span data-stu-id="e4f94-118">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4f94-119">属性</span><span class="sxs-lookup"><span data-stu-id="e4f94-119">Properties</span></span>

|<span data-ttu-id="e4f94-120">名称</span><span class="sxs-lookup"><span data-stu-id="e4f94-120">Name</span></span> | <span data-ttu-id="e4f94-121">类型</span><span class="sxs-lookup"><span data-stu-id="e4f94-121">Type</span></span> | <span data-ttu-id="e4f94-122">说明</span><span class="sxs-lookup"><span data-stu-id="e4f94-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e4f94-123">状态</span><span class="sxs-lookup"><span data-stu-id="e4f94-123">status</span></span> | <span data-ttu-id="e4f94-124">状态</span><span class="sxs-lookup"><span data-stu-id="e4f94-124">status</span></span> | <span data-ttu-id="e4f94-125">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="e4f94-125">Set by the server.</span></span> <span data-ttu-id="e4f94-126">一个用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="e4f94-126">A status code used to identify valid objects.</span></span> <span data-ttu-id="e4f94-127">值：活动、已更新、已删除、已忽略。</span><span class="sxs-lookup"><span data-stu-id="e4f94-127">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="e4f94-128">userTimezone</span><span class="sxs-lookup"><span data-stu-id="e4f94-128">userTimezone</span></span> | <span data-ttu-id="e4f94-129">字符串</span><span class="sxs-lookup"><span data-stu-id="e4f94-129">String</span></span> | <span data-ttu-id="e4f94-130">可选。</span><span class="sxs-lookup"><span data-stu-id="e4f94-130">Optional.</span></span> <span data-ttu-id="e4f94-131">用于生成活动的用户设备所在的时区当时位于活动创建时。</span><span class="sxs-lookup"><span data-stu-id="e4f94-131">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="e4f94-132">值作为 Olson ID 提供，以便支持跨平台表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4f94-132">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="e4f94-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f94-133">createdDateTime</span></span> | <span data-ttu-id="e4f94-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f94-134">DateTimeOffset</span></span> | <span data-ttu-id="e4f94-135">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="e4f94-135">Set by the server.</span></span> <span data-ttu-id="e4f94-136">服务器创建对象时的 UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="e4f94-136">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="e4f94-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f94-137">lastModifiedDateTime</span></span> | <span data-ttu-id="e4f94-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f94-138">DateTimeOffset</span></span> | <span data-ttu-id="e4f94-139">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="e4f94-139">Set by the server.</span></span> <span data-ttu-id="e4f94-140">在服务器上修改对象时的 UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="e4f94-140">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="e4f94-141">ID</span><span class="sxs-lookup"><span data-stu-id="e4f94-141">id</span></span> | <span data-ttu-id="e4f94-142">字符串</span><span class="sxs-lookup"><span data-stu-id="e4f94-142">String</span></span> | <span data-ttu-id="e4f94-143">必需。</span><span class="sxs-lookup"><span data-stu-id="e4f94-143">Required.</span></span> <span data-ttu-id="e4f94-144"> **historyItem** 对象的客户端集 GUID。</span><span class="sxs-lookup"><span data-stu-id="e4f94-144">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="e4f94-145">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f94-145">startedDateTime</span></span> | <span data-ttu-id="e4f94-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f94-146">DateTimeOffset</span></span> | <span data-ttu-id="e4f94-147">必需。</span><span class="sxs-lookup"><span data-stu-id="e4f94-147">Required.</span></span> <span data-ttu-id="e4f94-148">启动 **historyItem** （活动会话）时的 UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="e4f94-148">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="e4f94-149">所需的时间线历史记录。</span><span class="sxs-lookup"><span data-stu-id="e4f94-149">Required for timeline history.</span></span>|
|<span data-ttu-id="e4f94-150">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f94-150">lastActiveDateTime</span></span> | <span data-ttu-id="e4f94-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f94-151">DateTimeOffset</span></span> | <span data-ttu-id="e4f94-152">可选。</span><span class="sxs-lookup"><span data-stu-id="e4f94-152">Optional.</span></span> <span data-ttu-id="e4f94-153">**historyItem** （活动会话）最后被理解为活动或已完成时的 UTC DateTime，如果为空，**historyItem** 状态应为“正在进行”。</span><span class="sxs-lookup"><span data-stu-id="e4f94-153">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="e4f94-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f94-154">expirationDateTime</span></span> | <span data-ttu-id="e4f94-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f94-155">DateTimeOffset</span></span> | <span data-ttu-id="e4f94-156">可选。</span><span class="sxs-lookup"><span data-stu-id="e4f94-156">Optional.</span></span> <span data-ttu-id="e4f94-157"> **historyItem** 将进行硬删除时的 UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="e4f94-157">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="e4f94-158">可以由客户端设置。</span><span class="sxs-lookup"><span data-stu-id="e4f94-158">Can be set by the client.</span></span>|
|<span data-ttu-id="e4f94-159">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="e4f94-159">activeDurationSeconds</span></span> | <span data-ttu-id="e4f94-160">int</span><span class="sxs-lookup"><span data-stu-id="e4f94-160">int</span></span> | <span data-ttu-id="e4f94-161">可选。</span><span class="sxs-lookup"><span data-stu-id="e4f94-161">Optional.</span></span> <span data-ttu-id="e4f94-162">活动用户互动的持续时间。</span><span class="sxs-lookup"><span data-stu-id="e4f94-162">The duration of active user engagement.</span></span> <span data-ttu-id="e4f94-163">如果未提供，则从 **startedDateTime** 和 **lastActiveDateTime**计算得出。</span><span class="sxs-lookup"><span data-stu-id="e4f94-163">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4f94-164">关系</span><span class="sxs-lookup"><span data-stu-id="e4f94-164">Relationships</span></span>

|<span data-ttu-id="e4f94-165">关系</span><span class="sxs-lookup"><span data-stu-id="e4f94-165">Relationship</span></span> | <span data-ttu-id="e4f94-166">类型</span><span class="sxs-lookup"><span data-stu-id="e4f94-166">Type</span></span> | <span data-ttu-id="e4f94-167">说明</span><span class="sxs-lookup"><span data-stu-id="e4f94-167">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="e4f94-168">activity</span><span class="sxs-lookup"><span data-stu-id="e4f94-168">activity</span></span>| [<span data-ttu-id="e4f94-169">userActivity</span><span class="sxs-lookup"><span data-stu-id="e4f94-169">userActivity</span></span>](../resources/projectrome_activity.md) | <span data-ttu-id="e4f94-170">可选。</span><span class="sxs-lookup"><span data-stu-id="e4f94-170">Optional.</span></span> <span data-ttu-id="e4f94-171">NavigationProperty/Containment；关联活动的导航属性。</span><span class="sxs-lookup"><span data-stu-id="e4f94-171">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4f94-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4f94-172">JSON representation</span></span>

<span data-ttu-id="e4f94-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4f94-173">Here is a JSON representation of the resource.</span></span>

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
