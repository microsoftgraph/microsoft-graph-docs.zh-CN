---
title: 'onlineMeeting: createOrGet'
description: 使用自定义指定的外部 ID 创建联机会议。 如果已存在外部 ID，此 API 将返回具有该外部 ID 的 **onlineMeeting** 对象。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7ddeccaa3a792c1af67bef3bc80901e1369e8caa
ms.sourcegitcommit: f26428bce3034e206b901e9c747cffcf64b55882
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47651302"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="f2439-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="f2439-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="f2439-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2439-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2439-106">创建具有自定义的指定外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2439-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="f2439-107">如果已存在外部 ID，此 API 将返回具有该外部 ID 的 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2439-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="f2439-108">**注释**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="f2439-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2439-109">权限</span><span class="sxs-lookup"><span data-stu-id="f2439-109">Permissions</span></span>
<span data-ttu-id="f2439-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2439-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2439-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2439-112">Permission type</span></span>                        | <span data-ttu-id="f2439-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2439-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f2439-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2439-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2439-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2439-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="f2439-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2439-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2439-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2439-117">Not supported.</span></span>                               |
| <span data-ttu-id="f2439-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2439-118">Application</span></span>                            | <span data-ttu-id="f2439-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2439-119">Not supported.</span></span>                |

## <a name="http-request"></a><span data-ttu-id="f2439-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2439-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

## <a name="request-headers"></a><span data-ttu-id="f2439-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2439-121">Request headers</span></span>
| <span data-ttu-id="f2439-122">名称</span><span class="sxs-lookup"><span data-stu-id="f2439-122">Name</span></span>          | <span data-ttu-id="f2439-123">说明</span><span class="sxs-lookup"><span data-stu-id="f2439-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f2439-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2439-124">Authorization</span></span> | <span data-ttu-id="f2439-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2439-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2439-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="f2439-127">Content-type</span></span>  | <span data-ttu-id="f2439-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f2439-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2439-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2439-130">Request body</span></span>
<span data-ttu-id="f2439-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f2439-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f2439-132">参数</span><span class="sxs-lookup"><span data-stu-id="f2439-132">Parameter</span></span>        | <span data-ttu-id="f2439-133">类型</span><span class="sxs-lookup"><span data-stu-id="f2439-133">Type</span></span>                                     |<span data-ttu-id="f2439-134">描述</span><span class="sxs-lookup"><span data-stu-id="f2439-134">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="f2439-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f2439-135">endDateTime</span></span>      | <span data-ttu-id="f2439-136">日期时间</span><span class="sxs-lookup"><span data-stu-id="f2439-136">DateTime</span></span>                                 | <span data-ttu-id="f2439-137">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="f2439-137">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="f2439-138">externalId</span><span class="sxs-lookup"><span data-stu-id="f2439-138">externalId</span></span>       | <span data-ttu-id="f2439-139">String</span><span class="sxs-lookup"><span data-stu-id="f2439-139">String</span></span>                                   | <span data-ttu-id="f2439-140">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="f2439-140">The external ID.</span></span> <span data-ttu-id="f2439-141">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="f2439-141">A custom ID.</span></span> <span data-ttu-id="f2439-142"> (必需的) </span><span class="sxs-lookup"><span data-stu-id="f2439-142">(Required)</span></span> |
| <span data-ttu-id="f2439-143">participants</span><span class="sxs-lookup"><span data-stu-id="f2439-143">participants</span></span>     | [<span data-ttu-id="f2439-144">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="f2439-144">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="f2439-145">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="f2439-145">The participants associated with the online meeting.</span></span>  <span data-ttu-id="f2439-146">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="f2439-146">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="f2439-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f2439-147">startDateTime</span></span>    | <span data-ttu-id="f2439-148">日期时间</span><span class="sxs-lookup"><span data-stu-id="f2439-148">DateTime</span></span>                                 | <span data-ttu-id="f2439-149">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="f2439-149">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="f2439-150">subject</span><span class="sxs-lookup"><span data-stu-id="f2439-150">subject</span></span>          | <span data-ttu-id="f2439-151">String</span><span class="sxs-lookup"><span data-stu-id="f2439-151">String</span></span>                                   | <span data-ttu-id="f2439-152">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="f2439-152">The subject of the online meeting.</span></span> |

> <span data-ttu-id="f2439-153">**注意：**</span><span class="sxs-lookup"><span data-stu-id="f2439-153">**Notes:**</span></span>
>
> - <span data-ttu-id="f2439-154">如果未提供 **startDateTime** 和 **EndDateTime** ，则 **StartDateTime** 将默认为当前 dateTime 值， **endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="f2439-154">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="f2439-155">如果提供了 **startDateTime** ，但 **endDateTime** 不是，则 **endDateTime** 值将等于 **startDateTime** + 1 小时。</span><span class="sxs-lookup"><span data-stu-id="f2439-155">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="f2439-156">如果在没有**startDateTime**的情况下提供**EndDateTime** ，或者**endDateTime**早于**startDateTime**，则将引发错误。</span><span class="sxs-lookup"><span data-stu-id="f2439-156">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>

## <a name="response"></a><span data-ttu-id="f2439-157">响应</span><span class="sxs-lookup"><span data-stu-id="f2439-157">Response</span></span>
<span data-ttu-id="f2439-158">如果成功，此方法将在 `201 Created` 创建新会议时返回响应代码，或者在 `200 OK` 检索现有会议时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2439-158">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="f2439-159">在这两种情况下，响应正文中都会返回一个 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2439-159">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2439-160">示例</span><span class="sxs-lookup"><span data-stu-id="f2439-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2439-161">请求</span><span class="sxs-lookup"><span data-stu-id="f2439-161">Request</span></span>

<span data-ttu-id="f2439-162">下面的示例演示如何创建或获取具有外部 ID 的联机会议。</span><span class="sxs-lookup"><span data-stu-id="f2439-162">The following example shows how to create or get an online meeting with an external ID.</span></span>

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

#### <a name="response"></a><span data-ttu-id="f2439-163">响应</span><span class="sxs-lookup"><span data-stu-id="f2439-163">Response</span></span>

><span data-ttu-id="f2439-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f2439-164">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
