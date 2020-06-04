---
title: 'onlineMeeting: createOrGet'
description: 使用自定义指定的外部 ID 创建联机会议。 如果已存在外部 ID，此 API 将返回具有该外部 ID 的**onlineMeeting**对象。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e59029da6265f2acd7ca515a0bbe4283c788dec7
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556308"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="83903-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="83903-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="83903-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83903-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83903-106">创建具有自定义的指定外部 ID 的[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="83903-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="83903-107">如果已存在外部 ID，此 API 将返回具有该外部 ID 的[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="83903-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="83903-108">**注释**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="83903-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="83903-109">权限</span><span class="sxs-lookup"><span data-stu-id="83903-109">Permissions</span></span>
<span data-ttu-id="83903-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83903-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83903-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="83903-112">Permission type</span></span>                        | <span data-ttu-id="83903-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83903-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83903-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83903-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="83903-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83903-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="83903-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83903-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83903-117">不支持</span><span class="sxs-lookup"><span data-stu-id="83903-117">Not Supported</span></span>                               |
| <span data-ttu-id="83903-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="83903-118">Application</span></span>                            | <span data-ttu-id="83903-119">不支持</span><span class="sxs-lookup"><span data-stu-id="83903-119">Not Supported</span></span>                |

## <a name="http-request"></a><span data-ttu-id="83903-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83903-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

## <a name="request-headers"></a><span data-ttu-id="83903-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="83903-121">Request headers</span></span>
| <span data-ttu-id="83903-122">名称</span><span class="sxs-lookup"><span data-stu-id="83903-122">Name</span></span>          | <span data-ttu-id="83903-123">说明</span><span class="sxs-lookup"><span data-stu-id="83903-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="83903-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="83903-124">Authorization</span></span> | <span data-ttu-id="83903-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83903-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83903-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="83903-127">Content-type</span></span>  | <span data-ttu-id="83903-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="83903-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83903-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="83903-130">Request body</span></span>
<span data-ttu-id="83903-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="83903-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83903-132">参数</span><span class="sxs-lookup"><span data-stu-id="83903-132">Parameter</span></span>        | <span data-ttu-id="83903-133">类型</span><span class="sxs-lookup"><span data-stu-id="83903-133">Type</span></span>                                     |<span data-ttu-id="83903-134">说明</span><span class="sxs-lookup"><span data-stu-id="83903-134">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="83903-135">chatInfo</span><span class="sxs-lookup"><span data-stu-id="83903-135">chatInfo</span></span>         |[<span data-ttu-id="83903-136">chatInfo</span><span class="sxs-lookup"><span data-stu-id="83903-136">chatInfo</span></span>](../resources/chatinfo.md)                   |<span data-ttu-id="83903-137">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="83903-137">The chat information associated with this online meeting.</span></span>|
| <span data-ttu-id="83903-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="83903-138">endDateTime</span></span>      | <span data-ttu-id="83903-139">日期/时间</span><span class="sxs-lookup"><span data-stu-id="83903-139">DateTime</span></span>                                 | <span data-ttu-id="83903-140">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="83903-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="83903-141">externalId</span><span class="sxs-lookup"><span data-stu-id="83903-141">externalId</span></span>       | <span data-ttu-id="83903-142">String</span><span class="sxs-lookup"><span data-stu-id="83903-142">String</span></span>                                   | <span data-ttu-id="83903-143">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="83903-143">The external ID.</span></span> <span data-ttu-id="83903-144">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="83903-144">A custom ID.</span></span> <span data-ttu-id="83903-145">需要</span><span class="sxs-lookup"><span data-stu-id="83903-145">(Required)</span></span> |
| <span data-ttu-id="83903-146">participants</span><span class="sxs-lookup"><span data-stu-id="83903-146">participants</span></span>     | [<span data-ttu-id="83903-147">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="83903-147">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="83903-148">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="83903-148">The participants associated with the online meeting.</span></span>  <span data-ttu-id="83903-149">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="83903-149">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="83903-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="83903-150">startDateTime</span></span>    | <span data-ttu-id="83903-151">日期/时间</span><span class="sxs-lookup"><span data-stu-id="83903-151">DateTime</span></span>                                 | <span data-ttu-id="83903-152">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="83903-152">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="83903-153">subject</span><span class="sxs-lookup"><span data-stu-id="83903-153">subject</span></span>          | <span data-ttu-id="83903-154">String</span><span class="sxs-lookup"><span data-stu-id="83903-154">String</span></span>                                   | <span data-ttu-id="83903-155">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="83903-155">The subject of the online meeting.</span></span> |

><span data-ttu-id="83903-156">**注意：** 如果 `startDateTime` `endDateTime` 未提供，则 `startDateTime` 默认为当前日期/时间值， `endDateTime` 值将等于 startDateTime + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="83903-156">**Note:** If the `startDateTime` and `endDateTime` are not provided, the `startDateTime` will default to the current dateTime value and `endDateTime` value will equal the startDateTime + 1 hour.</span></span> 

><span data-ttu-id="83903-157">如果 `startDateTime` 提供了，但 `endDateTime` 不是，则 `endDateTime` 值将等于 `startDateTime` + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="83903-157">If the `startDateTime` is provided, but `endDateTime` is not, the `endDateTime` value will equal the `startDateTime` + 1 hour.</span></span> 

><span data-ttu-id="83903-158">如果提供的不是 `endDateTime` ， `startDateTime` 或者 `endDateTime` 早于，则会引发错误 `startDateTime` 。</span><span class="sxs-lookup"><span data-stu-id="83903-158">An error will be thrown if the `endDateTime` is provided without the `startDateTime` or if the `endDateTime` is earlier than the `startDateTime`.</span></span>

## <a name="response"></a><span data-ttu-id="83903-159">响应</span><span class="sxs-lookup"><span data-stu-id="83903-159">Response</span></span>
<span data-ttu-id="83903-160">如果成功，此方法将在 `201 Created` 创建新会议时返回响应代码，或者在 `200 OK` 检索现有会议时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="83903-160">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="83903-161">在这两种情况下，响应正文中都会返回一个[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="83903-161">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83903-162">示例</span><span class="sxs-lookup"><span data-stu-id="83903-162">Examples</span></span>

<span data-ttu-id="83903-163">下面的示例演示如何创建或获取具有外部 ID 的联机会议。</span><span class="sxs-lookup"><span data-stu-id="83903-163">The following example shows how to create or get an online meeting with an external ID.</span></span>

### <a name="request"></a><span data-ttu-id="83903-164">请求</span><span class="sxs-lookup"><span data-stu-id="83903-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="83903-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="83903-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json

{
  "chatInfo": {
    "threadId":"19%3A3b52398f3c524556894b776357c1dd79%40thread.skype"
  },
  "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
  "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
  "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "d4a060b5-a8fc-450c-837b-750b2c280000",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd0110000"
        }
      },
      "upn": "test1@contoso.com"
    },
    "attendees": [
      {
        "identity": {
          "user": {
            "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
            "identityProvider": "MSA"
          }
        },
        "upn": "test@contoso.com"
      }
    ]
  },
  "subject":"Create a meeting with customId provided"
}
```
# <a name="c"></a>[<span data-ttu-id="83903-166">C#</span><span class="sxs-lookup"><span data-stu-id="83903-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83903-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83903-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83903-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83903-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="83903-169">响应</span><span class="sxs-lookup"><span data-stu-id="83903-169">Response</span></span>

><span data-ttu-id="83903-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="83903-170">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "creationDateTime": "2020-02-06T01:50:10.7396692+00:00",
  "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
  "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
 "joinWebUrl": "https://devspaces.skype.com/l/meetup-join/19%3ameeting_MWE2Y2U2NGYtMjk4Ni00NjYyLWEyMjItYjk3MGU4YzFh0000%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22d4a060b5-a8fc-450c-837b-750b2c2869b5%22%7d",
  "subject": "Create a meeting with customId provided",
  "participants": {
    "@odata.type": "#microsoft.graph.meetingParticipants",
    "organizer": {
      "@odata.type": "#microsoft.graph.meetingParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "d4a060b5-a8fc-450c-837b-750b2c280000",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd0110000",
          "displayName": "Tyler Stein",
          "identityProvider": "AAD"
        }
      },
      "upn": "test1@contoso.com"
    },
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.meetingParticipantInfo",
        "identity": {
          "@odata.type": "#microsoft.graph.identitySet",
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
            "displayName": "Jasmine Miller",
            "identityProvider": "MSA"
          }
        },
        "upn": "test@contoso.com"
      }
    ],
    "producers": [],
    "contributors": []
  },
  "isBroadcast": false,
  "autoAdmittedUsers": "everyone",
  "capabilities": [],
  "audioConferencing": {
    "@odata.type": "#microsoft.graph.audioConferencing",
    "conferenceId": "804980000",
    "tollNumber": "555-749-0000",
    "dialinUrl": "https://dialin.teams.microsoft.com/8bf6e654-57eb-4b85-aeaf-36c84429b2fe?id=804980000"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_MWE2Y2U2NGYtMjk4Ni00NjYyLWEyMjItYjk3MGU4YzFh0000@thread.v2",
    "messageId": "0"
  },
  "videoTeleconferenceId": "5556440000",
  "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
  "id": "d4a060b5-a8fc-450c-837b-750b2c2869b5_19:meeting_MWE2Y2U2NGYtMjk4Ni00NjYyLWEyMjItYjk3MGU4YzFh0000@thread.v2",
  "@odata.context": "http://localhost/$metadata#onlineMeetings/$entity",
  "outerMeetingAutoAdmittedUsers": null,
  "meetingInfo": null
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
