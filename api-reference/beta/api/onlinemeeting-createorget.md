---
title: 'onlineMeeting: createOrGet'
description: 使用自定义指定的外部 ID 创建联机会议。 如果已存在外部 ID，此 API 将返回具有该外部 ID 的 onlineMeeting 对象。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 51e619e6f09f98fcaa12423881a930df72c0597a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980137"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="4e7e7-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="4e7e7-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="4e7e7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e7e7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e7e7-106">创建具有自定义的指定外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="4e7e7-107">如果已存在外部 ID，此 API 将返回具有该外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="4e7e7-108">**注释** ：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-108">**Note** : The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e7e7-109">权限</span><span class="sxs-lookup"><span data-stu-id="4e7e7-109">Permissions</span></span>
<span data-ttu-id="4e7e7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e7e7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e7e7-112">Permission type</span></span>                        | <span data-ttu-id="4e7e7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e7e7-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4e7e7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e7e7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e7e7-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e7e7-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="4e7e7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e7e7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e7e7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-117">Not Supported.</span></span>                              |
| <span data-ttu-id="4e7e7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e7e7-118">Application</span></span>                            | <span data-ttu-id="4e7e7-119">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="4e7e7-119">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="4e7e7-120">\* 管理员必须创建 [应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy) 并将其授予用户，授权在该策略中配置的应用程序，以创建或获取一个外部 ID 代表该用户的联机会议， (用户 id 在请求路径) 中指定。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-120">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to create or get an online meeting with external ID on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="4e7e7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e7e7-121">HTTP request</span></span>

<span data-ttu-id="4e7e7-122">使用委派令牌时的请求：</span><span class="sxs-lookup"><span data-stu-id="4e7e7-122">Request when using a delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

<span data-ttu-id="4e7e7-123">使用应用程序令牌时的请求：</span><span class="sxs-lookup"><span data-stu-id="4e7e7-123">Request when using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/createOrGet
```

> <span data-ttu-id="4e7e7-124">**注意：** `userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-124">**Note:** `userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="4e7e7-125">有关详细信息，请参阅[应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-125">See more details in [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e7e7-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e7e7-126">Request headers</span></span>
| <span data-ttu-id="4e7e7-127">名称</span><span class="sxs-lookup"><span data-stu-id="4e7e7-127">Name</span></span>          | <span data-ttu-id="4e7e7-128">说明</span><span class="sxs-lookup"><span data-stu-id="4e7e7-128">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="4e7e7-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e7e7-129">Authorization</span></span> | <span data-ttu-id="4e7e7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4e7e7-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="4e7e7-132">Content-type</span></span>  | <span data-ttu-id="4e7e7-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4e7e7-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e7e7-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e7e7-135">Request body</span></span>
<span data-ttu-id="4e7e7-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e7e7-137">参数</span><span class="sxs-lookup"><span data-stu-id="4e7e7-137">Parameter</span></span>     | <span data-ttu-id="4e7e7-138">类型</span><span class="sxs-lookup"><span data-stu-id="4e7e7-138">Type</span></span>                                                       | <span data-ttu-id="4e7e7-139">说明</span><span class="sxs-lookup"><span data-stu-id="4e7e7-139">Description</span></span>                                                                                          |
| :------------ | :--------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4e7e7-140">chatInfo</span><span class="sxs-lookup"><span data-stu-id="4e7e7-140">chatInfo</span></span>      | [<span data-ttu-id="4e7e7-141">chatInfo</span><span class="sxs-lookup"><span data-stu-id="4e7e7-141">chatInfo</span></span>](../resources/chatinfo.md)                       | <span data-ttu-id="4e7e7-142">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-142">The chat information associated with this online meeting.</span></span>                                            |
| <span data-ttu-id="4e7e7-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4e7e7-143">endDateTime</span></span>   | <span data-ttu-id="4e7e7-144">日期时间</span><span class="sxs-lookup"><span data-stu-id="4e7e7-144">DateTime</span></span>                                                   | <span data-ttu-id="4e7e7-145">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-145">The meeting end time in UTC.</span></span>                                                                         |
| <span data-ttu-id="4e7e7-146">externalId</span><span class="sxs-lookup"><span data-stu-id="4e7e7-146">externalId</span></span>    | <span data-ttu-id="4e7e7-147">String</span><span class="sxs-lookup"><span data-stu-id="4e7e7-147">String</span></span>                                                     | <span data-ttu-id="4e7e7-148">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-148">The external ID.</span></span> <span data-ttu-id="4e7e7-149">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-149">A custom ID.</span></span> <span data-ttu-id="4e7e7-150"> (必需的) </span><span class="sxs-lookup"><span data-stu-id="4e7e7-150">(Required)</span></span>                                                             |
| <span data-ttu-id="4e7e7-151">participants</span><span class="sxs-lookup"><span data-stu-id="4e7e7-151">participants</span></span>  | [<span data-ttu-id="4e7e7-152">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="4e7e7-152">meetingParticipants</span></span>](../resources/meetingparticipants.md) | <span data-ttu-id="4e7e7-153">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-153">The participants associated with the online meeting.</span></span>  <span data-ttu-id="4e7e7-154">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-154">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="4e7e7-155">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e7e7-155">startDateTime</span></span> | <span data-ttu-id="4e7e7-156">日期时间</span><span class="sxs-lookup"><span data-stu-id="4e7e7-156">DateTime</span></span>                                                   | <span data-ttu-id="4e7e7-157">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-157">The meeting start time in UTC.</span></span>                                                                       |
| <span data-ttu-id="4e7e7-158">subject</span><span class="sxs-lookup"><span data-stu-id="4e7e7-158">subject</span></span>       | <span data-ttu-id="4e7e7-159">String</span><span class="sxs-lookup"><span data-stu-id="4e7e7-159">String</span></span>                                                     | <span data-ttu-id="4e7e7-160">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-160">The subject of the online meeting.</span></span>                                                                   |

> <span data-ttu-id="4e7e7-161">**注意：**</span><span class="sxs-lookup"><span data-stu-id="4e7e7-161">**Notes:**</span></span>
>
> - <span data-ttu-id="4e7e7-162">如果未提供 **startDateTime** 和 **EndDateTime** ，则 **StartDateTime** 将默认为当前 dateTime 值， **endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-162">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="4e7e7-163">如果提供了 **startDateTime** ，但 **endDateTime** 不是，则 **endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-163">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="4e7e7-164">如果在没有 **startDateTime** 的情况下提供 **EndDateTime** ，或者 **endDateTime** 早于 **startDateTime** ，则将引发错误。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-164">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>
>
> - <span data-ttu-id="4e7e7-165">当前 **chatInfo** 仅在 beta 中受支持。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-165">Currently **chatInfo** is only supported in beta.</span></span>

## <a name="response"></a><span data-ttu-id="4e7e7-166">响应</span><span class="sxs-lookup"><span data-stu-id="4e7e7-166">Response</span></span>
<span data-ttu-id="4e7e7-167">如果成功，此方法将在 `201 Created` 创建新会议时返回响应代码，或者在 `200 OK` 检索现有会议时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-167">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="4e7e7-168">在这两种情况下，响应正文中都会返回一个 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-168">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e7e7-169">示例</span><span class="sxs-lookup"><span data-stu-id="4e7e7-169">Examples</span></span>

### <a name="example-1-create-or-get-an-online-meeting-with-an-external-id"></a><span data-ttu-id="4e7e7-170">示例1：创建或获取具有外部 ID 的联机会议</span><span class="sxs-lookup"><span data-stu-id="4e7e7-170">Example 1: Create or get an online meeting with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="4e7e7-171">请求</span><span class="sxs-lookup"><span data-stu-id="4e7e7-171">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4e7e7-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e7e7-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json

{
    "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
    "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
    "subject": "Create a meeting with customId provided",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "attendees": [
            {
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                },
                "role": "presenter",
                "upn": "test1@contoso.com"
            }
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="4e7e7-173">C#</span><span class="sxs-lookup"><span data-stu-id="4e7e7-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e7e7-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e7e7-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e7e7-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e7e7-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e7e7-176">Java</span><span class="sxs-lookup"><span data-stu-id="4e7e7-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e7e7-177">响应</span><span class="sxs-lookup"><span data-stu-id="4e7e7-177">Response</span></span>

><span data-ttu-id="4e7e7-178">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-178">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "(redacted)",
    "creationDateTime": "2020-09-11T06:30:18.1909168Z",
    "startDateTime": "2020-09-11T06:30:18.0615989Z",
    "endDateTime": "2020-09-11T07:30:18.0615989Z",
    "joinWebUrl": "(redacted)",
    "subject": "Create a meeting with customId provided",
    "isBroadcast": false,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "(redacted)",
                }
            }
        },
        "attendees": [
            {
                "upn": "test1@contoso.com",
                "role": null,
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
                    }
                }
            }
        ],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    },
    "audioConferencing": {
        "conferenceId": "(redacted)",
        "tollNumber": "+1 206-485-3005",
        "tollFreeNumber": null,
        "dialinUrl": "https://dialin.teams.microsoft.com/0e73a853-1cc2-436c-b18c-9f53e0a97c24?id=(redacted)"
    },
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2",
        "messageId": "0",
        "replyChainMessageId": null
    },
}
```


### <a name="example-2-create-or-get-an-online-meeting-in-a-microsoft-teams-channel-with-an-external-id"></a><span data-ttu-id="4e7e7-179">示例2：在具有外部 ID 的 Microsoft 团队频道中创建或获取联机会议</span><span class="sxs-lookup"><span data-stu-id="4e7e7-179">Example 2: Create or get an online meeting in a Microsoft Teams channel with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="4e7e7-180">请求</span><span class="sxs-lookup"><span data-stu-id="4e7e7-180">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json

{
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2"
    },
    "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
    "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "attendees": [
            {
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                },
                "upn": "test1@contoso.com"
            }
        ]
    },
    "subject": "Create a meeting with customId provided"
}
```

#### <a name="response"></a><span data-ttu-id="4e7e7-181">响应</span><span class="sxs-lookup"><span data-stu-id="4e7e7-181">Response</span></span>

><span data-ttu-id="4e7e7-182">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e7e7-182">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "(redacted)",
    "creationDateTime": "2020-09-11T06:30:18.1909168Z",
    "startDateTime": "2020-09-11T06:30:18.0615989Z",
    "endDateTime": "2020-09-11T07:30:18.0615989Z",
    "joinWebUrl": "(redacted)",
    "subject": "Create a meeting with customId provided",
    "isBroadcast": false,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "(redacted)",
                }
            }
        },
        "attendees": [
            {
                "upn": "test1@contoso.com",
                "role": null,
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
                    }
                }
            }
        ],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    },
    "audioConferencing": {
        "conferenceId": "(redacted)",
        "tollNumber": "+1 206-485-3005",
        "tollFreeNumber": null,
        "dialinUrl": "https://dialin.teams.microsoft.com/0e73a853-1cc2-436c-b18c-9f53e0a97c24?id=(redacted)"
    },
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2",
        "messageId": "1599805818399",
        "replyChainMessageId": null
    },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


