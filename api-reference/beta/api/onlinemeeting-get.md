---
title: 获取 onlineMeeting
description: 检索 onlineMeeting 对象的属性和关系。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ba5a1a874431b2cd543ac35057c29127896e1f52
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896674"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="b4171-103">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b4171-103">Get onlineMeeting</span></span>

<span data-ttu-id="b4171-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4171-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4171-105">检索 [onlineMeeting 对象的属性和](../resources/onlinemeeting.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b4171-105">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="b4171-106">例如，你能够：</span><span class="sxs-lookup"><span data-stu-id="b4171-106">For example, you can:</span></span>
- <span data-ttu-id="b4171-107">使用[VideoTeleconferenceId、](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid)[会议 ID](#example-2-retrieve-an-online-meeting-by-meeting-id)或[JoinWebURL](#example-3-retrieve-an-online-meeting-by-joinweburl)获取 onlineMeeting 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b4171-107">Get details of an onlineMeeting using [VideoTeleconferenceId](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid), [meeting ID](#example-2-retrieve-an-online-meeting-by-meeting-id), or [JoinWebURL](#example-3-retrieve-an-online-meeting-by-joinweburl).</span></span>
- <span data-ttu-id="b4171-108">使用 `/attendeeReport` 路径获取实时事件的与会者报告，如示例 [4 所示](#example-4-retrieve-the-attendee-report-of-a-live-event)。</span><span class="sxs-lookup"><span data-stu-id="b4171-108">Use the `/attendeeReport` path to get an attendee report of a live event, as shown in [example 4](#example-4-retrieve-the-attendee-report-of-a-live-event).</span></span>
- <span data-ttu-id="b4171-109">使用 `/recording` 和 `/alternativeRecording` 路径获取实时事件的录制，如示例 [5 所示](#example-5-retrieve-the-recording-of-a-live-event)。</span><span class="sxs-lookup"><span data-stu-id="b4171-109">Use the `/recording` and `/alternativeRecording` paths to get the recordings of a live event, as shown in [example 5](#example-5-retrieve-the-recording-of-a-live-event).</span></span>
- <span data-ttu-id="b4171-110">使用 `/meetingAttendanceReport` 路径获取计划会议的会议出席报告，如示例 [6 所示](#example-6-retrieve-the-attendance-report-of-a-meeting)。</span><span class="sxs-lookup"><span data-stu-id="b4171-110">Use the `/meetingAttendanceReport` path to get the attendance report for a scheduled meeting, as shown in [example 6](#example-6-retrieve-the-attendance-report-of-a-meeting).</span></span>

> [!NOTE]
>- <span data-ttu-id="b4171-111">会议与会者报告可用于实时事件外的会议，并且仅在会议结束后可用。</span><span class="sxs-lookup"><span data-stu-id="b4171-111">Meeting attendance reports are available for meetings other than live events, and are only available when the meeting has concluded.</span></span>
>- <span data-ttu-id="b4171-112">只有会议组织者可以访问会议出席报告。</span><span class="sxs-lookup"><span data-stu-id="b4171-112">Only the meeting organizer can access meeting attendance reports.</span></span>
>- <span data-ttu-id="b4171-113">录制和与会者报告仅适用于实时事件，并且仅在实时事件结束时可用。</span><span class="sxs-lookup"><span data-stu-id="b4171-113">Recordings and attendee reports are only available for live events, and are only available when the live event has concluded.</span></span>
>- <span data-ttu-id="b4171-114">只有实时事件组织者可以访问与会者报告和录制。</span><span class="sxs-lookup"><span data-stu-id="b4171-114">Only the live event organizer can access attendee reports and recordings.</span></span>
>- <span data-ttu-id="b4171-115">实时事件参与者报告的下载链接和录制将在 60 秒后过期。</span><span class="sxs-lookup"><span data-stu-id="b4171-115">The download links for the live event attendee report and recordings expire in 60 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4171-116">权限</span><span class="sxs-lookup"><span data-stu-id="b4171-116">Permissions</span></span>

<span data-ttu-id="b4171-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4171-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4171-119">Permission type</span></span>                        | <span data-ttu-id="b4171-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4171-120">Permissions (from least to most privileged)</span></span>           |
| :------------------------------------- | :---------------------------------------------------- |
| <span data-ttu-id="b4171-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4171-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4171-122">OnlineMeetings.Read、OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4171-122">OnlineMeetings.Read, OnlineMeetings.ReadWrite</span></span>         |
| <span data-ttu-id="b4171-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4171-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4171-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4171-124">Not Supported.</span></span>                                        |
| <span data-ttu-id="b4171-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4171-125">Application</span></span>                            | <span data-ttu-id="b4171-126">OnlineMeetings.Read.All、OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="b4171-126">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All\*</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="b4171-127">\*管理员必须创建应用程序访问[](/graph/cloud-communication-online-meeting-application-access-policy)策略并授予用户，授权策略中配置的应用代表该用户检索联机会议 (请求路径) 中指定的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="b4171-127">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to retrieve an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="b4171-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4171-128">HTTP request</span></span>

<span data-ttu-id="b4171-129">若要使用具有委派权限的应用权限的会议 ID 获取 onlineMeeting：</span><span class="sxs-lookup"><span data-stu-id="b4171-129">To get an onlineMeeting using meeting ID with delegated and app permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}
GET /users/{userId}/onlineMeetings/{meetingId}
```

<span data-ttu-id="b4171-130">若要使用具有应用权限 **的 videoTeleconferenceId** 获取 onlineMeeting：</span><span class="sxs-lookup"><span data-stu-id="b4171-130">To get an onlineMeeting using **videoTeleconferenceId** with app permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{videoTeleconferenceId}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{videoTeleconferenceId}'
```

<span data-ttu-id="b4171-131">若要使用具有委派权限和应用权限 **的 joinWebUrl** 获取 onlineMeeting：</span><span class="sxs-lookup"><span data-stu-id="b4171-131">To get an onlineMeeting using **joinWebUrl** with delegated and app permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings?$filter=JoinWebUrl%20eq%20'{joinWebUrl}'
GET /users/{userId}/onlineMeetings?$filter=JoinWebUrl%20eq%20'{joinWebUrl}'
```

<span data-ttu-id="b4171-132">若要获取具有委派和应用权限的活动参与者报告，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b4171-132">To get the attendee report of a live event with delegated and app permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/attendeeReport
GET /users/{userId}/onlineMeetings/{meetingId}/attendeeReport
```

<span data-ttu-id="b4171-133">若要获取具有委派权限的应用权限的直播活动的录制，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b4171-133">To get the recordings of a live event with delegated and app permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/recording
GET /me/onlineMeetings/{meetingId}/alternativeRecording
GET /users/{userId}/onlineMeetings/{meetingId}/recording
GET /users/{userId}/onlineMeetings/{meetingId}/alternativeRecording
```

<span data-ttu-id="b4171-134">若要获取具有委派权限的会议的与会者报告，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b4171-134">To get the attendance report of a meeting with delegated permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/meetingAttendanceReport
```

> [!NOTE]
>- <span data-ttu-id="b4171-135">路径 `/app` 已弃用。</span><span class="sxs-lookup"><span data-stu-id="b4171-135">The `/app` path is deprecated.</span></span> <span data-ttu-id="b4171-136">今后，请使用路径 `/communications`。</span><span class="sxs-lookup"><span data-stu-id="b4171-136">Going forward, use the `/communications` path.</span></span>
>- <span data-ttu-id="b4171-137">`userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="b4171-137">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="b4171-138">有关详细信息，请参阅应用程序 [访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。</span><span class="sxs-lookup"><span data-stu-id="b4171-138">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
>- <span data-ttu-id="b4171-139">`meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**</span><span class="sxs-lookup"><span data-stu-id="b4171-139">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>
> - <span data-ttu-id="b4171-140">**videoTeleconferenceId** 为 Cloud-Video-Interop 许可用户生成，可在 [onlineMeeting](../resources/onlinemeeting.md) 对象中找到。</span><span class="sxs-lookup"><span data-stu-id="b4171-140">**videoTeleconferenceId** is generated for Cloud-Video-Interop licensed users and can be found in an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="b4171-141">有关更多详细信息 [，请参阅 VTC](/microsoftteams/cloud-video-interop-for-teams-set-up) 会议 ID。</span><span class="sxs-lookup"><span data-stu-id="b4171-141">Refer to [VTC conference id](/microsoftteams/cloud-video-interop-for-teams-set-up) for more details.</span></span>
>- <span data-ttu-id="b4171-142">`joinWebUrl` 必须经过 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="b4171-142">`joinWebUrl` must be URL encoded.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="b4171-143">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b4171-143">Optional query parameters</span></span>
<span data-ttu-id="b4171-144">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4171-144">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4171-145">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4171-145">Request headers</span></span>
| <span data-ttu-id="b4171-146">名称</span><span class="sxs-lookup"><span data-stu-id="b4171-146">Name</span></span>            | <span data-ttu-id="b4171-147">说明</span><span class="sxs-lookup"><span data-stu-id="b4171-147">Description</span></span>               |
| :-------------- | :------------------------ |
| <span data-ttu-id="b4171-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4171-148">Authorization</span></span>   | <span data-ttu-id="b4171-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4171-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4171-151">Accept-Language</span><span class="sxs-lookup"><span data-stu-id="b4171-151">Accept-Language</span></span> | <span data-ttu-id="b4171-152">语言。</span><span class="sxs-lookup"><span data-stu-id="b4171-152">Language.</span></span> <span data-ttu-id="b4171-153">可选。</span><span class="sxs-lookup"><span data-stu-id="b4171-153">Optional.</span></span>       |

<span data-ttu-id="b4171-154">如果请求包含 `Accept-Language` HTTP 标头，`joinInformation` 的 `content` 将采用 `Accept-Language` 标头中指定的语言和区域设置变量中。</span><span class="sxs-lookup"><span data-stu-id="b4171-154">If the request contains an `Accept-Language` HTTP header, the `content` of `joinInformation` will be in the language and locale variant specified in the `Accept-Language` header.</span></span> <span data-ttu-id="b4171-155">默认内容将为英语。</span><span class="sxs-lookup"><span data-stu-id="b4171-155">The default content will be in English.</span></span>

## <a name="request-body"></a><span data-ttu-id="b4171-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4171-156">Request body</span></span>
<span data-ttu-id="b4171-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4171-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4171-158">响应</span><span class="sxs-lookup"><span data-stu-id="b4171-158">Response</span></span>
<span data-ttu-id="b4171-159">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b4171-159">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="b4171-160">方法还包括以下项之一：</span><span class="sxs-lookup"><span data-stu-id="b4171-160">The method also includes one of the following:</span></span>

- <span data-ttu-id="b4171-161">如果根据会议 **ID、videoTeleconferenceId** 或 **joinWebUrl** 获取联机会议，此方法还会在响应正文中返回 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4171-161">If you're getting an online meeting based on meeting ID, **videoTeleconferenceId** or **joinWebUrl**, this method also returns an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>
- <span data-ttu-id="b4171-162">如果你要获取实时联机会议的与会者报告或录制，此方法还会分别返回一个标头，指示与会者报告或录制 `Location` 的 URI。</span><span class="sxs-lookup"><span data-stu-id="b4171-162">If you're getting the attendee report or recording of a live online meeting, this method also returns a `Location` header that indicates the URI to the attendee report or recording, respectively.</span></span>

## <a name="examples"></a><span data-ttu-id="b4171-163">示例</span><span class="sxs-lookup"><span data-stu-id="b4171-163">Examples</span></span>

> [!NOTE]
> <span data-ttu-id="b4171-164">为了可读性，已缩短以下示例的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4171-164">The response objects of the following examples have been shortened for readability.</span></span> <span data-ttu-id="b4171-165">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4171-165">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-retrieve-an-online-meeting-by-videoteleconferenceid"></a><span data-ttu-id="b4171-166">示例 1：通过 VideoTeleconferenceId 检索联机会议</span><span class="sxs-lookup"><span data-stu-id="b4171-166">Example 1: Retrieve an online meeting by VideoTeleconferenceId</span></span>

#### <a name="request"></a><span data-ttu-id="b4171-167">请求</span><span class="sxs-lookup"><span data-stu-id="b4171-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b4171-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4171-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["123456789"],
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[<span data-ttu-id="b4171-169">C#</span><span class="sxs-lookup"><span data-stu-id="b4171-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4171-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4171-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4171-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4171-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4171-172">Java</span><span class="sxs-lookup"><span data-stu-id="b4171-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b4171-173">响应</span><span class="sxs-lookup"><span data-stu-id="b4171-173">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "55525634478",
    "tollFreeNumber": "55566390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "participants": {
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
            "displayName": "Tyler Stein"
          }
        },
        "upn": "upn-value",
        "role": "attendee"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
          "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
          "displayName": "Jasmine Miller"
        }
      },
      "upn": "upn-value",
      "role": "presenter"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789",
  "lobbyBypassSettings": {
    "scope": "everyone",
    "isDialInBypassEnabled": true
  },
  "isEntryExitAnnounced": true,
  "allowedPresenters": "everyone",
  "allowMeetingChat": "enabled",
  "allowTeamworkReactions": true
}
```
><span data-ttu-id="b4171-174">**注意：** 如果指定了 'Accept-Language: ja' 来指示日语，则响应将包括以下内容。</span><span class="sxs-lookup"><span data-stu-id="b4171-174">**Note:** If 'Accept-Language: ja' is specified to indicate Japanese, for example, the response will include the following.</span></span>

```json
    "joinInformation": {
        "content": "data%3Atext%2Fhtml%2C%0A++%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A%09+%3C%2Fdiv%3E%0A++++%3Cdiv+class%3D%22me-email-text%22+style%3D%22color%3A%23252424%3Bfont-family%3A'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3B%22%3E%0A+++%3Cdiv+style%3D%22margin-top%3A+24px%3B+margin-bottom%3A+10px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-headline%22%0A++++++++++++++style%3D%22font-size%3A+18px%3Bfont-family%3A'Segoe+UI+Semibold'%2C'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3Btext-decoration%3A+underline%3Bcolor%3A+%236264a7%3B%22%0A++++++++++++++href%3D%22https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%252279a788bf-86f1-41af-91ab-000000000000%2522%252c%2522Oid%2522%253a%2522d4a060b5-a8fc-450c-837b-000000000000%2522%257d%22%0A++++++++++++++target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3EMicrosoft+Teams+%E4%BC%9A%E8%AD%B0%E3%81%AB%E5%8F%82%E5%8A%A0%3C%2Fa%3E%0A++++++%3C%2Fdiv%3E%0A%09+%3Cdiv%3E%0A++++%0A++++++%3Cdiv%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+14px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22%0A++++++++++href%3D%22tel%3A%2B16477490000%2C%2C11160000%26%2335%3B+%22+target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3E%2B16477490000%3C%2Fa%3E%0A++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%26nbsp%3B++(%E6%9C%89%E6%96%99)+%3C%2Fspan%3E%0A++++++%3C%2Fdiv%3E%0A++++%0A++%3C%2Fdiv%3E%0A%0A%09+%0A++++++%3Cdiv+style%3D%22margin-top%3A+10px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++++++%E4%BC%9A%E8%AD%B0+ID%3A%0A++++++++%3C%2Fspan%3E%0A++++++%3Cspan+style%3D%22font-size%3A+14px%3B%22%3E%0A++++++++111+000+00%23%0A++++++%3C%2Fspan%3E%0A++++%3C%2Fdiv%3E%0A++++%0A%09+%0A++++++++%3Cdiv+style%3D%22margin-bottom%3A+24px%3B%22%3E%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fdialin.teams.microsoft.com%2F8bf6e654-57eb-4b85-aeaf-36c84429b2fe%3Fid%3D11160000%22+rel%3D%22noreferrer+noopener%22%3E%E6%9C%80%E5%AF%84%E3%82%8A%E3%81%AE%E5%9B%BD%E3%81%AE%E9%9B%BB%E8%A9%B1%E7%95%AA%E5%8F%B7%E3%82%92%E6%A4%9C%E7%B4%A2%3C%2Fa%3E%0A+++++++++%7C%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fmysettings.lync.com%2Fpstnconferencing%22+rel%3D%22noreferrer+noopener%22%3E%0A++++++++PIN+%E3%82%92%E3%83%AA%E3%82%BB%E3%83%83%E3%83%88%3C%2Fa%3E%0A+++++++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Faka.ms%2FJoinTeamsMeeting%22+rel%3D%22noreferrer+noopener%22%3ETeams+%E3%81%AE%E8%A9%B3%E7%B4%B0%E3%82%92%E8%A1%A8%E7%A4%BA%3C%2Fa%3E%0A+++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fteams.microsoft.com%2FmeetingOptions%2F%3ForganizerId%3Dd4a060b5-a8fc-450c-837b-000000000000%26tenantId%3D79a788bf-86f1-41af-91ab-000000000000%26threadId%3D19_meeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%40thread.v2%26messageId%3D0%26language%3Dja%22+rel%3D%22noreferrer+noopener%22%3E%E4%BC%9A%E8%AD%B0%E3%81%AE%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B3%3C%2Fa%3E%0A++++%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%E3%83%93%E3%83%87%E3%82%AA%E4%BC%9A%E8%AD%B0%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E3%81%A7%E5%8F%82%E5%8A%A0%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A12px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22%22%3E000000000%40t.abcd.vc%3C%2Fa%3E+VTC+%E4%BC%9A%E8%AD%B0+ID%3A+0180300000%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A+12px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22https%3A%2F%2Fdialin.abcd.vc%2Fteams%2F%3Fkey%3D000000000%26conf%3D0180308922%22%3E%E4%BB%A3%E6%9B%BF+VTC+%E3%81%AE%E3%83%80%E3%82%A4%E3%83%A4%E3%83%AB%E6%96%B9%E6%B3%95%3C%2Fa%3E%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++%0A++++++%3C%2Fdiv%3E%0A++++++%3Cdiv+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++%0A++++++%3C%2Fdiv%3E%0A++++%0A+++++%3C%2Fdiv%3E%0A%09+%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A++%3C%2Fdiv%3E%22%2C%0A",
        "contentType": "Html"
    }  
```

### <a name="example-2-retrieve-an-online-meeting-by-meeting-id"></a><span data-ttu-id="b4171-175">示例 2：按会议 ID 检索联机会议</span><span class="sxs-lookup"><span data-stu-id="b4171-175">Example 2: Retrieve an online meeting by meeting ID</span></span>
<span data-ttu-id="b4171-176">可以使用用户或应用程序令牌通过会议 ID 检索会议信息。</span><span class="sxs-lookup"><span data-stu-id="b4171-176">You can retrieve meeting information via meeting ID with either a user or application token.</span></span> <span data-ttu-id="b4171-177">创建 [onlineMeeting](../resources/onlinemeeting.md)时，响应对象中会提供会议 ID。</span><span class="sxs-lookup"><span data-stu-id="b4171-177">The meeting ID is provided in the response object when creating an [onlineMeeting](../resources/onlinemeeting.md).</span></span> <span data-ttu-id="b4171-178">此选项可用于支持已知会议 ID 的用例，例如当应用程序首先使用 Graph API 创建联机会议时，稍后将检索会议信息作为单独操作。</span><span class="sxs-lookup"><span data-stu-id="b4171-178">This option is available to support use cases where the meeting ID is known, such as when an application first creates the online meeting using Graph API first then retrieves meeting information later as a separate action.</span></span>

#### <a name="request"></a><span data-ttu-id="b4171-179">请求</span><span class="sxs-lookup"><span data-stu-id="b4171-179">Request</span></span>

> <span data-ttu-id="b4171-180">**注意：** 为了可读性，会议 ID 已被截断。</span><span class="sxs-lookup"><span data-stu-id="b4171-180">**Note:** The meeting ID has been truncated for readability.</span></span>

<span data-ttu-id="b4171-181">以下请求使用用户令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-181">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

<span data-ttu-id="b4171-182">以下请求使用应用程序令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-182">The following request uses an app token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

#### <a name="response"></a><span data-ttu-id="b4171-183">响应</span><span class="sxs-lookup"><span data-stu-id="b4171-183">Response</span></span>

```json
{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy",
    "creationDateTime": "2020-09-29T22:35:33.1594516Z",
    "startDateTime": "2020-09-29T22:35:31.389759Z",
    "endDateTime": "2020-09-29T23:35:31.389759Z",
    "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
    "subject": null,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "allowMeetingChat": "enabled",
    "allowTeamworkReactions": true,
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    }
}
```

### <a name="example-3-retrieve-an-online-meeting-by-joinweburl"></a><span data-ttu-id="b4171-184">示例 3：通过 JoinWebUrl 检索联机会议</span><span class="sxs-lookup"><span data-stu-id="b4171-184">Example 3: Retrieve an online meeting by JoinWebUrl</span></span>
<span data-ttu-id="b4171-185">您可以使用用户令牌或应用程序令牌通过 JoinWebUrl 检索会议信息。</span><span class="sxs-lookup"><span data-stu-id="b4171-185">You can retrieve meeting information via JoinWebUrl by using either a user or application token.</span></span> <span data-ttu-id="b4171-186">此选项可用于支持会议 ID 未知但 JoinWebUrl 为的用例，例如当用户创建会议 (例如，在 Microsoft Teams 客户端) 中，而单独的应用程序需要检索会议详细信息作为后续操作。</span><span class="sxs-lookup"><span data-stu-id="b4171-186">This option is available to support use cases where the meeting ID is not known but the JoinWebUrl is, such as when a user creates a meeting (for example in the Microsoft Teams client), and a seperate application needs to retrieve meeting details as a followup action.</span></span>

#### <a name="request"></a><span data-ttu-id="b4171-187">请求</span><span class="sxs-lookup"><span data-stu-id="b4171-187">Request</span></span>

<span data-ttu-id="b4171-188">以下请求使用用户令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-188">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

<span data-ttu-id="b4171-189">以下请求使用应用程序令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-189">The following request uses an app token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

#### <a name="response"></a><span data-ttu-id="b4171-190">响应</span><span class="sxs-lookup"><span data-stu-id="b4171-190">Response</span></span>

```json
{
    "value": [
        {
            "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2@thread.v2",
            "creationDateTime": "2020-09-29T22:35:33.1594516Z",
            "startDateTime": "2020-09-29T22:35:31.389759Z",
            "endDateTime": "2020-09-29T23:35:31.389759Z",
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
            "subject": null,
            "autoAdmittedUsers": "EveryoneInCompany",
            "isEntryExitAnnounced": true,
            "allowedPresenters": "everyone",
            "allowMeetingChat": "enabled",
            "allowTeamworkReactions": true,
            "videoTeleconferenceId": "(redacted)",
            "participants": {
                "organizer": {
                    "upn": "(redacted)",
                    "role": "presenter",
                    "identity": {
                        "user": {
                            "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                            "displayName": null,
                            "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                            "identityProvider": "AAD"
                        }
                    }
                },
                "attendees": [],
                "producers": [],
                "contributors": []
            },
            "lobbyBypassSettings": {
                "scope": "organization",
                "isDialInBypassEnabled": false
            }
        }
    ]
}
```

### <a name="example-4-retrieve-the-attendee-report-of-a-live-event"></a><span data-ttu-id="b4171-191">示例 4：检索实时事件的与会者报告</span><span class="sxs-lookup"><span data-stu-id="b4171-191">Example 4: Retrieve the attendee report of a live event</span></span>
<span data-ttu-id="b4171-192">以下示例显示下载与会者报告的请求。</span><span class="sxs-lookup"><span data-stu-id="b4171-192">The following example shows a request to download an attendee report.</span></span>

#### <a name="request"></a><span data-ttu-id="b4171-193">请求</span><span class="sxs-lookup"><span data-stu-id="b4171-193">Request</span></span>
<span data-ttu-id="b4171-194">以下请求使用用户令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-194">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/attendeeReport
```

<span data-ttu-id="b4171-195">以下请求使用应用程序令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-195">The following request uses an app token.</span></span>
# <a name="http"></a>[<span data-ttu-id="b4171-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4171-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dc74d9bb-6afe-433d-8eaa-e39d80d3a647", "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2"],
  "name": "get-attendeeReport-app-token"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/attendeeReport
```
# <a name="c"></a>[<span data-ttu-id="b4171-197">C#</span><span class="sxs-lookup"><span data-stu-id="b4171-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendeereport-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4171-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4171-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendeereport-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4171-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4171-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendeereport-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4171-200">Java</span><span class="sxs-lookup"><span data-stu-id="b4171-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendeereport-app-token-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4171-201">响应</span><span class="sxs-lookup"><span data-stu-id="b4171-201">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/attendeeReport
```

### <a name="example-5-retrieve-the-recording-of-a-live-event"></a><span data-ttu-id="b4171-202">示例 5：检索实时事件的录制</span><span class="sxs-lookup"><span data-stu-id="b4171-202">Example 5: Retrieve the recording of a live event</span></span>
<span data-ttu-id="b4171-203">以下示例显示下载录制的请求。</span><span class="sxs-lookup"><span data-stu-id="b4171-203">The following example shows a request to download a recording.</span></span>

#### <a name="request"></a><span data-ttu-id="b4171-204">请求</span><span class="sxs-lookup"><span data-stu-id="b4171-204">Request</span></span>
<span data-ttu-id="b4171-205">以下请求使用用户令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-205">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/recording
```

<span data-ttu-id="b4171-206">以下请求使用应用程序令牌。</span><span class="sxs-lookup"><span data-stu-id="b4171-206">The following request uses an app token.</span></span>
# <a name="http"></a>[<span data-ttu-id="b4171-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4171-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dc74d9bb-6afe-433d-8eaa-e39d80d3a647", "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2"],
  "name": "get-recording-app-token"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/recording
```
# <a name="c"></a>[<span data-ttu-id="b4171-208">C#</span><span class="sxs-lookup"><span data-stu-id="b4171-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recording-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4171-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4171-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recording-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4171-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4171-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recording-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4171-211">Java</span><span class="sxs-lookup"><span data-stu-id="b4171-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recording-app-token-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4171-212">响应</span><span class="sxs-lookup"><span data-stu-id="b4171-212">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/recording
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

### <a name="example-6-retrieve-the-attendance-report-of-a-meeting"></a><span data-ttu-id="b4171-213">示例 6：检索会议与会者报告</span><span class="sxs-lookup"><span data-stu-id="b4171-213">Example 6: Retrieve the attendance report of a meeting</span></span>
<span data-ttu-id="b4171-214">以下示例显示获取会议出席报告的请求。</span><span class="sxs-lookup"><span data-stu-id="b4171-214">The following example shows a request to get a meeting attendance report.</span></span>

#### <a name="request"></a><span data-ttu-id="b4171-215">请求</span><span class="sxs-lookup"><span data-stu-id="b4171-215">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b4171-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4171-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dc74d9bb-6afe-433d-8eaa-e39d80d3a647", "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy"],
  "name": "get-meetingAttendanceReport"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```
# <a name="c"></a>[<span data-ttu-id="b4171-217">C#</span><span class="sxs-lookup"><span data-stu-id="b4171-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-meetingattendancereport-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4171-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4171-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-meetingattendancereport-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4171-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4171-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-meetingattendancereport-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4171-220">Java</span><span class="sxs-lookup"><span data-stu-id="b4171-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-meetingattendancereport-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="b4171-221">响应</span><span class="sxs-lookup"><span data-stu-id="b4171-221">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1876

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('dc74d9bb-6afe-433d-8eaa-e39d80d3a647')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy')/meetingAttendanceReport/$entity",
    "attendanceRecords": [
        {
            "emailAddress": "email address",
            "totalAttendanceInSeconds": 1558,
            "role": "Organizer",
            "identity": {
                "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
                "displayName": "(redacted)",
                "tenantId": null
            },
            "attendanceIntervals": [
                {
                    "joinDateTime": "2021-03-16T18:59:46.598956Z",
                    "leaveDateTime": "2021-03-16T19:25:45.4473057Z",
                    "durationInSeconds": 1558
                }
            ]
        },
        {
            "emailAddress": "email address",
            "totalAttendanceInSeconds": 1152,
            "role": "Presenter",
            "identity": {
                "id": "(redacted)",
                "displayName": "(redacted)",
                "tenantId": null
            },
            "attendanceIntervals": [
                {
                    "joinDateTime": "2021-03-16T18:59:52.2782182Z",
                    "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
                    "durationInSeconds": 415
                },
                {
                    "joinDateTime": "2021-03-16T19:09:23.9834702Z",
                    "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
                    "durationInSeconds": 427
                },
                {
                    "joinDateTime": "2021-03-16T19:20:27.7094382Z",
                    "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
                    "durationInSeconds": 310
                }
            ]
        }
    ]
}

```
