---
title: 参与者：邀请
description: 邀请参与者加入活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 72889e4e6071e8b9a6386ebe892e8d65c30bbf3f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865812"
---
# <a name="participant-invite"></a><span data-ttu-id="add4a-103">参与者：邀请</span><span class="sxs-lookup"><span data-stu-id="add4a-103">participant: invite</span></span>

<span data-ttu-id="add4a-104">邀请参与者加入活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="add4a-104">Invite participants to the active call.</span></span>

<span data-ttu-id="add4a-105">有关如何处理操作的详细信息，请参阅[commsoperation](../resources/commsoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="add4a-105">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="add4a-106">**注意：** 组调用仅支持此 API。</span><span class="sxs-lookup"><span data-stu-id="add4a-106">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="add4a-107">权限</span><span class="sxs-lookup"><span data-stu-id="add4a-107">Permissions</span></span>
<span data-ttu-id="add4a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="add4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="add4a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="add4a-110">Permission type</span></span> | <span data-ttu-id="add4a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="add4a-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="add4a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="add4a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="add4a-113">不支持</span><span class="sxs-lookup"><span data-stu-id="add4a-113">Not supported</span></span>                       |
| <span data-ttu-id="add4a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="add4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="add4a-115">不支持</span><span class="sxs-lookup"><span data-stu-id="add4a-115">Not supported</span></span>                       |
| <span data-ttu-id="add4a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="add4a-116">Application</span></span>     | <span data-ttu-id="add4a-117">InitiateGroupCalls</span><span class="sxs-lookup"><span data-stu-id="add4a-117">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="add4a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="add4a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="add4a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="add4a-119">Request headers</span></span>
| <span data-ttu-id="add4a-120">名称</span><span class="sxs-lookup"><span data-stu-id="add4a-120">Name</span></span>          | <span data-ttu-id="add4a-121">说明</span><span class="sxs-lookup"><span data-stu-id="add4a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="add4a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="add4a-122">Authorization</span></span> | <span data-ttu-id="add4a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="add4a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="add4a-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="add4a-125">Content-type</span></span>  | <span data-ttu-id="add4a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="add4a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="add4a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="add4a-128">Request body</span></span>
<span data-ttu-id="add4a-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="add4a-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="add4a-130">参数</span><span class="sxs-lookup"><span data-stu-id="add4a-130">Parameter</span></span>      | <span data-ttu-id="add4a-131">类型</span><span class="sxs-lookup"><span data-stu-id="add4a-131">Type</span></span>    |<span data-ttu-id="add4a-132">说明</span><span class="sxs-lookup"><span data-stu-id="add4a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="add4a-133">participants</span><span class="sxs-lookup"><span data-stu-id="add4a-133">participants</span></span>|<span data-ttu-id="add4a-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="add4a-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="add4a-135">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="add4a-135">The participants to be invited.</span></span>|
|<span data-ttu-id="add4a-136">适用</span><span class="sxs-lookup"><span data-stu-id="add4a-136">clientContext</span></span>|<span data-ttu-id="add4a-137">String</span><span class="sxs-lookup"><span data-stu-id="add4a-137">String</span></span>|<span data-ttu-id="add4a-138">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="add4a-138">Unique Client Context string.</span></span> <span data-ttu-id="add4a-139">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="add4a-139">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="add4a-140">响应</span><span class="sxs-lookup"><span data-stu-id="add4a-140">Response</span></span>
<span data-ttu-id="add4a-141">如果 succsessful，此方法将返回`200 OK`响应代码和位置标头，其中包含为此请求创建的[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)的 URI。</span><span class="sxs-lookup"><span data-stu-id="add4a-141">If succsessful, this method returns a `200 OK` response code and a location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> 

<span data-ttu-id="add4a-142">响应正文包含创建的[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="add4a-142">The body of the response contains the created [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).</span></span>

><span data-ttu-id="add4a-143">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="add4a-143">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="add4a-144">示例</span><span class="sxs-lookup"><span data-stu-id="add4a-144">Examples</span></span>
<span data-ttu-id="add4a-145">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="add4a-145">The following examples show how to call this API.</span></span>

> <span data-ttu-id="add4a-146">**注意：** 为了提高可读性，响应对象可能会缩短。</span><span class="sxs-lookup"><span data-stu-id="add4a-146">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="add4a-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="add4a-147">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="add4a-148">示例1：邀请一个参与者加入一个现有的组呼叫</span><span class="sxs-lookup"><span data-stu-id="add4a-148">Example 1: Invite one participant to an existing group call</span></span>

##### <a name="request"></a><span data-ttu-id="add4a-149">请求</span><span class="sxs-lookup"><span data-stu-id="add4a-149">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="add4a-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="add4a-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="add4a-151">C#</span><span class="sxs-lookup"><span data-stu-id="add4a-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="add4a-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add4a-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="add4a-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="add4a-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="add4a-154">Java</span><span class="sxs-lookup"><span data-stu-id="add4a-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="add4a-155">响应</span><span class="sxs-lookup"><span data-stu-id="add4a-155">Response</span></span>

> <span data-ttu-id="add4a-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="add4a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "eec3812a-fdc3-4fb4-825c-a06c9f35414e",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "displayName": "string"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="add4a-158">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="add4a-158">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{ 
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "displayName": "string"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         }
      }
   ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="add4a-159">已添加参与者的通知-名单</span><span class="sxs-lookup"><span data-stu-id="add4a-159">Notification - roster updated with participant added</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "application":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}

```

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="add4a-160">示例2：将多个参与者邀请到现有组调用</span><span class="sxs-lookup"><span data-stu-id="add4a-160">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="add4a-161">**注意**：现有的组调用必须具有有效的[chatInfo](../resources/chatInfo.md)。</span><span class="sxs-lookup"><span data-stu-id="add4a-161">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="add4a-162">最高可邀请5个参与者。</span><span class="sxs-lookup"><span data-stu-id="add4a-162">Inviting up to 5 participants is supported.</span></span>

##### <a name="request"></a><span data-ttu-id="add4a-163">请求</span><span class="sxs-lookup"><span data-stu-id="add4a-163">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="add4a-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="add4a-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-multiple"
}-->

```http
POST /communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "string"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "1e126418-44a0-4a94-a6f8-0efe1ad71acb",
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="add4a-165">C#</span><span class="sxs-lookup"><span data-stu-id="add4a-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="add4a-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add4a-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="add4a-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="add4a-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="add4a-168">Java</span><span class="sxs-lookup"><span data-stu-id="add4a-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-multiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="add4a-169">响应</span><span class="sxs-lookup"><span data-stu-id="add4a-169">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
   "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e",
   "status":"Running",
   "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
   "resultInfo":null,
   "participants":[
      {
         "endpointType":null,
         "replacesCallId":null,
         "identity":{
            "user":{
              "@odata.type": "#microsoft.graph.identity",
               "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
               "displayName": "string"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      },
      {
         "endpointType":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "@odata.type": "#microsoft.graph.identity",
               "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
               "displayName": "string"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      }
   ]
}

```
##### <a name="notification---operation-completed"></a><span data-ttu-id="add4a-170">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="add4a-170">Notification - operation completed</span></span>
```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "truncated": "true",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "participants": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "displayName": "string"
              }
            }
          },
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "displayName": "string"
              }
            }
          }
        ],
        "status": "completed",
        "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
        "id": null
      }
    }
  ]
}

```
##### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="add4a-171">已添加参与者的通知-名单已更新</span><span class="sxs-lookup"><span data-stu-id="add4a-171">Notification - roster updated with participants added</span></span>
```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json

{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
     "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe"
              }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
                "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "displayName": "string"
             }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "3",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        }
      ]
    }
  ]
}


```

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="add4a-172">示例3：邀请参与者加入现有的组呼叫，替换现有的对等呼叫</span><span class="sxs-lookup"><span data-stu-id="add4a-172">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="add4a-173">邀请 API 在替换现有的对等呼叫时仅支持一个参与者。</span><span class="sxs-lookup"><span data-stu-id="add4a-173">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="add4a-174">当请求正文中提供多个参与者时，将只读取第一个参与者，并且将忽略参与者的其余部分。</span><span class="sxs-lookup"><span data-stu-id="add4a-174">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="add4a-175">**注意：** 邀请 API 仅支持一个参与者（如果`replacesCallId`提供）。</span><span class="sxs-lookup"><span data-stu-id="add4a-175">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="add4a-176">有关使用`replacesCallId`替换现有的对等呼叫的详细信息，请参阅[invitationParticipantInfo](../resources/invitationparticipantinfo.md)。</span><span class="sxs-lookup"><span data-stu-id="add4a-176">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="add4a-177">请求</span><span class="sxs-lookup"><span data-stu-id="add4a-177">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="add4a-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="add4a-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-existing"
}-->

```http
POST /communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="add4a-179">C#</span><span class="sxs-lookup"><span data-stu-id="add4a-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="add4a-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add4a-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="add4a-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="add4a-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="add4a-182">Java</span><span class="sxs-lookup"><span data-stu-id="add4a-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-existing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="add4a-183">响应</span><span class="sxs-lookup"><span data-stu-id="add4a-183">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "278405a3-f568-4b3e-b684-009193463064",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "Participant"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="add4a-184">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="add4a-184">Notification - operation completed</span></span>

``` http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json
{ 
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "displayName": "string"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"278405a3-f568-4b3e-b684-009193463064"
         }
      }
   ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="add4a-185">已添加参与者的通知-名单</span><span class="sxs-lookup"><span data-stu-id="add4a-185">Notification - roster updated with participant added</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceUrl":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "displayName": "string"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}
```

><span data-ttu-id="add4a-186">**注意：** 在 "已完成" 状态下，您可以预计收到有关如何终止和删除原始对等呼叫的通知。</span><span class="sxs-lookup"><span data-stu-id="add4a-186">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
