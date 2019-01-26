---
title: 活动资源类型
description: 表示应用程序-例如，TV 显示、 文档或视频游戏中的当前市场活动中的单个活动。 当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 3d05c684d9498378a07a944f7aebd5e8a6b97f53
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573835"
---
# <a name="activity-resource-type"></a><span data-ttu-id="4d21d-105">活动资源类型</span><span class="sxs-lookup"><span data-stu-id="4d21d-105">activity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d21d-106">表示应用程序-例如，TV 显示、 文档或视频游戏中的当前市场活动中的单个活动。</span><span class="sxs-lookup"><span data-stu-id="4d21d-106">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="4d21d-107">当用户启动与该活动时，此服务捕获作为[历史记录项](projectrome-historyitem.md)，指示该活动的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="4d21d-107">When a user engages with that activity, the engagement is captured as a [history item](projectrome-historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="4d21d-108">根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。</span><span class="sxs-lookup"><span data-stu-id="4d21d-108">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="4d21d-109">您可以使用在 Microsoft Graph 活动使用户能够获得到它们在做什么其应用程序中跨多个设备。</span><span class="sxs-lookup"><span data-stu-id="4d21d-109">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="4d21d-110">您的应用程序创建的活动显示所有用户在设备上，并向用户公开为深度链接到您的应用程序中的特定内容。</span><span class="sxs-lookup"><span data-stu-id="4d21d-110">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="4d21d-111">您可以为在 Windows 中，并在 iOS 和通过 Cortana 通知 Android 设备上访问展示的目标应用程序中表示特定内容。</span><span class="sxs-lookup"><span data-stu-id="4d21d-111">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="4d21d-112">由于每个应用程序不同，这取决于您了解映射中将出现在 Cortana 和日程表的用户活动应用程序的操作的最佳方式。</span><span class="sxs-lookup"><span data-stu-id="4d21d-112">Because every app is different, it's up to you to understand the best way to map actions within your application to user activities that will appear in Cortana and Timeline.</span></span> <span data-ttu-id="4d21d-113">例如，游戏可能创建活动的每个市场活动、 文档创作应用程序可能会创建每个唯一的文档，活动和业务线应用程序可能会创建每个工作流活动。</span><span class="sxs-lookup"><span data-stu-id="4d21d-113">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="4d21d-114">用户活动将供展示中 Cortana 和 Windows 时间线用户体验，重点以帮助其选择回到从事过去的内容来提高用户工作效率和效率。</span><span class="sxs-lookup"><span data-stu-id="4d21d-114">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="4d21d-115">方法</span><span class="sxs-lookup"><span data-stu-id="4d21d-115">Methods</span></span>

|<span data-ttu-id="4d21d-116">方法</span><span class="sxs-lookup"><span data-stu-id="4d21d-116">Method</span></span> | <span data-ttu-id="4d21d-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="4d21d-117">Return Type</span></span> | <span data-ttu-id="4d21d-118">说明</span><span class="sxs-lookup"><span data-stu-id="4d21d-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="4d21d-119">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="4d21d-119">Create or replace activity</span></span>](../api/projectrome-put-activity.md) | [<span data-ttu-id="4d21d-120">活动</span><span class="sxs-lookup"><span data-stu-id="4d21d-120">activity</span></span>](projectrome-activity.md) |<span data-ttu-id="4d21d-121">创建或替换现有的活动 (upsert)。</span><span class="sxs-lookup"><span data-stu-id="4d21d-121">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="4d21d-122">AppActivityId 需要 URL 安全 （除 RFC 2396 必须将未保留的字符转换为十六进制表示形式为所有字符），但原始 appActivityId 不必是安全的 URL。</span><span class="sxs-lookup"><span data-stu-id="4d21d-122">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="4d21d-123">删除活动</span><span class="sxs-lookup"><span data-stu-id="4d21d-123">Delete an activity</span></span>](../api/projectrome-delete-activity.md) | <span data-ttu-id="4d21d-124">无内容</span><span class="sxs-lookup"><span data-stu-id="4d21d-124">No Content</span></span> | <span data-ttu-id="4d21d-125">从您的应用程序中删除指定为该用户的活动。</span><span class="sxs-lookup"><span data-stu-id="4d21d-125">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="4d21d-126">获取活动</span><span class="sxs-lookup"><span data-stu-id="4d21d-126">Get activities</span></span>](../api/projectrome-get-activities.md) | <span data-ttu-id="4d21d-127">[活动](projectrome-activity.md)的集合</span><span class="sxs-lookup"><span data-stu-id="4d21d-127">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="4d21d-128">获取指定用户的应用程序的活动。</span><span class="sxs-lookup"><span data-stu-id="4d21d-128">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="4d21d-129">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="4d21d-129">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md) | <span data-ttu-id="4d21d-130">[活动](projectrome-activity.md)的集合</span><span class="sxs-lookup"><span data-stu-id="4d21d-130">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="4d21d-131">为给定的用户、 排序和基于[historyItems](projectrome-historyitem.md)最近创建或更新您的应用程序获取最新的活动。</span><span class="sxs-lookup"><span data-stu-id="4d21d-131">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome-historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="4d21d-132">属性</span><span class="sxs-lookup"><span data-stu-id="4d21d-132">Properties</span></span>

|<span data-ttu-id="4d21d-133">名称</span><span class="sxs-lookup"><span data-stu-id="4d21d-133">Name</span></span> | <span data-ttu-id="4d21d-134">类型</span><span class="sxs-lookup"><span data-stu-id="4d21d-134">Type</span></span> | <span data-ttu-id="4d21d-135">说明</span><span class="sxs-lookup"><span data-stu-id="4d21d-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4d21d-136">userTimezone</span><span class="sxs-lookup"><span data-stu-id="4d21d-136">userTimezone</span></span> | <span data-ttu-id="4d21d-137">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-137">String</span></span> | <span data-ttu-id="4d21d-138">可选。</span><span class="sxs-lookup"><span data-stu-id="4d21d-138">Optional.</span></span> <span data-ttu-id="4d21d-139">在其中用于生成活动的用户的设备已位于在活动创建时; timezone为了支持跨平台表示形式作为 Olson Id 提供的值。</span><span class="sxs-lookup"><span data-stu-id="4d21d-139">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="4d21d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d21d-140">createdDateTime</span></span> | <span data-ttu-id="4d21d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d21d-141">DateTimeOffset</span></span> | <span data-ttu-id="4d21d-142">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="4d21d-142">Set by the server.</span></span> <span data-ttu-id="4d21d-143">采用 UTC 的服务器上创建对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4d21d-143">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="4d21d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d21d-144">lastModifiedDateTime</span></span> | <span data-ttu-id="4d21d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d21d-145">DateTimeOffset</span></span> | <span data-ttu-id="4d21d-146">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="4d21d-146">Set by the server.</span></span> <span data-ttu-id="4d21d-147">采用 UTC 的服务器上修改对象时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4d21d-147">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="4d21d-148">id</span><span class="sxs-lookup"><span data-stu-id="4d21d-148">id</span></span> | <span data-ttu-id="4d21d-149">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-149">String</span></span> | <span data-ttu-id="4d21d-150">使用的 URL 地址的服务器生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="4d21d-150">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="4d21d-151">appActivityId</span><span class="sxs-lookup"><span data-stu-id="4d21d-151">appActivityId</span></span> | <span data-ttu-id="4d21d-152">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-152">String</span></span> | <span data-ttu-id="4d21d-153">必需。</span><span class="sxs-lookup"><span data-stu-id="4d21d-153">Required.</span></span> <span data-ttu-id="4d21d-154">应用程序-此后提供呼叫者和不可变的上下文中唯一的活动 ID。</span><span class="sxs-lookup"><span data-stu-id="4d21d-154">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="4d21d-155">activitySourceHost</span><span class="sxs-lookup"><span data-stu-id="4d21d-155">activitySourceHost</span></span> | <span data-ttu-id="4d21d-156">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-156">String</span></span> | <span data-ttu-id="4d21d-157">必需。</span><span class="sxs-lookup"><span data-stu-id="4d21d-157">Required.</span></span> <span data-ttu-id="4d21d-158">表示应用程序的跨平台标识映射的域的 URL。</span><span class="sxs-lookup"><span data-stu-id="4d21d-158">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="4d21d-159">映射是存储也为 JSON 文件域上托管或通过 Windows 开发人员中心可配置。</span><span class="sxs-lookup"><span data-stu-id="4d21d-159">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="4d21d-160">JSON 文件命名为跨平台应用程序标识符和承载在您的 HTTPS 域，在顶级域根目录或包括 sub 域。</span><span class="sxs-lookup"><span data-stu-id="4d21d-160">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="4d21d-161">例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。</span><span class="sxs-lookup"><span data-stu-id="4d21d-161">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="4d21d-162">您必须具有唯一文件和域 （或 sub 域），每个跨平台应用程序标识。</span><span class="sxs-lookup"><span data-stu-id="4d21d-162">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="4d21d-163">例如，Word 与 PowerPoint 的需要单独的文件和域。</span><span class="sxs-lookup"><span data-stu-id="4d21d-163">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="4d21d-164">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="4d21d-164">appDisplayName</span></span> | <span data-ttu-id="4d21d-165">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-165">String</span></span> | <span data-ttu-id="4d21d-166">可选。</span><span class="sxs-lookup"><span data-stu-id="4d21d-166">Optional.</span></span> <span data-ttu-id="4d21d-167">用于生成使用活动情况下，用户的本地设备上未安装应用程序时应用程序的简短的文本说明。</span><span class="sxs-lookup"><span data-stu-id="4d21d-167">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="4d21d-168">activationUrl</span><span class="sxs-lookup"><span data-stu-id="4d21d-168">activationUrl</span></span> | <span data-ttu-id="4d21d-169">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-169">String</span></span> | <span data-ttu-id="4d21d-170">必需。</span><span class="sxs-lookup"><span data-stu-id="4d21d-170">Required.</span></span> <span data-ttu-id="4d21d-171">用于启动最佳本机体验由 appId 中的活动 URL。</span><span class="sxs-lookup"><span data-stu-id="4d21d-171">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="4d21d-172">如果没有的本机应用程序存在，则可能会启动一个基于 web 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4d21d-172">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="4d21d-173">fallbackUrl</span><span class="sxs-lookup"><span data-stu-id="4d21d-173">fallbackUrl</span></span> | <span data-ttu-id="4d21d-174">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-174">String</span></span> | <span data-ttu-id="4d21d-175">可选。</span><span class="sxs-lookup"><span data-stu-id="4d21d-175">Optional.</span></span> <span data-ttu-id="4d21d-176">用于启动基于 web 的应用程序中的活动如果可用的 URL。</span><span class="sxs-lookup"><span data-stu-id="4d21d-176">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="4d21d-177">contentUrl</span><span class="sxs-lookup"><span data-stu-id="4d21d-177">contentUrl</span></span> | <span data-ttu-id="4d21d-178">String</span><span class="sxs-lookup"><span data-stu-id="4d21d-178">String</span></span> | <span data-ttu-id="4d21d-179">可选。</span><span class="sxs-lookup"><span data-stu-id="4d21d-179">Optional.</span></span> <span data-ttu-id="4d21d-180">使用在事件的内容可以呈现之外的本机或基于 web 的应用程序体验 （例如，RSS 源中的项目的指针）。</span><span class="sxs-lookup"><span data-stu-id="4d21d-180">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="4d21d-181">visualElements</span><span class="sxs-lookup"><span data-stu-id="4d21d-181">visualElements</span></span>| [<span data-ttu-id="4d21d-182">visualInfo</span><span class="sxs-lookup"><span data-stu-id="4d21d-182">visualInfo</span></span>](../resources/projectrome-visualinfo.md) | <span data-ttu-id="4d21d-183">必需。</span><span class="sxs-lookup"><span data-stu-id="4d21d-183">Required.</span></span> <span data-ttu-id="4d21d-184">包含信息呈现体验中的活动的对象</span><span class="sxs-lookup"><span data-stu-id="4d21d-184">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="4d21d-185">contentInfo</span><span class="sxs-lookup"><span data-stu-id="4d21d-185">contentInfo</span></span> | <span data-ttu-id="4d21d-186">类型化的 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="4d21d-186">Untyped JSON object</span></span> | <span data-ttu-id="4d21d-187">可选。</span><span class="sxs-lookup"><span data-stu-id="4d21d-187">Optional.</span></span> <span data-ttu-id="4d21d-188">一个自定义的数据的 JSON LD 根据[schema.org](https://schema.org)语法的内容的可扩展说明。</span><span class="sxs-lookup"><span data-stu-id="4d21d-188">A custom piece of data - JSON-LD extensible description of content according to [schema.org](https://schema.org) syntax.</span></span>|
|<span data-ttu-id="4d21d-189">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4d21d-189">expirationDateTime</span></span> | <span data-ttu-id="4d21d-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d21d-190">DateTimeOffset</span></span> | <span data-ttu-id="4d21d-191">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="4d21d-191">Set by the server.</span></span> <span data-ttu-id="4d21d-192">采用 UTC 对象过期的服务器上时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4d21d-192">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="4d21d-193">status</span><span class="sxs-lookup"><span data-stu-id="4d21d-193">status</span></span> | <span data-ttu-id="4d21d-194">枚举字符串</span><span class="sxs-lookup"><span data-stu-id="4d21d-194">enum-string</span></span> | <span data-ttu-id="4d21d-195">由服务器设置。</span><span class="sxs-lookup"><span data-stu-id="4d21d-195">Set by the server.</span></span> <span data-ttu-id="4d21d-196">一个用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="4d21d-196">A status code used to identify valid objects.</span></span> <span data-ttu-id="4d21d-197">值： 活动更新、 删除、 忽略。</span><span class="sxs-lookup"><span data-stu-id="4d21d-197">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d21d-198">关系</span><span class="sxs-lookup"><span data-stu-id="4d21d-198">Relationships</span></span>

|<span data-ttu-id="4d21d-199">关系</span><span class="sxs-lookup"><span data-stu-id="4d21d-199">Relationship</span></span> | <span data-ttu-id="4d21d-200">类型</span><span class="sxs-lookup"><span data-stu-id="4d21d-200">Type</span></span> | <span data-ttu-id="4d21d-201">说明</span><span class="sxs-lookup"><span data-stu-id="4d21d-201">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="4d21d-202">historyItems</span><span class="sxs-lookup"><span data-stu-id="4d21d-202">historyItems</span></span>| <span data-ttu-id="4d21d-203">[historyItem](../resources/projectrome-historyitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="4d21d-203">[historyItem](../resources/projectrome-historyitem.md) collection</span></span> | <span data-ttu-id="4d21d-204">可选。</span><span class="sxs-lookup"><span data-stu-id="4d21d-204">Optional.</span></span> <span data-ttu-id="4d21d-205">NavigationProperty/包容;导航到活动的 historyItems 属性。</span><span class="sxs-lookup"><span data-stu-id="4d21d-205">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d21d-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d21d-206">JSON representation</span></span>

<span data-ttu-id="4d21d-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d21d-207">Here is a JSON representation of the resource.</span></span>

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
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@data.type": "microsoft.graph.Json" },
    "visualElements": { "@data.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.historyItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
