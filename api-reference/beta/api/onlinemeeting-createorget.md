---
title: 'onlineMeeting: createOrGet'
description: 使用自定义指定的外部 ID 创建联机会议。 如果已存在外部 ID，此 API 将返回具有该外部 ID 的 **onlineMeeting** 对象。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d99a9ac98fd5fbb4ca5c96904831bb76c93b158c
ms.sourcegitcommit: f26428bce3034e206b901e9c747cffcf64b55882
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47651321"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="14415-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="14415-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="14415-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14415-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14415-106">创建具有自定义的指定外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14415-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="14415-107">如果已存在外部 ID，此 API 将返回具有该外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14415-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="14415-108">**注释**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="14415-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="14415-109">权限</span><span class="sxs-lookup"><span data-stu-id="14415-109">Permissions</span></span>
<span data-ttu-id="14415-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14415-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14415-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="14415-112">Permission type</span></span>                        | <span data-ttu-id="14415-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14415-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14415-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14415-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="14415-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14415-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="14415-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14415-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14415-117">不支持</span><span class="sxs-lookup"><span data-stu-id="14415-117">Not Supported</span></span>                               |
| <span data-ttu-id="14415-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="14415-118">Application</span></span>                            | <span data-ttu-id="14415-119">不支持</span><span class="sxs-lookup"><span data-stu-id="14415-119">Not Supported</span></span>                |

## <a name="http-request"></a><span data-ttu-id="14415-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14415-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

## <a name="request-headers"></a><span data-ttu-id="14415-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="14415-121">Request headers</span></span>
| <span data-ttu-id="14415-122">名称</span><span class="sxs-lookup"><span data-stu-id="14415-122">Name</span></span>          | <span data-ttu-id="14415-123">说明</span><span class="sxs-lookup"><span data-stu-id="14415-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="14415-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14415-124">Authorization</span></span> | <span data-ttu-id="14415-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14415-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14415-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="14415-127">Content-type</span></span>  | <span data-ttu-id="14415-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="14415-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14415-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="14415-130">Request body</span></span>
<span data-ttu-id="14415-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="14415-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="14415-132">参数</span><span class="sxs-lookup"><span data-stu-id="14415-132">Parameter</span></span>        | <span data-ttu-id="14415-133">类型</span><span class="sxs-lookup"><span data-stu-id="14415-133">Type</span></span>                                     |<span data-ttu-id="14415-134">描述</span><span class="sxs-lookup"><span data-stu-id="14415-134">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="14415-135">chatInfo</span><span class="sxs-lookup"><span data-stu-id="14415-135">chatInfo</span></span>         |[<span data-ttu-id="14415-136">chatInfo</span><span class="sxs-lookup"><span data-stu-id="14415-136">chatInfo</span></span>](../resources/chatinfo.md)                   |<span data-ttu-id="14415-137">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="14415-137">The chat information associated with this online meeting.</span></span>|
| <span data-ttu-id="14415-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="14415-138">endDateTime</span></span>      | <span data-ttu-id="14415-139">日期时间</span><span class="sxs-lookup"><span data-stu-id="14415-139">DateTime</span></span>                                 | <span data-ttu-id="14415-140">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="14415-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="14415-141">externalId</span><span class="sxs-lookup"><span data-stu-id="14415-141">externalId</span></span>       | <span data-ttu-id="14415-142">String</span><span class="sxs-lookup"><span data-stu-id="14415-142">String</span></span>                                   | <span data-ttu-id="14415-143">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="14415-143">The external ID.</span></span> <span data-ttu-id="14415-144">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="14415-144">A custom ID.</span></span> <span data-ttu-id="14415-145"> (必需的) </span><span class="sxs-lookup"><span data-stu-id="14415-145">(Required)</span></span> |
| <span data-ttu-id="14415-146">participants</span><span class="sxs-lookup"><span data-stu-id="14415-146">participants</span></span>     | [<span data-ttu-id="14415-147">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="14415-147">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="14415-148">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="14415-148">The participants associated with the online meeting.</span></span>  <span data-ttu-id="14415-149">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="14415-149">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="14415-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="14415-150">startDateTime</span></span>    | <span data-ttu-id="14415-151">日期时间</span><span class="sxs-lookup"><span data-stu-id="14415-151">DateTime</span></span>                                 | <span data-ttu-id="14415-152">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="14415-152">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="14415-153">subject</span><span class="sxs-lookup"><span data-stu-id="14415-153">subject</span></span>          | <span data-ttu-id="14415-154">String</span><span class="sxs-lookup"><span data-stu-id="14415-154">String</span></span>                                   | <span data-ttu-id="14415-155">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="14415-155">The subject of the online meeting.</span></span> |

> <span data-ttu-id="14415-156">**注意：**</span><span class="sxs-lookup"><span data-stu-id="14415-156">**Notes:**</span></span>
>
> - <span data-ttu-id="14415-157">如果未提供 **startDateTime** 和 **EndDateTime** ，则 **StartDateTime** 将默认为当前 dateTime 值， **endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="14415-157">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="14415-158">如果提供了 **startDateTime** ，但 **endDateTime** 不是，则 **endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="14415-158">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="14415-159">如果在没有**startDateTime**的情况下提供**EndDateTime** ，或者**endDateTime**早于**startDateTime**，则将引发错误。</span><span class="sxs-lookup"><span data-stu-id="14415-159">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>
>
> - <span data-ttu-id="14415-160">当前 **chatInfo** 仅在 beta 中受支持。</span><span class="sxs-lookup"><span data-stu-id="14415-160">Currently **chatInfo** is only supported in beta.</span></span>

## <a name="response"></a><span data-ttu-id="14415-161">响应</span><span class="sxs-lookup"><span data-stu-id="14415-161">Response</span></span>
<span data-ttu-id="14415-162">如果成功，此方法将在 `201 Created` 创建新会议时返回响应代码，或者在 `200 OK` 检索现有会议时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="14415-162">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="14415-163">在这两种情况下，响应正文中都会返回一个 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14415-163">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14415-164">示例</span><span class="sxs-lookup"><span data-stu-id="14415-164">Examples</span></span>

### <a name="example-1-create-or-get-an-online-meeting-with-an-external-id"></a><span data-ttu-id="14415-165">示例1：创建或获取具有外部 ID 的联机会议</span><span class="sxs-lookup"><span data-stu-id="14415-165">Example 1: Create or get an online meeting with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="14415-166">请求</span><span class="sxs-lookup"><span data-stu-id="14415-166">Request</span></span>

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
                "upn": "test1@contoso.com"
            }
        ]
    }
}
```

#### <a name="response"></a><span data-ttu-id="14415-167">响应</span><span class="sxs-lookup"><span data-stu-id="14415-167">Response</span></span>

><span data-ttu-id="14415-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="14415-168">**Note:** The response object shown here might be shortened for readability.</span></span> 

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


### <a name="example-2-create-or-get-an-online-meeting-in-a-microsoft-teams-channel-with-an-external-id"></a><span data-ttu-id="14415-169">示例2：在具有外部 ID 的 Microsoft 团队频道中创建或获取联机会议</span><span class="sxs-lookup"><span data-stu-id="14415-169">Example 2: Create or get an online meeting in a Microsoft Teams channel with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="14415-170">请求</span><span class="sxs-lookup"><span data-stu-id="14415-170">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="14415-171">响应</span><span class="sxs-lookup"><span data-stu-id="14415-171">Response</span></span>

><span data-ttu-id="14415-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="14415-172">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
