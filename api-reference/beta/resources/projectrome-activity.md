---
title: 活动资源类型
description: 代表某个应用程序内的单个活动，例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时，会将该预订作为历史项目进行捕获，以指示该活动的开始时间和结束时间。 随着时间的推移，用户随着时间的推移而重新参与该活动，会为单个用户活动记录多个历史记录项目。
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: f72a63280df3cb32d7814cd00f28ac457880d67e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026521"
---
# <a name="activity-resource-type"></a><span data-ttu-id="3c584-105">活动资源类型</span><span class="sxs-lookup"><span data-stu-id="3c584-105">activity resource type</span></span>

<span data-ttu-id="3c584-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c584-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c584-107">代表某个应用程序内的单个活动，例如电视节目、文档或视频游戏中的当前市场活动。</span><span class="sxs-lookup"><span data-stu-id="3c584-107">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="3c584-108">当用户参与该活动时，会将该预订作为 [历史项目](projectrome-historyitem.md) 进行捕获，以指示该活动的开始时间和结束时间。</span><span class="sxs-lookup"><span data-stu-id="3c584-108">When a user engages with that activity, the engagement is captured as a [history item](projectrome-historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="3c584-109">随着时间的推移，用户随着时间的推移而重新参与该活动，会为单个用户活动记录多个历史记录项目。</span><span class="sxs-lookup"><span data-stu-id="3c584-109">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="3c584-110">您可以使用 Microsoft Graph 中的活动来使用户能够返回到在其应用程序中的多个设备上执行的操作。</span><span class="sxs-lookup"><span data-stu-id="3c584-110">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="3c584-111">您的应用程序创建的活动将显示在所有用户的设备上，并向用户公开为您的应用程序中的特定内容的深层链接。</span><span class="sxs-lookup"><span data-stu-id="3c584-111">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="3c584-112">您可以将应用程序中的特定内容表示为在 Windows 中 showcased 的目标，并通过 Cortana 通知在 iOS 和 Android 设备上访问。</span><span class="sxs-lookup"><span data-stu-id="3c584-112">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="3c584-113">由于每个应用程序都不同，因此您可以了解将应用程序内的操作映射到将在 Cortana 和时间线中显示的用户活动的最佳方式。</span><span class="sxs-lookup"><span data-stu-id="3c584-113">Because every app is different, it's up to you to understand the best way to map actions within your application to user activities that will appear in Cortana and Timeline.</span></span> <span data-ttu-id="3c584-114">例如，游戏可能会为每个市场活动创建一个活动，文档创作应用程序可能会为每个唯一文档创建一个活动，并且业务线应用程序可能会为每个工作流创建一个活动。</span><span class="sxs-lookup"><span data-stu-id="3c584-114">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="3c584-115">你的用户活动将 showcased 在 Cortana 和 Windows 时间线用户体验中，这主要是为了提高用户的工作效率和效率，因为它可帮助他们获取过去对用户的工作内容。</span><span class="sxs-lookup"><span data-stu-id="3c584-115">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="3c584-116">方法</span><span class="sxs-lookup"><span data-stu-id="3c584-116">Methods</span></span>

|<span data-ttu-id="3c584-117">方法</span><span class="sxs-lookup"><span data-stu-id="3c584-117">Method</span></span> | <span data-ttu-id="3c584-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c584-118">Return Type</span></span> | <span data-ttu-id="3c584-119">说明</span><span class="sxs-lookup"><span data-stu-id="3c584-119">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="3c584-120">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="3c584-120">Create or replace activity</span></span>](../api/projectrome-put-activity.md) | [<span data-ttu-id="3c584-121">活动</span><span class="sxs-lookup"><span data-stu-id="3c584-121">activity</span></span>](projectrome-activity.md) |<span data-ttu-id="3c584-122">创建或替换现有活动 (upsert) 。</span><span class="sxs-lookup"><span data-stu-id="3c584-122">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="3c584-123">AppActivityId 需要是 URL 安全 (除 RFC 2396 非保留字符之外的所有字符都必须转换为十六进制表示形式) ，但原始 appActivityId 不必是 URL 安全的。</span><span class="sxs-lookup"><span data-stu-id="3c584-123">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="3c584-124">删除活动</span><span class="sxs-lookup"><span data-stu-id="3c584-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md) | <span data-ttu-id="3c584-125">无内容</span><span class="sxs-lookup"><span data-stu-id="3c584-125">No Content</span></span> | <span data-ttu-id="3c584-126">从您的应用程序中删除该用户的指定活动。</span><span class="sxs-lookup"><span data-stu-id="3c584-126">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="3c584-127">获取活动</span><span class="sxs-lookup"><span data-stu-id="3c584-127">Get activities</span></span>](../api/projectrome-get-activities.md) | <span data-ttu-id="3c584-128">[活动](projectrome-activity.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c584-128">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="3c584-129">获取适用于给定用户的应用程序活动。</span><span class="sxs-lookup"><span data-stu-id="3c584-129">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="3c584-130">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="3c584-130">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md) | <span data-ttu-id="3c584-131">[活动](projectrome-activity.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c584-131">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="3c584-132">为给定用户获取应用程序最近的活动，并根据最近创建或更新的 [historyItems](projectrome-historyitem.md)对其进行排序。</span><span class="sxs-lookup"><span data-stu-id="3c584-132">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome-historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="3c584-133">属性</span><span class="sxs-lookup"><span data-stu-id="3c584-133">Properties</span></span>

|<span data-ttu-id="3c584-134">名称</span><span class="sxs-lookup"><span data-stu-id="3c584-134">Name</span></span> | <span data-ttu-id="3c584-135">类型</span><span class="sxs-lookup"><span data-stu-id="3c584-135">Type</span></span> | <span data-ttu-id="3c584-136">说明</span><span class="sxs-lookup"><span data-stu-id="3c584-136">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="3c584-137">userTimezone</span><span class="sxs-lookup"><span data-stu-id="3c584-137">userTimezone</span></span> | <span data-ttu-id="3c584-138">String</span><span class="sxs-lookup"><span data-stu-id="3c584-138">String</span></span> | <span data-ttu-id="3c584-139">可选。</span><span class="sxs-lookup"><span data-stu-id="3c584-139">Optional.</span></span> <span data-ttu-id="3c584-140">用于生成活动的用户设备所在的时区位于活动创建时;作为 Olson Id 提供的值，以便支持跨平台表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c584-140">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="3c584-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c584-141">createdDateTime</span></span> | <span data-ttu-id="3c584-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c584-142">DateTimeOffset</span></span> | <span data-ttu-id="3c584-143">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="3c584-143">Set by the server.</span></span> <span data-ttu-id="3c584-144">在服务器上创建对象时的 UTC 时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="3c584-144">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="3c584-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c584-145">lastModifiedDateTime</span></span> | <span data-ttu-id="3c584-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c584-146">DateTimeOffset</span></span> | <span data-ttu-id="3c584-147">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="3c584-147">Set by the server.</span></span> <span data-ttu-id="3c584-148">在服务器上修改对象时的 UTC 时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="3c584-148">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="3c584-149">id</span><span class="sxs-lookup"><span data-stu-id="3c584-149">id</span></span> | <span data-ttu-id="3c584-150">String</span><span class="sxs-lookup"><span data-stu-id="3c584-150">String</span></span> | <span data-ttu-id="3c584-151">用于 URL 寻址的服务器生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="3c584-151">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="3c584-152">appActivityId</span><span class="sxs-lookup"><span data-stu-id="3c584-152">appActivityId</span></span> | <span data-ttu-id="3c584-153">String</span><span class="sxs-lookup"><span data-stu-id="3c584-153">String</span></span> | <span data-ttu-id="3c584-154">必需。</span><span class="sxs-lookup"><span data-stu-id="3c584-154">Required.</span></span> <span data-ttu-id="3c584-155">由呼叫者提供的应用程序上下文中的唯一活动 ID，之后是不可变的。</span><span class="sxs-lookup"><span data-stu-id="3c584-155">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="3c584-156">activitySourceHost</span><span class="sxs-lookup"><span data-stu-id="3c584-156">activitySourceHost</span></span> | <span data-ttu-id="3c584-157">String</span><span class="sxs-lookup"><span data-stu-id="3c584-157">String</span></span> | <span data-ttu-id="3c584-158">必需。</span><span class="sxs-lookup"><span data-stu-id="3c584-158">Required.</span></span> <span data-ttu-id="3c584-159">表示应用程序的跨平台标识映射的域的 URL。</span><span class="sxs-lookup"><span data-stu-id="3c584-159">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="3c584-160">映射存储为托管在域中或通过 Windows 开发人员中心配置的 JSON 文件。</span><span class="sxs-lookup"><span data-stu-id="3c584-160">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="3c584-161">JSON 文件命名为跨平台-应用标识符，并在您的 HTTPS 域的根目录（位于顶级域或包含子域）中托管。</span><span class="sxs-lookup"><span data-stu-id="3c584-161">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="3c584-162">例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。</span><span class="sxs-lookup"><span data-stu-id="3c584-162">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="3c584-163">您必须具有唯一的文件和域 (或子域) 每个跨平台应用程序标识。</span><span class="sxs-lookup"><span data-stu-id="3c584-163">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="3c584-164">例如，Word 与 PowerPoint 需要一个单独的文件和域。</span><span class="sxs-lookup"><span data-stu-id="3c584-164">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="3c584-165">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c584-165">appDisplayName</span></span> | <span data-ttu-id="3c584-166">String</span><span class="sxs-lookup"><span data-stu-id="3c584-166">String</span></span> | <span data-ttu-id="3c584-167">可选。</span><span class="sxs-lookup"><span data-stu-id="3c584-167">Optional.</span></span> <span data-ttu-id="3c584-168">用于生成活动的应用程序的简短文本说明，在用户的本地设备上未安装应用程序时用于生成活动的情况。</span><span class="sxs-lookup"><span data-stu-id="3c584-168">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="3c584-169">activationUrl</span><span class="sxs-lookup"><span data-stu-id="3c584-169">activationUrl</span></span> | <span data-ttu-id="3c584-170">String</span><span class="sxs-lookup"><span data-stu-id="3c584-170">String</span></span> | <span data-ttu-id="3c584-171">必需。</span><span class="sxs-lookup"><span data-stu-id="3c584-171">Required.</span></span> <span data-ttu-id="3c584-172">用于在由 appId 表示的最佳本机体验中启动活动的 URL。</span><span class="sxs-lookup"><span data-stu-id="3c584-172">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="3c584-173">如果不存在本机应用程序，则可能启动基于 web 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="3c584-173">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="3c584-174">fallbackUrl</span><span class="sxs-lookup"><span data-stu-id="3c584-174">fallbackUrl</span></span> | <span data-ttu-id="3c584-175">String</span><span class="sxs-lookup"><span data-stu-id="3c584-175">String</span></span> | <span data-ttu-id="3c584-176">可选。</span><span class="sxs-lookup"><span data-stu-id="3c584-176">Optional.</span></span> <span data-ttu-id="3c584-177">用于在基于 web 的应用程序中启动活动的 URL （如果有）。</span><span class="sxs-lookup"><span data-stu-id="3c584-177">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="3c584-178">contentUrl</span><span class="sxs-lookup"><span data-stu-id="3c584-178">contentUrl</span></span> | <span data-ttu-id="3c584-179">String</span><span class="sxs-lookup"><span data-stu-id="3c584-179">String</span></span> | <span data-ttu-id="3c584-180">可选。</span><span class="sxs-lookup"><span data-stu-id="3c584-180">Optional.</span></span> <span data-ttu-id="3c584-181">当内容可以在本机或基于 web 的应用程序体验之外呈现时使用 (例如，指向 RSS 源) 中的项的指针。</span><span class="sxs-lookup"><span data-stu-id="3c584-181">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="3c584-182">visualElements</span><span class="sxs-lookup"><span data-stu-id="3c584-182">visualElements</span></span>| [<span data-ttu-id="3c584-183">visualInfo</span><span class="sxs-lookup"><span data-stu-id="3c584-183">visualInfo</span></span>](../resources/projectrome-visualinfo.md) | <span data-ttu-id="3c584-184">必需。</span><span class="sxs-lookup"><span data-stu-id="3c584-184">Required.</span></span> <span data-ttu-id="3c584-185">包含用于在 UX 中呈现活动的信息的对象。</span><span class="sxs-lookup"><span data-stu-id="3c584-185">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="3c584-186">contentInfo</span><span class="sxs-lookup"><span data-stu-id="3c584-186">contentInfo</span></span> | <span data-ttu-id="3c584-187">非类型化 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="3c584-187">Untyped JSON object</span></span> | <span data-ttu-id="3c584-188">可选。</span><span class="sxs-lookup"><span data-stu-id="3c584-188">Optional.</span></span> <span data-ttu-id="3c584-189">根据 [schema.org](https://schema.org) 语法的内容的自定义数据 JSON-LD 可扩展说明。</span><span class="sxs-lookup"><span data-stu-id="3c584-189">A custom piece of data - JSON-LD extensible description of content according to [schema.org](https://schema.org) syntax.</span></span>|
|<span data-ttu-id="3c584-190">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3c584-190">expirationDateTime</span></span> | <span data-ttu-id="3c584-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c584-191">DateTimeOffset</span></span> | <span data-ttu-id="3c584-192">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="3c584-192">Set by the server.</span></span> <span data-ttu-id="3c584-193">当对象在服务器上过期时的日期时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="3c584-193">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="3c584-194">状态</span><span class="sxs-lookup"><span data-stu-id="3c584-194">status</span></span> | <span data-ttu-id="3c584-195">string</span><span class="sxs-lookup"><span data-stu-id="3c584-195">string</span></span> | <span data-ttu-id="3c584-196">由服务器进行设置。</span><span class="sxs-lookup"><span data-stu-id="3c584-196">Set by the server.</span></span> <span data-ttu-id="3c584-197">用于标识有效对象的状态代码。</span><span class="sxs-lookup"><span data-stu-id="3c584-197">A status code used to identify valid objects.</span></span> <span data-ttu-id="3c584-198">值：活动、已更新、已删除、已忽略。</span><span class="sxs-lookup"><span data-stu-id="3c584-198">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c584-199">关系</span><span class="sxs-lookup"><span data-stu-id="3c584-199">Relationships</span></span>

|<span data-ttu-id="3c584-200">关系</span><span class="sxs-lookup"><span data-stu-id="3c584-200">Relationship</span></span> | <span data-ttu-id="3c584-201">类型</span><span class="sxs-lookup"><span data-stu-id="3c584-201">Type</span></span> | <span data-ttu-id="3c584-202">说明</span><span class="sxs-lookup"><span data-stu-id="3c584-202">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="3c584-203">historyItems</span><span class="sxs-lookup"><span data-stu-id="3c584-203">historyItems</span></span>| <span data-ttu-id="3c584-204">[historyItem](../resources/projectrome-historyitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c584-204">[historyItem](../resources/projectrome-historyitem.md) collection</span></span> | <span data-ttu-id="3c584-205">可选。</span><span class="sxs-lookup"><span data-stu-id="3c584-205">Optional.</span></span> <span data-ttu-id="3c584-206">NavigationProperty/包含;指向活动的 historyItems 的导航属性。</span><span class="sxs-lookup"><span data-stu-id="3c584-206">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c584-207">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c584-207">JSON representation</span></span>

<span data-ttu-id="3c584-208">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c584-208">Here is a JSON representation of the resource.</span></span>

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
  "keyProperty": "id",
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
    "status": "string",
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
  "suppressions": []
}
-->


