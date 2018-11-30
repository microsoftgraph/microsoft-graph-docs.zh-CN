---
title: 活动资源类型
description: 表示应用程序-例如，TV 显示、 文档或视频游戏中的当前市场活动中的单个活动。 当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。
ms.openlocfilehash: 2c619cf2ad1707a8efa9d363344ccce93d92bb10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045606"
---
# <a name="activity-resource-type"></a><span data-ttu-id="0fd6d-105">活动资源类型</span><span class="sxs-lookup"><span data-stu-id="0fd6d-105">activity resource type</span></span>

> <span data-ttu-id="0fd6d-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fd6d-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fd6d-108">表示应用程序-例如，TV 显示、 文档或视频游戏中的当前市场活动中的单个活动。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-108">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="0fd6d-109">当用户启动与该活动时，此服务捕获作为[历史记录项](projectrome-historyitem.md)，指示该活动的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-109">When a user engages with that activity, the engagement is captured as a [history item](projectrome-historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="0fd6d-110">根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="0fd6d-111">您可以使用在 Microsoft Graph 活动使用户能够获得到它们在做什么其应用程序中跨多个设备。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-111">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="0fd6d-112">您的应用程序创建的活动显示所有用户在设备上，并向用户公开为深度链接到您的应用程序中的特定内容。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-112">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="0fd6d-113">您可以为在 Windows 中，并在 iOS 和通过 Cortana 通知 Android 设备上访问展示的目标应用程序中表示特定内容。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-113">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="0fd6d-114">由于每个应用程序不同，这取决于您了解映射中将出现在 Cortana 和日程表的用户活动应用程序的操作的最佳方式。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-114">Because every app is different, it's up to you to understand the best way to map actions within your application to user activities that will appear in Cortana and Timeline.</span></span> <span data-ttu-id="0fd6d-115">例如，游戏可能创建活动的每个市场活动、 文档创作应用程序可能会创建每个唯一的文档，活动和业务线应用程序可能会创建每个工作流活动。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-115">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="0fd6d-116">用户活动将供展示中 Cortana 和 Windows 时间线用户体验，重点以帮助其选择回到从事过去的内容来提高用户工作效率和效率。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-116">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="0fd6d-117">方法</span><span class="sxs-lookup"><span data-stu-id="0fd6d-117">Methods</span></span>

|<span data-ttu-id="0fd6d-118">方法</span><span class="sxs-lookup"><span data-stu-id="0fd6d-118">Method</span></span> | <span data-ttu-id="0fd6d-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fd6d-119">Return Type</span></span> | <span data-ttu-id="0fd6d-120">说明</span><span class="sxs-lookup"><span data-stu-id="0fd6d-120">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="0fd6d-121">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="0fd6d-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md) | [<span data-ttu-id="0fd6d-122">活动</span><span class="sxs-lookup"><span data-stu-id="0fd6d-122">activity</span></span>](projectrome-activity.md) |<span data-ttu-id="0fd6d-123">创建或替换现有的活动 (upsert)。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-123">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="0fd6d-124">AppActivityId 需要 URL 安全 （除 RFC 2396 必须将未保留的字符转换为十六进制表示形式为所有字符），但原始 appActivityId 不必是安全的 URL。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-124">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="0fd6d-125">删除活动</span><span class="sxs-lookup"><span data-stu-id="0fd6d-125">Delete an activity</span></span>](../api/projectrome-delete-activity.md) | <span data-ttu-id="0fd6d-126">无内容</span><span class="sxs-lookup"><span data-stu-id="0fd6d-126">No Content</span></span> | <span data-ttu-id="0fd6d-127">从您的应用程序中删除指定为该用户的活动。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-127">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="0fd6d-128">获取活动</span><span class="sxs-lookup"><span data-stu-id="0fd6d-128">Get activities</span></span>](../api/projectrome-get-activities.md) | <span data-ttu-id="0fd6d-129">[活动](projectrome-activity.md)的集合</span><span class="sxs-lookup"><span data-stu-id="0fd6d-129">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="0fd6d-130">获取指定用户的应用程序的活动。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-130">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="0fd6d-131">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="0fd6d-131">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md) | <span data-ttu-id="0fd6d-132">[活动](projectrome-activity.md)的集合</span><span class="sxs-lookup"><span data-stu-id="0fd6d-132">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="0fd6d-133">为给定的用户、 排序和基于[historyItems](projectrome-historyitem.md)最近创建或更新您的应用程序获取最新的活动。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-133">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome-historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="0fd6d-134">属性</span><span class="sxs-lookup"><span data-stu-id="0fd6d-134">Properties</span></span>

|<span data-ttu-id="0fd6d-135">名称</span><span class="sxs-lookup"><span data-stu-id="0fd6d-135">Name</span></span> | <span data-ttu-id="0fd6d-136">类型</span><span class="sxs-lookup"><span data-stu-id="0fd6d-136">Type</span></span> | <span data-ttu-id="0fd6d-137">说明</span><span class="sxs-lookup"><span data-stu-id="0fd6d-137">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="0fd6d-138">userTimezone</span><span class="sxs-lookup"><span data-stu-id="0fd6d-138">userTimezone</span></span> | <span data-ttu-id="0fd6d-139">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-139">String</span></span> | <span data-ttu-id="0fd6d-140">可选。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-140">Optional.</span></span> <span data-ttu-id="0fd6d-141">在其中用于生成活动的用户的设备已位于在活动创建时; timezone为了支持跨平台表示形式作为 Olson Id 提供的值。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-141">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="0fd6d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd6d-142">createdDateTime</span></span> | <span data-ttu-id="0fd6d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd6d-143">DateTimeOffset</span></span> | <span data-ttu-id="0fd6d-144">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-144">Set by the server.</span></span> <span data-ttu-id="0fd6d-145">采用 UTC 的服务器上创建对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-145">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="0fd6d-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd6d-146">lastModifiedDateTime</span></span> | <span data-ttu-id="0fd6d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd6d-147">DateTimeOffset</span></span> | <span data-ttu-id="0fd6d-148">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-148">Set by the server.</span></span> <span data-ttu-id="0fd6d-149">采用 UTC 的服务器上修改对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-149">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="0fd6d-150">id</span><span class="sxs-lookup"><span data-stu-id="0fd6d-150">id</span></span> | <span data-ttu-id="0fd6d-151">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-151">String</span></span> | <span data-ttu-id="0fd6d-152">使用的 URL 地址的服务器生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-152">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="0fd6d-153">appActivityId</span><span class="sxs-lookup"><span data-stu-id="0fd6d-153">appActivityId</span></span> | <span data-ttu-id="0fd6d-154">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-154">String</span></span> | <span data-ttu-id="0fd6d-155">必需项。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-155">Required.</span></span> <span data-ttu-id="0fd6d-156">应用程序-此后提供呼叫者和不可变的上下文中唯一的活动 ID。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-156">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="0fd6d-157">activitySourceHost</span><span class="sxs-lookup"><span data-stu-id="0fd6d-157">activitySourceHost</span></span> | <span data-ttu-id="0fd6d-158">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-158">String</span></span> | <span data-ttu-id="0fd6d-159">必需项。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-159">Required.</span></span> <span data-ttu-id="0fd6d-160">表示应用程序的跨平台标识映射的域的 URL。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-160">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="0fd6d-161">映射是存储也为 JSON 文件域上托管或通过 Windows 开发人员中心可配置。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-161">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="0fd6d-162">JSON 文件命名为跨平台应用程序标识符和承载在您的 HTTPS 域，在顶级域根目录或包括 sub 域。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-162">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="0fd6d-163">例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-163">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="0fd6d-164">您必须具有唯一文件和域 （或 sub 域），每个跨平台应用程序标识。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-164">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="0fd6d-165">例如，Word 与 PowerPoint 的需要单独的文件和域。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-165">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="0fd6d-166">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="0fd6d-166">appDisplayName</span></span> | <span data-ttu-id="0fd6d-167">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-167">String</span></span> | <span data-ttu-id="0fd6d-168">可选。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-168">Optional.</span></span> <span data-ttu-id="0fd6d-169">用于生成使用活动情况下，用户的本地设备上未安装应用程序时应用程序的简短的文本说明。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-169">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="0fd6d-170">activationUrl</span><span class="sxs-lookup"><span data-stu-id="0fd6d-170">activationUrl</span></span> | <span data-ttu-id="0fd6d-171">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-171">String</span></span> | <span data-ttu-id="0fd6d-172">必需项。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-172">Required.</span></span> <span data-ttu-id="0fd6d-173">用于启动最佳本机体验由 appId 中的活动 URL。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-173">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="0fd6d-174">如果没有的本机应用程序存在，则可能会启动一个基于 web 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-174">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="0fd6d-175">fallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0fd6d-175">fallbackUrl</span></span> | <span data-ttu-id="0fd6d-176">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-176">String</span></span> | <span data-ttu-id="0fd6d-177">可选。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-177">Optional.</span></span> <span data-ttu-id="0fd6d-178">用于启动基于 web 的应用程序中的活动如果可用的 URL。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-178">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="0fd6d-179">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0fd6d-179">contentUrl</span></span> | <span data-ttu-id="0fd6d-180">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd6d-180">String</span></span> | <span data-ttu-id="0fd6d-181">可选。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-181">Optional.</span></span> <span data-ttu-id="0fd6d-182">使用在事件的内容可以呈现之外的本机或基于 web 的应用程序体验 （例如，RSS 源中的项目的指针）。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-182">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="0fd6d-183">visualElements</span><span class="sxs-lookup"><span data-stu-id="0fd6d-183">visualElements</span></span>| [<span data-ttu-id="0fd6d-184">visualInfo</span><span class="sxs-lookup"><span data-stu-id="0fd6d-184">visualInfo</span></span>](../resources/projectrome-visualinfo.md) | <span data-ttu-id="0fd6d-185">必需。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-185">Required.</span></span> <span data-ttu-id="0fd6d-186">包含信息呈现体验中的活动的对象</span><span class="sxs-lookup"><span data-stu-id="0fd6d-186">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="0fd6d-187">contentInfo</span><span class="sxs-lookup"><span data-stu-id="0fd6d-187">contentInfo</span></span> | <span data-ttu-id="0fd6d-188">类型化的 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="0fd6d-188">Untyped JSON object</span></span> | <span data-ttu-id="0fd6d-189">可选。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-189">Optional.</span></span> <span data-ttu-id="0fd6d-190">一个自定义的数据的 JSON LD 根据[schema.org](https://schema.org)语法的内容的可扩展说明。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-190">A custom piece of data - JSON-LD extensible description of content according to [schema.org](https://schema.org) syntax.</span></span>|
|<span data-ttu-id="0fd6d-191">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd6d-191">expirationDateTime</span></span> | <span data-ttu-id="0fd6d-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd6d-192">DateTimeOffset</span></span> | <span data-ttu-id="0fd6d-193">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-193">Set by the server.</span></span> <span data-ttu-id="0fd6d-194">采用 UTC 对象过期的服务器上时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-194">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="0fd6d-195">状态</span><span class="sxs-lookup"><span data-stu-id="0fd6d-195">status</span></span> | <span data-ttu-id="0fd6d-196">EnumType</span><span class="sxs-lookup"><span data-stu-id="0fd6d-196">EnumType</span></span> | <span data-ttu-id="0fd6d-197">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-197">Set by the server.</span></span> <span data-ttu-id="0fd6d-198">一个用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-198">A status code used to identify valid objects.</span></span> <span data-ttu-id="0fd6d-199">值： 活动更新、 删除、 忽略。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-199">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fd6d-200">Relationships</span><span class="sxs-lookup"><span data-stu-id="0fd6d-200">Relationships</span></span>

|<span data-ttu-id="0fd6d-201">关系</span><span class="sxs-lookup"><span data-stu-id="0fd6d-201">Relationship</span></span> | <span data-ttu-id="0fd6d-202">类型</span><span class="sxs-lookup"><span data-stu-id="0fd6d-202">Type</span></span> | <span data-ttu-id="0fd6d-203">说明</span><span class="sxs-lookup"><span data-stu-id="0fd6d-203">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="0fd6d-204">historyItems</span><span class="sxs-lookup"><span data-stu-id="0fd6d-204">historyItems</span></span>| <span data-ttu-id="0fd6d-205">[historyItem](../resources/projectrome-historyitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fd6d-205">[historyItem](../resources/projectrome-historyitem.md) collection</span></span> | <span data-ttu-id="0fd6d-206">可选。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-206">Optional.</span></span> <span data-ttu-id="0fd6d-207">NavigationProperty/包容;导航到活动的 historyItems 属性。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-207">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fd6d-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fd6d-208">JSON representation</span></span>

<span data-ttu-id="0fd6d-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fd6d-209">Here is a JSON representation of the resource.</span></span>

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
  "@odata.type": "microsoft.graph.activity"
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
    "status": "EnumType",
    "contentInfo": { "@data.type": "microsoft.graph.Json" },
    "visualElements": { "@data.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.historyItem" }]
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
