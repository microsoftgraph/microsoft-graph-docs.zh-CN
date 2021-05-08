---
title: 更新 onlineMeeting
description: 更新联机会议的属性。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6d239a98275b6ca8fb390ae646f67a82c2212c99
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241077"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="580e8-103">更新 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="580e8-103">Update onlineMeeting</span></span>

<span data-ttu-id="580e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="580e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="580e8-105">更新指定的 [onlineMeeting 对象](../resources/onlinemeeting.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="580e8-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="580e8-106">请参阅 [请求正文](#request-body) 部分，了解支持更新的属性列表。</span><span class="sxs-lookup"><span data-stu-id="580e8-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="580e8-107">权限</span><span class="sxs-lookup"><span data-stu-id="580e8-107">Permissions</span></span>

| <span data-ttu-id="580e8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="580e8-108">Permission type</span></span>                        | <span data-ttu-id="580e8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="580e8-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="580e8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="580e8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="580e8-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="580e8-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="580e8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="580e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="580e8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="580e8-113">Not Supported.</span></span>                              |
| <span data-ttu-id="580e8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="580e8-114">Application</span></span>                            | <span data-ttu-id="580e8-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="580e8-115">OnlineMeetings.ReadWrite.All\*</span></span>               |

> [!IMPORTANT]
> <span data-ttu-id="580e8-116">\*管理员必须创建应用程序访问[](/graph/cloud-communication-online-meeting-application-access-policy)策略并授予用户，授权策略中配置的应用代表该用户更新联机会议 (请求路径) 中指定的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="580e8-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="580e8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="580e8-117">HTTP request</span></span>
<span data-ttu-id="580e8-118">若要使用委派令牌通过会议 ID 更新指定的 onlineMeeting，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="580e8-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="580e8-119">若要使用应用程序令牌通过会议 ID 更新指定的 onlineMeeting，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="580e8-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
> - <span data-ttu-id="580e8-120">`userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="580e8-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="580e8-121">有关详细信息，请参阅应用程序 [访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。</span><span class="sxs-lookup"><span data-stu-id="580e8-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="580e8-122">`meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**</span><span class="sxs-lookup"><span data-stu-id="580e8-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="580e8-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="580e8-123">Request headers</span></span>
| <span data-ttu-id="580e8-124">名称</span><span class="sxs-lookup"><span data-stu-id="580e8-124">Name</span></span>          | <span data-ttu-id="580e8-125">说明</span><span class="sxs-lookup"><span data-stu-id="580e8-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="580e8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="580e8-126">Authorization</span></span> | <span data-ttu-id="580e8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="580e8-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="580e8-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="580e8-129">Content-type</span></span>  | <span data-ttu-id="580e8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="580e8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="580e8-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="580e8-132">Request body</span></span>
<span data-ttu-id="580e8-133">下表列出了可更新的属性。</span><span class="sxs-lookup"><span data-stu-id="580e8-133">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="580e8-134">在请求正文中，仅包括需要更新的属性，但以下例外：</span><span class="sxs-lookup"><span data-stu-id="580e8-134">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="580e8-135">调整联机会议开始或结束日期/时间始终需要请求正文中的 **startDateTime** 和 **endDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="580e8-135">Adjusting the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="580e8-136">**无法** 更新 **参与者属性** 的 organizer 字段。</span><span class="sxs-lookup"><span data-stu-id="580e8-136">**organizer** field of the **participants** property cannot be updated.</span></span> <span data-ttu-id="580e8-137">创建会议后，不能修改会议的组织者。</span><span class="sxs-lookup"><span data-stu-id="580e8-137">The organizer of the meeting cannot be modified once the meeting is created.</span></span>
- <span data-ttu-id="580e8-138">调整 **参与者属性** 的 **attendees** 字段（如向会议添加或删除与会者）始终需要请求正文中与会者的完整列表。</span><span class="sxs-lookup"><span data-stu-id="580e8-138">Adjusting the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="580e8-139">属性</span><span class="sxs-lookup"><span data-stu-id="580e8-139">Property</span></span>             | <span data-ttu-id="580e8-140">类型</span><span class="sxs-lookup"><span data-stu-id="580e8-140">Type</span></span>                                                         | <span data-ttu-id="580e8-141">说明</span><span class="sxs-lookup"><span data-stu-id="580e8-141">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="580e8-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="580e8-142">startDateTime</span></span>        | <span data-ttu-id="580e8-143">日期时间</span><span class="sxs-lookup"><span data-stu-id="580e8-143">DateTime</span></span>                                                     | <span data-ttu-id="580e8-144">会议开始时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="580e8-144">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="580e8-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="580e8-145">endDateTime</span></span>          | <span data-ttu-id="580e8-146">日期时间</span><span class="sxs-lookup"><span data-stu-id="580e8-146">DateTime</span></span>                                                     | <span data-ttu-id="580e8-147">会议结束时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="580e8-147">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="580e8-148">subject</span><span class="sxs-lookup"><span data-stu-id="580e8-148">subject</span></span>              | <span data-ttu-id="580e8-149">String</span><span class="sxs-lookup"><span data-stu-id="580e8-149">String</span></span>                                                       | <span data-ttu-id="580e8-150">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="580e8-150">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="580e8-151">participants</span><span class="sxs-lookup"><span data-stu-id="580e8-151">participants</span></span>         | [<span data-ttu-id="580e8-152">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="580e8-152">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="580e8-153">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="580e8-153">The participants associated with the online meeting.</span></span> <span data-ttu-id="580e8-154">仅与会者可以更新。</span><span class="sxs-lookup"><span data-stu-id="580e8-154">Only attendees can be updated.</span></span>                                            |
| <span data-ttu-id="580e8-155">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="580e8-155">isEntryExitAnnounced</span></span> | <span data-ttu-id="580e8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="580e8-156">Boolean</span></span>                                                      | <span data-ttu-id="580e8-157">呼叫者加入或离开时是否宣布。</span><span class="sxs-lookup"><span data-stu-id="580e8-157">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="580e8-158">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="580e8-158">lobbyBypassSettings</span></span>  | [<span data-ttu-id="580e8-159">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="580e8-159">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="580e8-160">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="580e8-160">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="580e8-161">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="580e8-161">allowedPresenters</span></span>    | <span data-ttu-id="580e8-162">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="580e8-162">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="580e8-163">指定可在会议中成为演示者的人。</span><span class="sxs-lookup"><span data-stu-id="580e8-163">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="580e8-164">可能的值包括 everyone、organization、roleIsPresenter、organizer 和 unknownFutureValue。</span><span class="sxs-lookup"><span data-stu-id="580e8-164">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="580e8-165">响应</span><span class="sxs-lookup"><span data-stu-id="580e8-165">Response</span></span>
<span data-ttu-id="580e8-166">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="580e8-166">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="580e8-167">示例</span><span class="sxs-lookup"><span data-stu-id="580e8-167">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="580e8-168">示例 1：更新 startDateTime、endDateTime 和 subject</span><span class="sxs-lookup"><span data-stu-id="580e8-168">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="580e8-169">请求</span><span class="sxs-lookup"><span data-stu-id="580e8-169">Request</span></span>

> <span data-ttu-id="580e8-170">**注意：** 为了可读性，会议 ID 已被截断。</span><span class="sxs-lookup"><span data-stu-id="580e8-170">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="580e8-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="580e8-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="580e8-172">C#</span><span class="sxs-lookup"><span data-stu-id="580e8-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="580e8-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="580e8-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="580e8-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="580e8-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="580e8-175">Java</span><span class="sxs-lookup"><span data-stu-id="580e8-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="580e8-176">响应</span><span class="sxs-lookup"><span data-stu-id="580e8-176">Response</span></span>

> <span data-ttu-id="580e8-177">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="580e8-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="580e8-178">示例 2：更新 lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="580e8-178">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="580e8-179">**注意：** 为了可读性，会议 ID 已被截断。</span><span class="sxs-lookup"><span data-stu-id="580e8-179">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="580e8-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="580e8-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="580e8-181">C#</span><span class="sxs-lookup"><span data-stu-id="580e8-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="580e8-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="580e8-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="580e8-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="580e8-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="580e8-184">Java</span><span class="sxs-lookup"><span data-stu-id="580e8-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="580e8-185">响应</span><span class="sxs-lookup"><span data-stu-id="580e8-185">Response</span></span>

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


