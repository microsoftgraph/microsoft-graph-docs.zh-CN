---
title: 更新 onlineMeeting
description: 更新联机会议的属性。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 14d083bb6ed6e74fe1017ab4a7a87ed2bf159cc9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775603"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="63433-103">更新 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="63433-103">Update onlineMeeting</span></span>

<span data-ttu-id="63433-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63433-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63433-105">更新指定的 [onlineMeeting 对象](../resources/onlinemeeting.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="63433-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="63433-106">请参阅 [请求正文](#request-body) 部分，了解支持更新的属性列表。</span><span class="sxs-lookup"><span data-stu-id="63433-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="63433-107">权限</span><span class="sxs-lookup"><span data-stu-id="63433-107">Permissions</span></span>

| <span data-ttu-id="63433-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="63433-108">Permission type</span></span>                        | <span data-ttu-id="63433-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63433-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="63433-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63433-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="63433-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63433-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="63433-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63433-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63433-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="63433-113">Not Supported.</span></span>                              |
| <span data-ttu-id="63433-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="63433-114">Application</span></span>                            | <span data-ttu-id="63433-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="63433-115">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="63433-116">\*管理员必须创建应用程序访问[](/graph/cloud-communication-online-meeting-application-access-policy)策略并授予用户，授权策略中配置的应用代表该用户更新联机会议 (请求路径) 中指定的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="63433-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="63433-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63433-117">HTTP request</span></span>
<span data-ttu-id="63433-118">若要使用委派令牌通过会议 ID 更新指定的 onlineMeeting，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="63433-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="63433-119">若要使用应用程序令牌通过会议 ID 更新指定的 onlineMeeting，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="63433-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="63433-120">**注意：**</span><span class="sxs-lookup"><span data-stu-id="63433-120">**Notes:**</span></span>
> - <span data-ttu-id="63433-121">`userId`是 Azure 用户管理门户中的[用户的对象 ID。](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="63433-121">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="63433-122">有关详细信息，请参阅应用程序 [访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。</span><span class="sxs-lookup"><span data-stu-id="63433-122">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="63433-123">`meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**</span><span class="sxs-lookup"><span data-stu-id="63433-123">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63433-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="63433-124">Request headers</span></span>
| <span data-ttu-id="63433-125">名称</span><span class="sxs-lookup"><span data-stu-id="63433-125">Name</span></span>          | <span data-ttu-id="63433-126">说明</span><span class="sxs-lookup"><span data-stu-id="63433-126">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="63433-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="63433-127">Authorization</span></span> | <span data-ttu-id="63433-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63433-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="63433-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="63433-130">Content-type</span></span>  | <span data-ttu-id="63433-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="63433-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63433-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="63433-133">Request body</span></span>
<span data-ttu-id="63433-134">下表列出了可更新的属性。</span><span class="sxs-lookup"><span data-stu-id="63433-134">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="63433-135">在请求正文中，仅包括需要更新的属性，但以下例外：</span><span class="sxs-lookup"><span data-stu-id="63433-135">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="63433-136">调整联机会议开始或结束日期/时间始终需要请求正文中的 **startDateTime** 和 **endDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="63433-136">Adjusting the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="63433-137">调整 **参与者属性** 的 **attendees** 字段（如向会议添加或删除与会者）始终需要请求正文中与会者的完整列表。</span><span class="sxs-lookup"><span data-stu-id="63433-137">Adjusting the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="63433-138">属性</span><span class="sxs-lookup"><span data-stu-id="63433-138">Property</span></span>             | <span data-ttu-id="63433-139">类型</span><span class="sxs-lookup"><span data-stu-id="63433-139">Type</span></span>                                                         | <span data-ttu-id="63433-140">说明</span><span class="sxs-lookup"><span data-stu-id="63433-140">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="63433-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="63433-141">startDateTime</span></span>        | <span data-ttu-id="63433-142">日期时间</span><span class="sxs-lookup"><span data-stu-id="63433-142">DateTime</span></span>                                                     | <span data-ttu-id="63433-143">会议开始时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="63433-143">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="63433-144">endDateTime</span><span class="sxs-lookup"><span data-stu-id="63433-144">endDateTime</span></span>          | <span data-ttu-id="63433-145">日期时间</span><span class="sxs-lookup"><span data-stu-id="63433-145">DateTime</span></span>                                                     | <span data-ttu-id="63433-146">会议结束时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="63433-146">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="63433-147">subject</span><span class="sxs-lookup"><span data-stu-id="63433-147">subject</span></span>              | <span data-ttu-id="63433-148">String</span><span class="sxs-lookup"><span data-stu-id="63433-148">String</span></span>                                                       | <span data-ttu-id="63433-149">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="63433-149">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="63433-150">participants</span><span class="sxs-lookup"><span data-stu-id="63433-150">participants</span></span>         | [<span data-ttu-id="63433-151">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="63433-151">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="63433-152">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="63433-152">The participants associated with the online meeting.</span></span> <span data-ttu-id="63433-153">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="63433-153">This includes the organizer and the attendees.</span></span>                                            |
| <span data-ttu-id="63433-154">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="63433-154">isEntryExitAnnounced</span></span> | <span data-ttu-id="63433-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="63433-155">Boolean</span></span>                                                      | <span data-ttu-id="63433-156">呼叫者加入或离开时是否宣布。</span><span class="sxs-lookup"><span data-stu-id="63433-156">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="63433-157">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="63433-157">lobbyBypassSettings</span></span>  | [<span data-ttu-id="63433-158">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="63433-158">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="63433-159">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="63433-159">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="63433-160">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="63433-160">allowedPresenters</span></span>    | <span data-ttu-id="63433-161">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="63433-161">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="63433-162">指定可在会议中成为演示者的人。</span><span class="sxs-lookup"><span data-stu-id="63433-162">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="63433-163">可能的值包括 everyone、organization、roleIsPresenter、organizer 和 unknownFutureValue。</span><span class="sxs-lookup"><span data-stu-id="63433-163">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="63433-164">响应</span><span class="sxs-lookup"><span data-stu-id="63433-164">Response</span></span>
<span data-ttu-id="63433-165">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63433-165">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63433-166">示例</span><span class="sxs-lookup"><span data-stu-id="63433-166">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="63433-167">示例 1：更新 startDateTime、endDateTime 和 subject</span><span class="sxs-lookup"><span data-stu-id="63433-167">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="63433-168">请求</span><span class="sxs-lookup"><span data-stu-id="63433-168">Request</span></span>

> <span data-ttu-id="63433-169">**注意：** 为了可读性，会议 ID 已被截断。</span><span class="sxs-lookup"><span data-stu-id="63433-169">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="63433-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="63433-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="63433-171">C#</span><span class="sxs-lookup"><span data-stu-id="63433-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63433-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63433-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63433-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63433-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63433-174">Java</span><span class="sxs-lookup"><span data-stu-id="63433-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63433-175">响应</span><span class="sxs-lookup"><span data-stu-id="63433-175">Response</span></span>

> <span data-ttu-id="63433-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63433-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"+1-900-555-0100",
      "tollFreeNumber":"+1-800-555-0100",
      "dialinUrl":"url"
   }
}
```

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="63433-178">示例 2：更新 lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="63433-178">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="63433-179">**注意：** 为了可读性，会议 ID 已被截断。</span><span class="sxs-lookup"><span data-stu-id="63433-179">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="63433-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="63433-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="63433-181">C#</span><span class="sxs-lookup"><span data-stu-id="63433-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63433-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63433-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63433-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63433-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63433-184">Java</span><span class="sxs-lookup"><span data-stu-id="63433-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63433-185">响应</span><span class="sxs-lookup"><span data-stu-id="63433-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
    "creationDateTime":"2020-07-03T00:23:39.444642Z",
    "startDateTime":"2020-09-09T21:33:30.8546353Z",
    "endDateTime":"2020-09-09T22:03:30.8566356Z",
    "joinWebUrl":"(redacted)",
    "subject":"Patch Meeting Subject",
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
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
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


