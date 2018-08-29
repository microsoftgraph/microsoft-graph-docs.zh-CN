# <a name="activity-resource-type"></a><span data-ttu-id="788bf-101">活动资源类型</span><span class="sxs-lookup"><span data-stu-id="788bf-101">For details, see activity resource type.</span></span>

<span data-ttu-id="788bf-102">表示应用内的单一活动——例如，电视节目、文档或视频游戏中的当前活动。</span><span class="sxs-lookup"><span data-stu-id="788bf-102">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="788bf-103">当用户预订那个活动时，该预订捕获作为 [历史记录项](projectrome_historyitem.md)，显示该活动的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="788bf-103">When a user engages with that activity, the engagement is captured as a [history item](projectrome_historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="788bf-104">经过一段时间后当用户重新预订该活动时，单一用户活动会记录着多个历史记录项。</span><span class="sxs-lookup"><span data-stu-id="788bf-104">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="788bf-105">你可以在多个设备使用 Microsoft Graph 中的活动使用户能够回到他们当时在应用中正在做的事情。</span><span class="sxs-lookup"><span data-stu-id="788bf-105">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="788bf-106">你的应用所创建的活动会显示在所有用户的设备上，并以深层链接让用户接触到你应用内的特定内容。</span><span class="sxs-lookup"><span data-stu-id="788bf-106">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="788bf-107">你可以将你应用内的特定内容表示为 Windows 中展示的目的地，并且通过 Cortana 通知数在 iOS 和 Android 设备上都可以访问。</span><span class="sxs-lookup"><span data-stu-id="788bf-107">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="788bf-108">因为每个应用都不一样，所以这取决于你了解将你应用程序内的操作映射到将出现在 Cortana 和日程表中的用户活动的最佳方式。</span><span class="sxs-lookup"><span data-stu-id="788bf-108">Because every app is different, it's up to each app developer to understand the best way to map actions within your application to user activities.</span></span> <span data-ttu-id="788bf-109">例如，游戏可能为每个关卡创建活动、文档创作应用程序可能会为每个唯一的文档创建活动，业务线应用程序可能会为每个工作流创建活动。</span><span class="sxs-lookup"><span data-stu-id="788bf-109">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="788bf-110">用户活动将展示在用户体验的 Cortana 和 Windows 日程表中，重点以帮助用户回到他们过去从事过的内容来提高用户生产力和效率。</span><span class="sxs-lookup"><span data-stu-id="788bf-110">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="788bf-111">方法</span><span class="sxs-lookup"><span data-stu-id="788bf-111">Methods</span></span>

|<span data-ttu-id="788bf-112">方法</span><span class="sxs-lookup"><span data-stu-id="788bf-112">Method</span></span> | <span data-ttu-id="788bf-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="788bf-113">Return Type</span></span> | <span data-ttu-id="788bf-114">说明</span><span class="sxs-lookup"><span data-stu-id="788bf-114">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="788bf-115">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="788bf-115">Create or replace an activity</span></span>](../api/projectrome_put_activity.md) | [<span data-ttu-id="788bf-116">活动</span><span class="sxs-lookup"><span data-stu-id="788bf-116">activity</span></span>](projectrome_activity.md) |<span data-ttu-id="788bf-117">创建或替换现有的活动 (upsert)。</span><span class="sxs-lookup"><span data-stu-id="788bf-117">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="788bf-118">appActivityId 需要是 URL-safe 的（除 RFC 2396 未保留的字符外所有字符都必须转换为十六进制表示），但原始的 appActivityId 不必是 URL-safe 的。</span><span class="sxs-lookup"><span data-stu-id="788bf-118">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="788bf-119">删除活动</span><span class="sxs-lookup"><span data-stu-id="788bf-119">Delete an activity</span></span>](../api/projectrome_delete_activity.md) | <span data-ttu-id="788bf-120">没有内容</span><span class="sxs-lookup"><span data-stu-id="788bf-120">204 No Content</span></span> | <span data-ttu-id="788bf-121">从你的应用中删除那个用户的指定活动。</span><span class="sxs-lookup"><span data-stu-id="788bf-121">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="788bf-122">获取活动</span><span class="sxs-lookup"><span data-stu-id="788bf-122">Get recent activities</span></span>](../api/projectrome_get_activities.md) | <span data-ttu-id="788bf-123"> [活动](projectrome_activity.md)集合</span><span class="sxs-lookup"><span data-stu-id="788bf-123">Collection of [activities](projectrome_activity.md)</span></span> | <span data-ttu-id="788bf-124">获取给定用户的应用的活动。</span><span class="sxs-lookup"><span data-stu-id="788bf-124">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="788bf-125">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="788bf-125">Get recent activities</span></span>](../api/projectrome_get_recent_activities.md) | <span data-ttu-id="788bf-126"> [活动](projectrome_activity.md)集合</span><span class="sxs-lookup"><span data-stu-id="788bf-126">Collection of [activities](projectrome_activity.md)</span></span> | <span data-ttu-id="788bf-127">按照最近创建或更新的 [historyItems](projectrome_historyitem.md)排序并以此为根据来获取你给定用户的应用的最新活动。</span><span class="sxs-lookup"><span data-stu-id="788bf-127">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome_historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="788bf-128">属性</span><span class="sxs-lookup"><span data-stu-id="788bf-128">Properties</span></span>

|<span data-ttu-id="788bf-129">名称</span><span class="sxs-lookup"><span data-stu-id="788bf-129">Name</span></span> | <span data-ttu-id="788bf-130">类型</span><span class="sxs-lookup"><span data-stu-id="788bf-130">Type</span></span> | <span data-ttu-id="788bf-131">说明</span><span class="sxs-lookup"><span data-stu-id="788bf-131">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="788bf-132">userTimezone</span><span class="sxs-lookup"><span data-stu-id="788bf-132">userTimezone</span></span> | <span data-ttu-id="788bf-133">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-133">String</span></span> | <span data-ttu-id="788bf-134">可选。</span><span class="sxs-lookup"><span data-stu-id="788bf-134">Optional.</span></span> <span data-ttu-id="788bf-135">用于生成活动的用户设备所在的时区当时位于在活动创建时；值作为 Olson ID 提供，以便支持跨平台表示形式。</span><span class="sxs-lookup"><span data-stu-id="788bf-135">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="788bf-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="788bf-136">createdDateTime</span></span> | <span data-ttu-id="788bf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="788bf-137">DateTimeOffset</span></span> | <span data-ttu-id="788bf-138">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="788bf-138">Set by the server.</span></span> <span data-ttu-id="788bf-139">服务器创建对象时的 UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="788bf-139">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="788bf-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="788bf-140">lastModifiedDateTime</span></span> | <span data-ttu-id="788bf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="788bf-141">DateTimeOffset</span></span> | <span data-ttu-id="788bf-142">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="788bf-142">Set by the server.</span></span> <span data-ttu-id="788bf-143">服务器修改对象时的 UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="788bf-143">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="788bf-144">ID</span><span class="sxs-lookup"><span data-stu-id="788bf-144">id</span></span> | <span data-ttu-id="788bf-145">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-145">String</span></span> | <span data-ttu-id="788bf-146">用于 URL 寻址的服务器生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="788bf-146">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="788bf-147">appActivityId</span><span class="sxs-lookup"><span data-stu-id="788bf-147">appActivityId</span></span> | <span data-ttu-id="788bf-148">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-148">String</span></span> | <span data-ttu-id="788bf-149">必需。</span><span class="sxs-lookup"><span data-stu-id="788bf-149">Required.</span></span> <span data-ttu-id="788bf-150">应用环境中唯一的活动 ID——由调用程序提供并且此后是不可变的。</span><span class="sxs-lookup"><span data-stu-id="788bf-150">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="788bf-151">activitySourceHost</span><span class="sxs-lookup"><span data-stu-id="788bf-151">activitySourceHost</span></span> | <span data-ttu-id="788bf-152">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-152">String</span></span> | <span data-ttu-id="788bf-153">必需项。</span><span class="sxs-lookup"><span data-stu-id="788bf-153">Required.</span></span> <span data-ttu-id="788bf-154">表示应用的跨平台标识映射的域的 URL。</span><span class="sxs-lookup"><span data-stu-id="788bf-154">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="788bf-155">映射或者以域托管的 JSON 文件存储，或者通过 Windows 开发人员中心配置。</span><span class="sxs-lookup"><span data-stu-id="788bf-155">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="788bf-156">JSON 文件命名为跨平台应用标识符并托管在你的 HTTPS 域的根，或者在顶级域，或者包括子域。</span><span class="sxs-lookup"><span data-stu-id="788bf-156">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="788bf-157">例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。</span><span class="sxs-lookup"><span data-stu-id="788bf-157">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="788bf-158">你必须每个跨平台应用标识都具有唯一文件和域 （或子域）。</span><span class="sxs-lookup"><span data-stu-id="788bf-158">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="788bf-159">例如，Word vs. PowerPoint 就需要单独的文件和域。</span><span class="sxs-lookup"><span data-stu-id="788bf-159">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="788bf-160">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="788bf-160">AppDisplayName</span></span> | <span data-ttu-id="788bf-161">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-161">String</span></span> | <span data-ttu-id="788bf-162">可选。</span><span class="sxs-lookup"><span data-stu-id="788bf-162">Optional.</span></span> <span data-ttu-id="788bf-163">用于在用户的本地设备上未安装应用的情况下生成使用活动的应用的简短文本说明。</span><span class="sxs-lookup"><span data-stu-id="788bf-163">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="788bf-164">activationUrl</span><span class="sxs-lookup"><span data-stu-id="788bf-164">activationUrl</span></span> | <span data-ttu-id="788bf-165">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-165">String</span></span> | <span data-ttu-id="788bf-166">必需项。</span><span class="sxs-lookup"><span data-stu-id="788bf-166">Required.</span></span> <span data-ttu-id="788bf-167">由 appId 表示的用于启动最佳本机体验的活动 URL。</span><span class="sxs-lookup"><span data-stu-id="788bf-167">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="788bf-168">如果没有本机的应用存在，则可能会启动一个基于 Web 的应用。</span><span class="sxs-lookup"><span data-stu-id="788bf-168">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="788bf-169">fallbackUrl</span><span class="sxs-lookup"><span data-stu-id="788bf-169">fallbackUrl</span></span> | <span data-ttu-id="788bf-170">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-170">String</span></span> | <span data-ttu-id="788bf-171">可选。</span><span class="sxs-lookup"><span data-stu-id="788bf-171">Optional.</span></span> <span data-ttu-id="788bf-172">用于启动基于 Web 的应用中的活动的 URL（如果可用）。</span><span class="sxs-lookup"><span data-stu-id="788bf-172">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="788bf-173">contentUrl</span><span class="sxs-lookup"><span data-stu-id="788bf-173">contentUrl</span></span> | <span data-ttu-id="788bf-174">字符串</span><span class="sxs-lookup"><span data-stu-id="788bf-174">String</span></span> | <span data-ttu-id="788bf-175">可选。</span><span class="sxs-lookup"><span data-stu-id="788bf-175">Optional.</span></span> <span data-ttu-id="788bf-176">用于内容可以呈现在本机或基于 Web 的应用体验之外的事件（例如，RSS 源中的项目的指针）。</span><span class="sxs-lookup"><span data-stu-id="788bf-176">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="788bf-177">visualElements</span><span class="sxs-lookup"><span data-stu-id="788bf-177">visualElements</span></span>| <span data-ttu-id="788bf-178">[visualInfo](../resources/projectrome_visualinfo.md)</span><span class="sxs-lookup"><span data-stu-id="788bf-178">Added [visualInfo](../resources/projectrome_visualinfo.md)</span></span> | <span data-ttu-id="788bf-179">必需。</span><span class="sxs-lookup"><span data-stu-id="788bf-179">Required.</span></span> <span data-ttu-id="788bf-180">包含呈现 UX 活动信息的对象。</span><span class="sxs-lookup"><span data-stu-id="788bf-180">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="788bf-181">contentInfo</span><span class="sxs-lookup"><span data-stu-id="788bf-181">contentInfo</span></span> | <span data-ttu-id="788bf-182">无类型的 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="788bf-182">Untyped JSON object</span></span> | <span data-ttu-id="788bf-183">可选。</span><span class="sxs-lookup"><span data-stu-id="788bf-183">Optional.</span></span> <span data-ttu-id="788bf-184">一段自定义数据—— JSON-LD 根据 [schema.org](http://schema.org) 语法的内容的可扩展说明。</span><span class="sxs-lookup"><span data-stu-id="788bf-184">A custom piece of data - JSON-LD extensible description of content according to [schema.org](http://schema.org) syntax.</span></span>|
|<span data-ttu-id="788bf-185">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="788bf-185">expirationDateTime</span></span> | <span data-ttu-id="788bf-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="788bf-186">DateTimeOffset</span></span> | <span data-ttu-id="788bf-187">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="788bf-187">Set by the server.</span></span> <span data-ttu-id="788bf-188">对象在服务器上过期时的 UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="788bf-188">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="788bf-189">状态</span><span class="sxs-lookup"><span data-stu-id="788bf-189">status</span></span> | <span data-ttu-id="788bf-190">状态</span><span class="sxs-lookup"><span data-stu-id="788bf-190">status</span></span> | <span data-ttu-id="788bf-191">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="788bf-191">Set by the server.</span></span> <span data-ttu-id="788bf-192">一个用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="788bf-192">A status code used to identify valid objects.</span></span> <span data-ttu-id="788bf-193">值：活动、已更新、已删除、已忽略。</span><span class="sxs-lookup"><span data-stu-id="788bf-193">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="788bf-194">关系</span><span class="sxs-lookup"><span data-stu-id="788bf-194">Relationships</span></span>

|<span data-ttu-id="788bf-195">关系</span><span class="sxs-lookup"><span data-stu-id="788bf-195">Relationship</span></span> | <span data-ttu-id="788bf-196">类型</span><span class="sxs-lookup"><span data-stu-id="788bf-196">Type</span></span> | <span data-ttu-id="788bf-197">说明</span><span class="sxs-lookup"><span data-stu-id="788bf-197">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="788bf-198">historyItems</span><span class="sxs-lookup"><span data-stu-id="788bf-198">historyItems</span></span>| <span data-ttu-id="788bf-199">[activityHistoryItem](../resources/projectrome_historyitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="788bf-199">[activityHistoryItem](../resources/projectrome_historyitem.md) collection</span></span> | <span data-ttu-id="788bf-200">可选。</span><span class="sxs-lookup"><span data-stu-id="788bf-200">Optional.</span></span> <span data-ttu-id="788bf-201">NavigationProperty/Containment；活动的 historyItems 的导航属性。</span><span class="sxs-lookup"><span data-stu-id="788bf-201">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="788bf-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="788bf-202">JSON representation</span></span>

<span data-ttu-id="788bf-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="788bf-203">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userActivity",
  "@odata.annotations": [
    {
      "capabilities": {
        "countable": false,
        "selectable": false,
        "skippable": false
      }
    }
  ]
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@odata.type": "microsoft.graph.Json" },
    "visualElements": { "@odata.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.activityHistoryItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
