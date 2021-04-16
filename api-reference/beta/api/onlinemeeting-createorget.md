---
title: onlineMeeting：createOrGet
description: 使用自定义指定的外部 ID 创建联机会议。 如果外部 ID 已存在，此 API 将返回具有该外部 ID 的 onlineMeeting 对象。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3256e99798de12d4a79da37888551d562ed6027e
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869860"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="07623-104">onlineMeeting：createOrGet</span><span class="sxs-lookup"><span data-stu-id="07623-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="07623-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07623-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07623-106">创建具有自定义指定外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07623-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="07623-107">如果外部 ID 已存在，此 API 将返回具有该外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07623-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="07623-108">**注释**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="07623-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="07623-109">权限</span><span class="sxs-lookup"><span data-stu-id="07623-109">Permissions</span></span>
<span data-ttu-id="07623-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07623-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07623-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="07623-112">Permission type</span></span>                        | <span data-ttu-id="07623-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07623-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="07623-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07623-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="07623-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07623-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="07623-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07623-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07623-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="07623-117">Not Supported.</span></span>                              |
| <span data-ttu-id="07623-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="07623-118">Application</span></span>                            | <span data-ttu-id="07623-119">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="07623-119">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="07623-120">\*管理员必须创建应用程序访问[](/graph/cloud-communication-online-meeting-application-access-policy)策略，并授予用户该策略，授权策略中配置的应用代表该用户在请求路径) 中指定的 (用户 ID 创建或获取具有外部 ID 的联机会议。</span><span class="sxs-lookup"><span data-stu-id="07623-120">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to create or get an online meeting with external ID on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="07623-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07623-121">HTTP request</span></span>
<span data-ttu-id="07623-122">使用委派 **令牌调用 createOrGet** API：</span><span class="sxs-lookup"><span data-stu-id="07623-122">To call **createOrGet** API with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

<span data-ttu-id="07623-123">使用应用程序 **令牌调用 createOrGet** API：</span><span class="sxs-lookup"><span data-stu-id="07623-123">To call **createOrGet** API with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/createOrGet
```

> [!NOTE]
> <span data-ttu-id="07623-124">`userId`是 Azure 用户管理门户中的[用户的对象 ID。](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="07623-124">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="07623-125">有关详细信息，请参阅[应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。</span><span class="sxs-lookup"><span data-stu-id="07623-125">See more details in [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>

## <a name="request-headers"></a><span data-ttu-id="07623-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="07623-126">Request headers</span></span>
| <span data-ttu-id="07623-127">名称</span><span class="sxs-lookup"><span data-stu-id="07623-127">Name</span></span>          | <span data-ttu-id="07623-128">说明</span><span class="sxs-lookup"><span data-stu-id="07623-128">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="07623-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="07623-129">Authorization</span></span> | <span data-ttu-id="07623-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07623-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="07623-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="07623-132">Content-type</span></span>  | <span data-ttu-id="07623-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="07623-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07623-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="07623-135">Request body</span></span>
<span data-ttu-id="07623-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="07623-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="07623-137">参数</span><span class="sxs-lookup"><span data-stu-id="07623-137">Parameter</span></span>     | <span data-ttu-id="07623-138">类型</span><span class="sxs-lookup"><span data-stu-id="07623-138">Type</span></span>                                                       | <span data-ttu-id="07623-139">说明</span><span class="sxs-lookup"><span data-stu-id="07623-139">Description</span></span>                                                                                          |
| :------------ | :--------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="07623-140">chatInfo</span><span class="sxs-lookup"><span data-stu-id="07623-140">chatInfo</span></span>      | [<span data-ttu-id="07623-141">chatInfo</span><span class="sxs-lookup"><span data-stu-id="07623-141">chatInfo</span></span>](../resources/chatinfo.md)                       | <span data-ttu-id="07623-142">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="07623-142">The chat information associated with this online meeting.</span></span>                                            |
| <span data-ttu-id="07623-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="07623-143">endDateTime</span></span>   | <span data-ttu-id="07623-144">日期时间</span><span class="sxs-lookup"><span data-stu-id="07623-144">DateTime</span></span>                                                   | <span data-ttu-id="07623-145">会议结束时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="07623-145">The meeting end time in UTC.</span></span>                                                                         |
| <span data-ttu-id="07623-146">externalId</span><span class="sxs-lookup"><span data-stu-id="07623-146">externalId</span></span>    | <span data-ttu-id="07623-147">String</span><span class="sxs-lookup"><span data-stu-id="07623-147">String</span></span>                                                     | <span data-ttu-id="07623-148">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="07623-148">The external ID.</span></span> <span data-ttu-id="07623-149">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="07623-149">A custom ID.</span></span> <span data-ttu-id="07623-150"> (必需) </span><span class="sxs-lookup"><span data-stu-id="07623-150">(Required)</span></span>                                                             |
| <span data-ttu-id="07623-151">participants</span><span class="sxs-lookup"><span data-stu-id="07623-151">participants</span></span>  | [<span data-ttu-id="07623-152">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="07623-152">meetingParticipants</span></span>](../resources/meetingparticipants.md) | <span data-ttu-id="07623-153">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="07623-153">The participants associated with the online meeting.</span></span>  <span data-ttu-id="07623-154">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="07623-154">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="07623-155">startDateTime</span><span class="sxs-lookup"><span data-stu-id="07623-155">startDateTime</span></span> | <span data-ttu-id="07623-156">日期时间</span><span class="sxs-lookup"><span data-stu-id="07623-156">DateTime</span></span>                                                   | <span data-ttu-id="07623-157">会议开始时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="07623-157">The meeting start time in UTC.</span></span>                                                                       |
| <span data-ttu-id="07623-158">subject</span><span class="sxs-lookup"><span data-stu-id="07623-158">subject</span></span>       | <span data-ttu-id="07623-159">String</span><span class="sxs-lookup"><span data-stu-id="07623-159">String</span></span>                                                     | <span data-ttu-id="07623-160">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="07623-160">The subject of the online meeting.</span></span>                                                                   |

> <span data-ttu-id="07623-161">**注意：**</span><span class="sxs-lookup"><span data-stu-id="07623-161">**Notes:**</span></span>
>
> - <span data-ttu-id="07623-162">如果未 **提供 startDateTime** 和 **endDateTime，startDateTime** 将默认为当前 dateTime 值 **，endDateTime** 值将等于 **startDateTime** + 1 小时。 </span><span class="sxs-lookup"><span data-stu-id="07623-162">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="07623-163">如果 **提供了 startDateTime，** 但 **endDateTime** 未提供， **则 endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="07623-163">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="07623-164">如果没有 **startDateTime 提供 endDateTime，** 或者 **endDateTime** 早于 **startDateTime**，将引发错误。</span><span class="sxs-lookup"><span data-stu-id="07623-164">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>
>
> - <span data-ttu-id="07623-165">目前 **，仅测试版支持 chatInfo。**</span><span class="sxs-lookup"><span data-stu-id="07623-165">Currently **chatInfo** is only supported in beta.</span></span>

## <a name="response"></a><span data-ttu-id="07623-166">响应</span><span class="sxs-lookup"><span data-stu-id="07623-166">Response</span></span>
<span data-ttu-id="07623-167">如果成功，此方法在新建会议时返回 响应代码，如果检索到现有会议，则返回 `201 Created` `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="07623-167">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="07623-168">在这两种情况下，在响应正文中返回 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07623-168">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07623-169">示例</span><span class="sxs-lookup"><span data-stu-id="07623-169">Examples</span></span>

### <a name="example-1-create-or-get-an-online-meeting-with-an-external-id"></a><span data-ttu-id="07623-170">示例 1：创建或获取具有外部 ID 的联机会议</span><span class="sxs-lookup"><span data-stu-id="07623-170">Example 1: Create or get an online meeting with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="07623-171">请求</span><span class="sxs-lookup"><span data-stu-id="07623-171">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="07623-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="07623-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting-1"
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
# <a name="c"></a>[<span data-ttu-id="07623-173">C#</span><span class="sxs-lookup"><span data-stu-id="07623-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07623-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07623-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07623-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07623-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07623-176">Java</span><span class="sxs-lookup"><span data-stu-id="07623-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="07623-177">响应</span><span class="sxs-lookup"><span data-stu-id="07623-177">Response</span></span>

><span data-ttu-id="07623-178">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="07623-178">**Note:** The response object shown here might be shortened for readability.</span></span> 

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


### <a name="example-2-create-or-get-an-online-meeting-in-a-microsoft-teams-channel-with-an-external-id"></a><span data-ttu-id="07623-179">示例 2：使用外部 ID 在 Microsoft Teams 频道创建或获取联机会议</span><span class="sxs-lookup"><span data-stu-id="07623-179">Example 2: Create or get an online meeting in a Microsoft Teams channel with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="07623-180">请求</span><span class="sxs-lookup"><span data-stu-id="07623-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="07623-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="07623-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting-2"
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
# <a name="c"></a>[<span data-ttu-id="07623-182">C#</span><span class="sxs-lookup"><span data-stu-id="07623-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07623-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07623-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07623-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07623-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07623-185">Java</span><span class="sxs-lookup"><span data-stu-id="07623-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="07623-186">响应</span><span class="sxs-lookup"><span data-stu-id="07623-186">Response</span></span>

><span data-ttu-id="07623-187">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="07623-187">**Note:** The response object shown here might be shortened for readability.</span></span> 

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


