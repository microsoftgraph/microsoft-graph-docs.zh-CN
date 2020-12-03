---
title: 'userTeamwork: sendActivityNotification'
description: 向用户发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ce246a04dae270d07abe0e16d3a133265db5b8d5
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522368"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="2bf2c-103">userTeamwork: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="2bf2c-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="2bf2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bf2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2bf2c-105">向用户发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="2bf2c-106">有关发送通知和执行此操作的要求的详细信息，请参阅 [发送团队活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bf2c-107">权限</span><span class="sxs-lookup"><span data-stu-id="2bf2c-107">Permissions</span></span>
<span data-ttu-id="2bf2c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bf2c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bf2c-110">Permission type</span></span>|<span data-ttu-id="2bf2c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2bf2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bf2c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bf2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bf2c-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="2bf2c-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="2bf2c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bf2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bf2c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-115">Not Supported.</span></span>|
|<span data-ttu-id="2bf2c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bf2c-116">Application</span></span>|<span data-ttu-id="2bf2c-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="2bf2c-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bf2c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bf2c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="2bf2c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bf2c-119">Request headers</span></span>
|<span data-ttu-id="2bf2c-120">名称</span><span class="sxs-lookup"><span data-stu-id="2bf2c-120">Name</span></span>|<span data-ttu-id="2bf2c-121">说明</span><span class="sxs-lookup"><span data-stu-id="2bf2c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2bf2c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bf2c-122">Authorization</span></span>|<span data-ttu-id="2bf2c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2bf2c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2bf2c-125">Content-Type</span></span>|<span data-ttu-id="2bf2c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2bf2c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bf2c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bf2c-128">Request body</span></span>
<span data-ttu-id="2bf2c-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2bf2c-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2bf2c-131">参数</span><span class="sxs-lookup"><span data-stu-id="2bf2c-131">Parameter</span></span>|<span data-ttu-id="2bf2c-132">类型</span><span class="sxs-lookup"><span data-stu-id="2bf2c-132">Type</span></span>|<span data-ttu-id="2bf2c-133">说明</span><span class="sxs-lookup"><span data-stu-id="2bf2c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bf2c-134">topic</span><span class="sxs-lookup"><span data-stu-id="2bf2c-134">topic</span></span>|[<span data-ttu-id="2bf2c-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="2bf2c-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="2bf2c-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-136">Topic of the notification.</span></span> <span data-ttu-id="2bf2c-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="2bf2c-138">activityType</span><span class="sxs-lookup"><span data-stu-id="2bf2c-138">activityType</span></span>|<span data-ttu-id="2bf2c-139">String</span><span class="sxs-lookup"><span data-stu-id="2bf2c-139">String</span></span>|<span data-ttu-id="2bf2c-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-140">Activity type.</span></span> <span data-ttu-id="2bf2c-141">必须在 [团队应用程序清单](/microsoftteams/platform/overview)中声明。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="2bf2c-142">chainId</span><span class="sxs-lookup"><span data-stu-id="2bf2c-142">chainId</span></span>|<span data-ttu-id="2bf2c-143">Int64</span><span class="sxs-lookup"><span data-stu-id="2bf2c-143">Int64</span></span>|<span data-ttu-id="2bf2c-144">可选。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-144">Optional.</span></span> <span data-ttu-id="2bf2c-145">用于替代以前的通知。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-145">Used to override a previous notification.</span></span> <span data-ttu-id="2bf2c-146">`chainId`在后续请求中使用相同的重写以前的通知。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="2bf2c-147">previewText</span><span class="sxs-lookup"><span data-stu-id="2bf2c-147">previewText</span></span>|[<span data-ttu-id="2bf2c-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="2bf2c-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="2bf2c-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-149">Preview text for the notification.</span></span> <span data-ttu-id="2bf2c-150">Microsoft 团队将仅显示前150个字符。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="2bf2c-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="2bf2c-151">templateParameters</span></span>|<span data-ttu-id="2bf2c-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2bf2c-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="2bf2c-153">在与 `activityType` [团队应用程序清单](/microsoftteams/platform/overview)对应的活动源条目中定义的模板变量的值。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="2bf2c-154">将主题属性的值设置为以下资源时，支持以下资源 `source` **topic** `entityUrl` ：</span><span class="sxs-lookup"><span data-stu-id="2bf2c-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="2bf2c-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2bf2c-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="2bf2c-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="2bf2c-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="2bf2c-157">响应</span><span class="sxs-lookup"><span data-stu-id="2bf2c-157">Response</span></span>

<span data-ttu-id="2bf2c-158">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2bf2c-159">示例</span><span class="sxs-lookup"><span data-stu-id="2bf2c-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="2bf2c-160">示例1：向已创建任务的用户发送通知</span><span class="sxs-lookup"><span data-stu-id="2bf2c-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="2bf2c-161">请求</span><span class="sxs-lookup"><span data-stu-id="2bf2c-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2bf2c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bf2c-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2bf2c-163">C#</span><span class="sxs-lookup"><span data-stu-id="2bf2c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userteamwork-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bf2c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bf2c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userteamwork-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bf2c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bf2c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userteamwork-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2bf2c-166">Java</span><span class="sxs-lookup"><span data-stu-id="2bf2c-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userteamwork-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2bf2c-167">响应</span><span class="sxs-lookup"><span data-stu-id="2bf2c-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="2bf2c-168">示例2：使用自定义主题通知用户有关事件</span><span class="sxs-lookup"><span data-stu-id="2bf2c-168">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="2bf2c-169">如果要链接不是由 Microsoft Graph 表示的方位，或者想要自定义该名称，可以为其设置源， `topic` `text` 并为其传入自定义值。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-169">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="2bf2c-170">`webUrl` 在使用源作为时，是必需的 `topic` `text` 。</span><span class="sxs-lookup"><span data-stu-id="2bf2c-170">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="2bf2c-171">请求</span><span class="sxs-lookup"><span data-stu-id="2bf2c-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2bf2c-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bf2c-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
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
# <a name="javascript"></a>[<span data-ttu-id="2bf2c-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bf2c-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2bf2c-174">响应</span><span class="sxs-lookup"><span data-stu-id="2bf2c-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
