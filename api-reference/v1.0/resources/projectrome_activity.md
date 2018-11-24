# <a name="activity-resource-type"></a><span data-ttu-id="a0df4-101">活动资源类型</span><span class="sxs-lookup"><span data-stu-id="a0df4-101">activity resource type</span></span>

<span data-ttu-id="a0df4-102">表示应用程序-例如，TV 显示、 文档或视频游戏中的当前市场活动中的单个活动。</span><span class="sxs-lookup"><span data-stu-id="a0df4-102">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="a0df4-103">当用户启动与该活动时，此服务捕获作为[历史记录项](projectrome_historyitem.md)，指示该活动的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="a0df4-103">When a user engages with that activity, the engagement is captured as a [history item](projectrome_historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="a0df4-104">根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。</span><span class="sxs-lookup"><span data-stu-id="a0df4-104">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="a0df4-105">您可以使用在 Microsoft Graph 活动使用户能够获得到它们在做什么其应用程序中跨多个设备。</span><span class="sxs-lookup"><span data-stu-id="a0df4-105">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="a0df4-106">您的应用程序创建的活动显示所有用户在设备上，并向用户公开为深度链接到您的应用程序中的特定内容。</span><span class="sxs-lookup"><span data-stu-id="a0df4-106">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="a0df4-107">您可以为在 Windows 中，并在 iOS 和通过 Cortana 通知 Android 设备上访问展示的目标应用程序中表示特定内容。</span><span class="sxs-lookup"><span data-stu-id="a0df4-107">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="a0df4-108">由于每个应用程序不同，这取决于您了解映射中将出现在 Cortana 和日程表的用户活动应用程序的操作的最佳方式。</span><span class="sxs-lookup"><span data-stu-id="a0df4-108">Because every app is different, it's up to you to understand the best way to map actions within your application to user activities that will appear in Cortana and Timeline.</span></span> <span data-ttu-id="a0df4-109">例如，游戏可能创建活动的每个市场活动、 文档创作应用程序可能会创建每个唯一的文档，活动和业务线应用程序可能会创建每个工作流活动。</span><span class="sxs-lookup"><span data-stu-id="a0df4-109">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="a0df4-110">用户活动将供展示中 Cortana 和 Windows 时间线用户体验，重点以帮助其选择回到从事过去的内容来提高用户工作效率和效率。</span><span class="sxs-lookup"><span data-stu-id="a0df4-110">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="a0df4-111">方法</span><span class="sxs-lookup"><span data-stu-id="a0df4-111">Methods</span></span>

|<span data-ttu-id="a0df4-112">方法</span><span class="sxs-lookup"><span data-stu-id="a0df4-112">Method</span></span> | <span data-ttu-id="a0df4-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0df4-113">Return Type</span></span> | <span data-ttu-id="a0df4-114">说明</span><span class="sxs-lookup"><span data-stu-id="a0df4-114">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="a0df4-115">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="a0df4-115">Create or replace activity</span></span>](../api/projectrome_put_activity.md) | [<span data-ttu-id="a0df4-116">活动</span><span class="sxs-lookup"><span data-stu-id="a0df4-116">activity</span></span>](projectrome_activity.md) |<span data-ttu-id="a0df4-117">创建或替换现有的活动 (upsert)。</span><span class="sxs-lookup"><span data-stu-id="a0df4-117">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="a0df4-118">AppActivityId 需要 URL 安全 （除 RFC 2396 必须将未保留的字符转换为十六进制表示形式为所有字符），但原始 appActivityId 不必是安全的 URL。</span><span class="sxs-lookup"><span data-stu-id="a0df4-118">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="a0df4-119">删除活动</span><span class="sxs-lookup"><span data-stu-id="a0df4-119">Delete an activity</span></span>](../api/projectrome_delete_activity.md) | <span data-ttu-id="a0df4-120">无内容</span><span class="sxs-lookup"><span data-stu-id="a0df4-120">No Content</span></span> | <span data-ttu-id="a0df4-121">从您的应用程序中删除指定为该用户的活动。</span><span class="sxs-lookup"><span data-stu-id="a0df4-121">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="a0df4-122">获取活动</span><span class="sxs-lookup"><span data-stu-id="a0df4-122">Get activities</span></span>](../api/projectrome_get_activities.md) | <span data-ttu-id="a0df4-123">[活动](projectrome_activity.md)的集合</span><span class="sxs-lookup"><span data-stu-id="a0df4-123">Collection of [activities](projectrome_activity.md)</span></span> | <span data-ttu-id="a0df4-124">获取指定用户的应用程序的活动。</span><span class="sxs-lookup"><span data-stu-id="a0df4-124">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="a0df4-125">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="a0df4-125">Get recent activities</span></span>](../api/projectrome_get_recent_activities.md) | <span data-ttu-id="a0df4-126">[活动](projectrome_activity.md)的集合</span><span class="sxs-lookup"><span data-stu-id="a0df4-126">Collection of [activities](projectrome_activity.md)</span></span> | <span data-ttu-id="a0df4-127">为给定的用户、 排序和基于[historyItems](projectrome_historyitem.md)最近创建或更新您的应用程序获取最新的活动。</span><span class="sxs-lookup"><span data-stu-id="a0df4-127">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome_historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="a0df4-128">属性</span><span class="sxs-lookup"><span data-stu-id="a0df4-128">Properties</span></span>

|<span data-ttu-id="a0df4-129">名称</span><span class="sxs-lookup"><span data-stu-id="a0df4-129">Name</span></span> | <span data-ttu-id="a0df4-130">类型</span><span class="sxs-lookup"><span data-stu-id="a0df4-130">Type</span></span> | <span data-ttu-id="a0df4-131">说明</span><span class="sxs-lookup"><span data-stu-id="a0df4-131">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a0df4-132">userTimezone</span><span class="sxs-lookup"><span data-stu-id="a0df4-132">userTimezone</span></span> | <span data-ttu-id="a0df4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-133">String</span></span> | <span data-ttu-id="a0df4-134">可选。</span><span class="sxs-lookup"><span data-stu-id="a0df4-134">Optional.</span></span> <span data-ttu-id="a0df4-135">在其中用于生成活动的用户的设备已位于在活动创建时; timezone为了支持跨平台表示形式作为 Olson Id 提供的值。</span><span class="sxs-lookup"><span data-stu-id="a0df4-135">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="a0df4-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0df4-136">createdDateTime</span></span> | <span data-ttu-id="a0df4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0df4-137">DateTimeOffset</span></span> | <span data-ttu-id="a0df4-138">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="a0df4-138">Set by the server.</span></span> <span data-ttu-id="a0df4-139">采用 UTC 的服务器上创建对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0df4-139">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="a0df4-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0df4-140">lastModifiedDateTime</span></span> | <span data-ttu-id="a0df4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0df4-141">DateTimeOffset</span></span> | <span data-ttu-id="a0df4-142">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="a0df4-142">Set by the server.</span></span> <span data-ttu-id="a0df4-143">采用 UTC 的服务器上修改对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0df4-143">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="a0df4-144">id</span><span class="sxs-lookup"><span data-stu-id="a0df4-144">id</span></span> | <span data-ttu-id="a0df4-145">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-145">String</span></span> | <span data-ttu-id="a0df4-146">使用的 URL 地址的服务器生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="a0df4-146">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="a0df4-147">appActivityId</span><span class="sxs-lookup"><span data-stu-id="a0df4-147">appActivityId</span></span> | <span data-ttu-id="a0df4-148">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-148">String</span></span> | <span data-ttu-id="a0df4-149">必需项。</span><span class="sxs-lookup"><span data-stu-id="a0df4-149">Required.</span></span> <span data-ttu-id="a0df4-150">应用程序-此后提供呼叫者和不可变的上下文中唯一的活动 ID。</span><span class="sxs-lookup"><span data-stu-id="a0df4-150">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="a0df4-151">activitySourceHost</span><span class="sxs-lookup"><span data-stu-id="a0df4-151">activitySourceHost</span></span> | <span data-ttu-id="a0df4-152">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-152">String</span></span> | <span data-ttu-id="a0df4-153">必需项。</span><span class="sxs-lookup"><span data-stu-id="a0df4-153">Required.</span></span> <span data-ttu-id="a0df4-154">表示应用程序的跨平台标识映射的域的 URL。</span><span class="sxs-lookup"><span data-stu-id="a0df4-154">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="a0df4-155">映射是存储也为 JSON 文件域上托管或通过 Windows 开发人员中心可配置。</span><span class="sxs-lookup"><span data-stu-id="a0df4-155">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="a0df4-156">JSON 文件命名为跨平台应用程序标识符和承载在您的 HTTPS 域，在顶级域根目录或包括 sub 域。</span><span class="sxs-lookup"><span data-stu-id="a0df4-156">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="a0df4-157">例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。</span><span class="sxs-lookup"><span data-stu-id="a0df4-157">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="a0df4-158">您必须具有唯一文件和域 （或 sub 域），每个跨平台应用程序标识。</span><span class="sxs-lookup"><span data-stu-id="a0df4-158">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="a0df4-159">例如，Word 与 PowerPoint 的需要单独的文件和域。</span><span class="sxs-lookup"><span data-stu-id="a0df4-159">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="a0df4-160">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="a0df4-160">appDisplayName</span></span> | <span data-ttu-id="a0df4-161">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-161">String</span></span> | <span data-ttu-id="a0df4-162">可选。</span><span class="sxs-lookup"><span data-stu-id="a0df4-162">Optional.</span></span> <span data-ttu-id="a0df4-163">用于生成使用活动情况下，用户的本地设备上未安装应用程序时应用程序的简短的文本说明。</span><span class="sxs-lookup"><span data-stu-id="a0df4-163">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="a0df4-164">activationUrl</span><span class="sxs-lookup"><span data-stu-id="a0df4-164">activationUrl</span></span> | <span data-ttu-id="a0df4-165">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-165">String</span></span> | <span data-ttu-id="a0df4-166">必需项。</span><span class="sxs-lookup"><span data-stu-id="a0df4-166">Required.</span></span> <span data-ttu-id="a0df4-167">用于启动最佳本机体验由 appId 中的活动 URL。</span><span class="sxs-lookup"><span data-stu-id="a0df4-167">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="a0df4-168">如果没有的本机应用程序存在，则可能会启动一个基于 web 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a0df4-168">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="a0df4-169">fallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a0df4-169">fallbackUrl</span></span> | <span data-ttu-id="a0df4-170">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-170">String</span></span> | <span data-ttu-id="a0df4-171">可选。</span><span class="sxs-lookup"><span data-stu-id="a0df4-171">Optional.</span></span> <span data-ttu-id="a0df4-172">用于启动基于 web 的应用程序中的活动如果可用的 URL。</span><span class="sxs-lookup"><span data-stu-id="a0df4-172">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="a0df4-173">contentUrl</span><span class="sxs-lookup"><span data-stu-id="a0df4-173">contentUrl</span></span> | <span data-ttu-id="a0df4-174">字符串</span><span class="sxs-lookup"><span data-stu-id="a0df4-174">String</span></span> | <span data-ttu-id="a0df4-175">可选。</span><span class="sxs-lookup"><span data-stu-id="a0df4-175">Optional.</span></span> <span data-ttu-id="a0df4-176">使用在事件的内容可以呈现之外的本机或基于 web 的应用程序体验 （例如，RSS 源中的项目的指针）。</span><span class="sxs-lookup"><span data-stu-id="a0df4-176">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="a0df4-177">visualElements</span><span class="sxs-lookup"><span data-stu-id="a0df4-177">visualElements</span></span>| [<span data-ttu-id="a0df4-178">visualInfo</span><span class="sxs-lookup"><span data-stu-id="a0df4-178">visualInfo</span></span>](../resources/projectrome_visualinfo.md) | <span data-ttu-id="a0df4-179">必需。</span><span class="sxs-lookup"><span data-stu-id="a0df4-179">Required.</span></span> <span data-ttu-id="a0df4-180">包含信息呈现体验中的活动的对象</span><span class="sxs-lookup"><span data-stu-id="a0df4-180">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="a0df4-181">contentInfo</span><span class="sxs-lookup"><span data-stu-id="a0df4-181">contentInfo</span></span> | <span data-ttu-id="a0df4-182">类型化的 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="a0df4-182">Untyped JSON object</span></span> | <span data-ttu-id="a0df4-183">可选。</span><span class="sxs-lookup"><span data-stu-id="a0df4-183">Optional.</span></span> <span data-ttu-id="a0df4-184">一个自定义的数据的 JSON LD 根据[schema.org](https://schema.org)语法的内容的可扩展说明。</span><span class="sxs-lookup"><span data-stu-id="a0df4-184">A custom piece of data - JSON-LD extensible description of content according to [schema.org](https://schema.org) syntax.</span></span>|
|<span data-ttu-id="a0df4-185">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a0df4-185">expirationDateTime</span></span> | <span data-ttu-id="a0df4-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0df4-186">DateTimeOffset</span></span> | <span data-ttu-id="a0df4-187">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="a0df4-187">Set by the server.</span></span> <span data-ttu-id="a0df4-188">采用 UTC 对象过期的服务器上时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0df4-188">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="a0df4-189">状态</span><span class="sxs-lookup"><span data-stu-id="a0df4-189">status</span></span> | <span data-ttu-id="a0df4-190">状态</span><span class="sxs-lookup"><span data-stu-id="a0df4-190">status</span></span> | <span data-ttu-id="a0df4-191">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="a0df4-191">Set by the server.</span></span> <span data-ttu-id="a0df4-192">一个用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="a0df4-192">A status code used to identify valid objects.</span></span> <span data-ttu-id="a0df4-193">值： 活动更新、 删除、 忽略。</span><span class="sxs-lookup"><span data-stu-id="a0df4-193">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0df4-194">Relationships</span><span class="sxs-lookup"><span data-stu-id="a0df4-194">Relationships</span></span>

|<span data-ttu-id="a0df4-195">关系</span><span class="sxs-lookup"><span data-stu-id="a0df4-195">Relationship</span></span> | <span data-ttu-id="a0df4-196">类型</span><span class="sxs-lookup"><span data-stu-id="a0df4-196">Type</span></span> | <span data-ttu-id="a0df4-197">说明</span><span class="sxs-lookup"><span data-stu-id="a0df4-197">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="a0df4-198">historyItems</span><span class="sxs-lookup"><span data-stu-id="a0df4-198">historyItems</span></span>| <span data-ttu-id="a0df4-199">[activityHistoryItem](../resources/projectrome_historyitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="a0df4-199">[activityHistoryItem](../resources/projectrome_historyitem.md) collection</span></span> | <span data-ttu-id="a0df4-200">可选。</span><span class="sxs-lookup"><span data-stu-id="a0df4-200">Optional.</span></span> <span data-ttu-id="a0df4-201">NavigationProperty/包容;导航到活动的 historyItems 属性。</span><span class="sxs-lookup"><span data-stu-id="a0df4-201">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0df4-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0df4-202">JSON representation</span></span>

<span data-ttu-id="a0df4-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0df4-203">Here is a JSON representation of the resource.</span></span>

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
