---
title: onlineMeeting：createOrGet
description: 使用自定义指定的外部 ID 创建联机会议。 如果外部 ID 已存在，此 API 将返回具有该外部 ID 的 **onlineMeeting** 对象。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 962ed5d23fa8c1e615846c02e376b1a9ad0155fd
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869881"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="e7437-104">onlineMeeting：createOrGet</span><span class="sxs-lookup"><span data-stu-id="e7437-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="e7437-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7437-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7437-106">创建具有自定义指定外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7437-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="e7437-107">如果外部 ID 已存在，此 API 将返回具有该外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7437-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="e7437-108">**注释**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="e7437-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7437-109">权限</span><span class="sxs-lookup"><span data-stu-id="e7437-109">Permissions</span></span>
<span data-ttu-id="e7437-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7437-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7437-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7437-112">Permission type</span></span>                        | <span data-ttu-id="e7437-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7437-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e7437-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7437-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7437-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7437-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="e7437-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7437-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7437-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7437-117">Not supported.</span></span>                               |
| <span data-ttu-id="e7437-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7437-118">Application</span></span>                            | <span data-ttu-id="e7437-119">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="e7437-119">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="e7437-120">\*管理员必须创建应用程序访问[](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md)策略，并授予用户该策略，授权策略中配置的应用代表该用户在请求路径) 中指定的 (用户 ID 创建或获取具有外部 ID 的联机会议。</span><span class="sxs-lookup"><span data-stu-id="e7437-120">\* Administrators must create an [application access policy](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) and grant it to a user, authorizing the app configured in the policy to create or get an online meeting with external ID on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="e7437-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7437-121">HTTP request</span></span>
<span data-ttu-id="e7437-122">使用委派 **令牌调用 createOrGet** API：</span><span class="sxs-lookup"><span data-stu-id="e7437-122">To call **createOrGet** API with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

<span data-ttu-id="e7437-123">使用应用程序 **令牌调用 createOrGet** API：</span><span class="sxs-lookup"><span data-stu-id="e7437-123">To call **createOrGet** API with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/createOrGet
```

> [!NOTE]
> <span data-ttu-id="e7437-124">`userId`是 Azure 用户管理门户中的[用户的对象 ID。](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="e7437-124">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="e7437-125">有关详细信息，请参阅[应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。</span><span class="sxs-lookup"><span data-stu-id="e7437-125">See more details in [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7437-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7437-126">Request headers</span></span>
| <span data-ttu-id="e7437-127">名称</span><span class="sxs-lookup"><span data-stu-id="e7437-127">Name</span></span>          | <span data-ttu-id="e7437-128">说明</span><span class="sxs-lookup"><span data-stu-id="e7437-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e7437-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7437-129">Authorization</span></span> | <span data-ttu-id="e7437-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7437-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7437-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="e7437-132">Content-type</span></span>  | <span data-ttu-id="e7437-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e7437-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7437-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7437-135">Request body</span></span>
<span data-ttu-id="e7437-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e7437-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e7437-137">参数</span><span class="sxs-lookup"><span data-stu-id="e7437-137">Parameter</span></span>        | <span data-ttu-id="e7437-138">类型</span><span class="sxs-lookup"><span data-stu-id="e7437-138">Type</span></span>                                     |<span data-ttu-id="e7437-139">说明</span><span class="sxs-lookup"><span data-stu-id="e7437-139">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="e7437-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e7437-140">endDateTime</span></span>      | <span data-ttu-id="e7437-141">日期时间</span><span class="sxs-lookup"><span data-stu-id="e7437-141">DateTime</span></span>                                 | <span data-ttu-id="e7437-142">会议结束时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="e7437-142">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="e7437-143">externalId</span><span class="sxs-lookup"><span data-stu-id="e7437-143">externalId</span></span>       | <span data-ttu-id="e7437-144">String</span><span class="sxs-lookup"><span data-stu-id="e7437-144">String</span></span>                                   | <span data-ttu-id="e7437-145">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="e7437-145">The external ID.</span></span> <span data-ttu-id="e7437-146">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="e7437-146">A custom ID.</span></span> <span data-ttu-id="e7437-147"> (必需) </span><span class="sxs-lookup"><span data-stu-id="e7437-147">(Required)</span></span> |
| <span data-ttu-id="e7437-148">participants</span><span class="sxs-lookup"><span data-stu-id="e7437-148">participants</span></span>     | [<span data-ttu-id="e7437-149">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="e7437-149">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="e7437-150">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="e7437-150">The participants associated with the online meeting.</span></span>  <span data-ttu-id="e7437-151">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="e7437-151">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="e7437-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e7437-152">startDateTime</span></span>    | <span data-ttu-id="e7437-153">日期时间</span><span class="sxs-lookup"><span data-stu-id="e7437-153">DateTime</span></span>                                 | <span data-ttu-id="e7437-154">会议开始时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="e7437-154">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="e7437-155">subject</span><span class="sxs-lookup"><span data-stu-id="e7437-155">subject</span></span>          | <span data-ttu-id="e7437-156">String</span><span class="sxs-lookup"><span data-stu-id="e7437-156">String</span></span>                                   | <span data-ttu-id="e7437-157">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="e7437-157">The subject of the online meeting.</span></span> |

> <span data-ttu-id="e7437-158">**注意：**</span><span class="sxs-lookup"><span data-stu-id="e7437-158">**Notes:**</span></span>
>
> - <span data-ttu-id="e7437-159">如果未 **提供 startDateTime** 和 **endDateTime，startDateTime** 将默认为当前 dateTime 值 **，endDateTime** 值将等于 **startDateTime** + 1 小时。 </span><span class="sxs-lookup"><span data-stu-id="e7437-159">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="e7437-160">如果 **提供了 startDateTime，** 但 **endDateTime** 未提供， **则 endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="e7437-160">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="e7437-161">如果没有 **startDateTime 提供 endDateTime，** 或者 **endDateTime** 早于 **startDateTime**，将引发错误。</span><span class="sxs-lookup"><span data-stu-id="e7437-161">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>

## <a name="response"></a><span data-ttu-id="e7437-162">响应</span><span class="sxs-lookup"><span data-stu-id="e7437-162">Response</span></span>
<span data-ttu-id="e7437-163">如果成功，此方法在新建会议时返回 响应代码，如果检索到现有会议，则返回 `201 Created` `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e7437-163">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="e7437-164">在这两种情况下，在响应正文中返回 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7437-164">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7437-165">示例</span><span class="sxs-lookup"><span data-stu-id="e7437-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7437-166">请求</span><span class="sxs-lookup"><span data-stu-id="e7437-166">Request</span></span>

<span data-ttu-id="e7437-167">以下示例演示如何使用外部 ID 创建或获取联机会议。</span><span class="sxs-lookup"><span data-stu-id="e7437-167">The following example shows how to create or get an online meeting with an external ID.</span></span>


# <a name="http"></a>[<span data-ttu-id="e7437-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7437-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/onlineMeetings/createOrGet
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
                "upn": "test1@contoso.com"
            }
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="e7437-169">C#</span><span class="sxs-lookup"><span data-stu-id="e7437-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7437-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7437-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7437-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7437-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7437-172">Java</span><span class="sxs-lookup"><span data-stu-id="e7437-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7437-173">响应</span><span class="sxs-lookup"><span data-stu-id="e7437-173">Response</span></span>

><span data-ttu-id="e7437-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e7437-174">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

