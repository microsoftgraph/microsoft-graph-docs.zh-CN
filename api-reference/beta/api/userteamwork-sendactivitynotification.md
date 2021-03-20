---
title: userTeamwork： sendActivityNotification
description: 向用户发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 73acd02d0189a4eb1c26f533e13b31b101a1fa7e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941935"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="804db-103">userTeamwork： sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="804db-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="804db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="804db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="804db-105">向用户发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="804db-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="804db-106">有关发送通知的更多详细信息以及发送通知的要求，请参阅 [发送 Teams 活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="804db-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="804db-107">权限</span><span class="sxs-lookup"><span data-stu-id="804db-107">Permissions</span></span>
<span data-ttu-id="804db-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="804db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="804db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="804db-110">Permission type</span></span>|<span data-ttu-id="804db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="804db-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="804db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="804db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="804db-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="804db-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="804db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="804db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="804db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="804db-115">Not Supported.</span></span>|
|<span data-ttu-id="804db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="804db-116">Application</span></span>|<span data-ttu-id="804db-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="804db-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="804db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="804db-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="804db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="804db-119">Request headers</span></span>
|<span data-ttu-id="804db-120">名称</span><span class="sxs-lookup"><span data-stu-id="804db-120">Name</span></span>|<span data-ttu-id="804db-121">说明</span><span class="sxs-lookup"><span data-stu-id="804db-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="804db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="804db-122">Authorization</span></span>|<span data-ttu-id="804db-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="804db-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="804db-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="804db-125">Content-Type</span></span>|<span data-ttu-id="804db-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="804db-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="804db-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="804db-128">Request body</span></span>
<span data-ttu-id="804db-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="804db-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="804db-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="804db-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="804db-131">参数</span><span class="sxs-lookup"><span data-stu-id="804db-131">Parameter</span></span>|<span data-ttu-id="804db-132">类型</span><span class="sxs-lookup"><span data-stu-id="804db-132">Type</span></span>|<span data-ttu-id="804db-133">说明</span><span class="sxs-lookup"><span data-stu-id="804db-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="804db-134">topic</span><span class="sxs-lookup"><span data-stu-id="804db-134">topic</span></span>|[<span data-ttu-id="804db-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="804db-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="804db-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="804db-136">Topic of the notification.</span></span> <span data-ttu-id="804db-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="804db-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="804db-138">activityType</span><span class="sxs-lookup"><span data-stu-id="804db-138">activityType</span></span>|<span data-ttu-id="804db-139">String</span><span class="sxs-lookup"><span data-stu-id="804db-139">String</span></span>|<span data-ttu-id="804db-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="804db-140">Activity type.</span></span> <span data-ttu-id="804db-141">这必须在 Teams 应用清单 [中声明](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="804db-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="804db-142">chainId</span><span class="sxs-lookup"><span data-stu-id="804db-142">chainId</span></span>|<span data-ttu-id="804db-143">Int64</span><span class="sxs-lookup"><span data-stu-id="804db-143">Int64</span></span>|<span data-ttu-id="804db-144">可选。</span><span class="sxs-lookup"><span data-stu-id="804db-144">Optional.</span></span> <span data-ttu-id="804db-145">用于替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="804db-145">Used to override a previous notification.</span></span> <span data-ttu-id="804db-146">在后续 `chainId` 请求中使用相同的方法替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="804db-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="804db-147">previewText</span><span class="sxs-lookup"><span data-stu-id="804db-147">previewText</span></span>|[<span data-ttu-id="804db-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="804db-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="804db-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="804db-149">Preview text for the notification.</span></span> <span data-ttu-id="804db-150">Microsoft Teams 将只显示前 150 个字符。</span><span class="sxs-lookup"><span data-stu-id="804db-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="804db-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="804db-151">templateParameters</span></span>|<span data-ttu-id="804db-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="804db-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="804db-153">在 Teams 应用清单 中对应的活动源条目中定义的 `activityType` 模板 [变量的值](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="804db-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="804db-154">将 topic 属性的值设置为 时 `source` ，支持 **以下** 资源 `entityUrl` ：</span><span class="sxs-lookup"><span data-stu-id="804db-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="804db-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="804db-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="804db-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="804db-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="804db-157">响应</span><span class="sxs-lookup"><span data-stu-id="804db-157">Response</span></span>

<span data-ttu-id="804db-158">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="804db-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="804db-159">示例</span><span class="sxs-lookup"><span data-stu-id="804db-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="804db-160">示例 1：向用户发送已创建任务的通知</span><span class="sxs-lookup"><span data-stu-id="804db-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="804db-161">请求</span><span class="sxs-lookup"><span data-stu-id="804db-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="804db-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="804db-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userteamwork_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="804db-163">C#</span><span class="sxs-lookup"><span data-stu-id="804db-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userteamwork-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="804db-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="804db-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userteamwork-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="804db-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="804db-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userteamwork-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="804db-166">Java</span><span class="sxs-lookup"><span data-stu-id="804db-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userteamwork-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="804db-167">响应</span><span class="sxs-lookup"><span data-stu-id="804db-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="804db-168">示例 2：使用自定义主题通知用户事件</span><span class="sxs-lookup"><span data-stu-id="804db-168">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="804db-169">如果要链接未由 Microsoft Graph 表示的方面，或者希望自定义名称，可以将 的源设置为 并传递其 `topic` `text` 自定义值。</span><span class="sxs-lookup"><span data-stu-id="804db-169">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="804db-170">`webUrl` 将 source 用作 时 `topic` 是必需的 `text` 。</span><span class="sxs-lookup"><span data-stu-id="804db-170">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="804db-171">请求</span><span class="sxs-lookup"><span data-stu-id="804db-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="804db-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="804db-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_4"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "deploymentApprovalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="804db-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="804db-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="804db-174">C#</span><span class="sxs-lookup"><span data-stu-id="804db-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="804db-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="804db-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="804db-176">Java</span><span class="sxs-lookup"><span data-stu-id="804db-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="804db-177">响应</span><span class="sxs-lookup"><span data-stu-id="804db-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
