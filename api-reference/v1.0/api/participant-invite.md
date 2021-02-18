---
title: 参与者：invite
description: 邀请参与者加入活动呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9a0a6bb439a54703ab952e046ebb71486baaf31c
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272569"
---
# <a name="participant-invite"></a><span data-ttu-id="8524d-103">参与者：invite</span><span class="sxs-lookup"><span data-stu-id="8524d-103">participant: invite</span></span>

<span data-ttu-id="8524d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8524d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8524d-105">邀请参与者加入活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="8524d-105">Invite participants to the active call.</span></span>

<span data-ttu-id="8524d-106">若要详细了解如何处理操作，请参阅[通信。](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8524d-106">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="8524d-107">**注意：** 此 API 仅支持组调用。</span><span class="sxs-lookup"><span data-stu-id="8524d-107">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="8524d-108">权限</span><span class="sxs-lookup"><span data-stu-id="8524d-108">Permissions</span></span>
<span data-ttu-id="8524d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8524d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8524d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8524d-111">Permission type</span></span> | <span data-ttu-id="8524d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8524d-112">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="8524d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8524d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8524d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="8524d-114">Not supported</span></span>                       |
| <span data-ttu-id="8524d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8524d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8524d-116">不支持</span><span class="sxs-lookup"><span data-stu-id="8524d-116">Not supported</span></span>                       |
| <span data-ttu-id="8524d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8524d-117">Application</span></span>     | <span data-ttu-id="8524d-118">Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="8524d-118">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="8524d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8524d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="8524d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8524d-120">Request headers</span></span>
| <span data-ttu-id="8524d-121">名称</span><span class="sxs-lookup"><span data-stu-id="8524d-121">Name</span></span>          | <span data-ttu-id="8524d-122">说明</span><span class="sxs-lookup"><span data-stu-id="8524d-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8524d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8524d-123">Authorization</span></span> | <span data-ttu-id="8524d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8524d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8524d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="8524d-126">Content-type</span></span>  | <span data-ttu-id="8524d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8524d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8524d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8524d-129">Request body</span></span>
<span data-ttu-id="8524d-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8524d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8524d-131">参数</span><span class="sxs-lookup"><span data-stu-id="8524d-131">Parameter</span></span>      | <span data-ttu-id="8524d-132">类型</span><span class="sxs-lookup"><span data-stu-id="8524d-132">Type</span></span>    |<span data-ttu-id="8524d-133">说明</span><span class="sxs-lookup"><span data-stu-id="8524d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8524d-134">participants</span><span class="sxs-lookup"><span data-stu-id="8524d-134">participants</span></span>|<span data-ttu-id="8524d-135">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8524d-135">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="8524d-136">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="8524d-136">The participants to be invited.</span></span>|
|<span data-ttu-id="8524d-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="8524d-137">clientContext</span></span>|<span data-ttu-id="8524d-138">String</span><span class="sxs-lookup"><span data-stu-id="8524d-138">String</span></span>|<span data-ttu-id="8524d-139">唯一客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="8524d-139">Unique Client Context string.</span></span> <span data-ttu-id="8524d-140">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="8524d-140">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="8524d-141">响应</span><span class="sxs-lookup"><span data-stu-id="8524d-141">Response</span></span>
<span data-ttu-id="8524d-142">如果成功，此方法会向为此请求创建的 `200 OK` [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) 返回响应代码和具有 URI 的位置标头。</span><span class="sxs-lookup"><span data-stu-id="8524d-142">If succsessful, this method returns a `200 OK` response code and a location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> 

<span data-ttu-id="8524d-143">响应的正文包含已创建的[inviteParticipantsOperation。](../resources/inviteparticipantsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8524d-143">The body of the response contains the created [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).</span></span>

><span data-ttu-id="8524d-144">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="8524d-144">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="8524d-145">示例</span><span class="sxs-lookup"><span data-stu-id="8524d-145">Examples</span></span>
<span data-ttu-id="8524d-146">以下示例显示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8524d-146">The following examples show how to call this API.</span></span>

> <span data-ttu-id="8524d-147">**注意：** 为了可读性，可能会缩短响应对象。</span><span class="sxs-lookup"><span data-stu-id="8524d-147">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="8524d-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8524d-148">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="8524d-149">示例 1：邀请一个参与者加入现有组通话</span><span class="sxs-lookup"><span data-stu-id="8524d-149">Example 1: Invite one participant to an existing group call</span></span>

##### <a name="request"></a><span data-ttu-id="8524d-150">请求</span><span class="sxs-lookup"><span data-stu-id="8524d-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8524d-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8524d-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8524d-152">C#</span><span class="sxs-lookup"><span data-stu-id="8524d-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8524d-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8524d-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8524d-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8524d-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8524d-155">Java</span><span class="sxs-lookup"><span data-stu-id="8524d-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8524d-156">响应</span><span class="sxs-lookup"><span data-stu-id="8524d-156">Response</span></span>

> <span data-ttu-id="8524d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8524d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="8524d-159">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="8524d-159">Notification - operation completed</span></span>

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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="8524d-160">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="8524d-160">Notification - roster updated with participant added</span></span>

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

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="8524d-161">示例 2：邀请多个参与者加入现有组呼叫</span><span class="sxs-lookup"><span data-stu-id="8524d-161">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="8524d-162">**注意**：现有组呼叫必须具有有效的 [chatInfo](../resources/chatInfo.md)。</span><span class="sxs-lookup"><span data-stu-id="8524d-162">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="8524d-163">最多支持邀请 5 个参与者。</span><span class="sxs-lookup"><span data-stu-id="8524d-163">Inviting up to 5 participants is supported.</span></span>

##### <a name="request"></a><span data-ttu-id="8524d-164">请求</span><span class="sxs-lookup"><span data-stu-id="8524d-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8524d-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="8524d-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8524d-166">C#</span><span class="sxs-lookup"><span data-stu-id="8524d-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8524d-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8524d-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8524d-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8524d-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8524d-169">Java</span><span class="sxs-lookup"><span data-stu-id="8524d-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-multiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8524d-170">响应</span><span class="sxs-lookup"><span data-stu-id="8524d-170">Response</span></span>

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
##### <a name="notification---operation-completed"></a><span data-ttu-id="8524d-171">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="8524d-171">Notification - operation completed</span></span>
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
##### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="8524d-172">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="8524d-172">Notification - roster updated with participants added</span></span>
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

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="8524d-173">示例 3：邀请参与者加入现有组呼叫，替换现有的对等呼叫</span><span class="sxs-lookup"><span data-stu-id="8524d-173">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="8524d-174">替换现有对等呼叫时，邀请 API 仅支持一个参与者。</span><span class="sxs-lookup"><span data-stu-id="8524d-174">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="8524d-175">当请求正文中提供了多个参与者时，只会读取第一个参与者，其余参与者将被忽略。</span><span class="sxs-lookup"><span data-stu-id="8524d-175">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="8524d-176">**注意：** 提供邀请 API 时，仅支持一 `replacesCallId` 个参与者。</span><span class="sxs-lookup"><span data-stu-id="8524d-176">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="8524d-177">有关使用替换现有对等呼叫的详细信息，请参阅 `replacesCallId` [invitationParticipantInfo。](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8524d-177">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="8524d-178">请求</span><span class="sxs-lookup"><span data-stu-id="8524d-178">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8524d-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="8524d-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8524d-180">C#</span><span class="sxs-lookup"><span data-stu-id="8524d-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8524d-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8524d-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8524d-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8524d-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8524d-183">Java</span><span class="sxs-lookup"><span data-stu-id="8524d-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-existing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8524d-184">响应</span><span class="sxs-lookup"><span data-stu-id="8524d-184">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="8524d-185">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="8524d-185">Notification - operation completed</span></span>

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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="8524d-186">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="8524d-186">Notification - roster updated with participant added</span></span>

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

><span data-ttu-id="8524d-187">**注意：** 对于"已完成"状态，您可以预期收到有关原始对等呼叫如何终止和删除的通知。</span><span class="sxs-lookup"><span data-stu-id="8524d-187">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

### <a name="example-4-invite-one-pstn-participant-to-an-existing-group-call"></a><span data-ttu-id="8524d-188">示例 4：邀请一个 PSTN 参与者加入现有组呼叫</span><span class="sxs-lookup"><span data-stu-id="8524d-188">Example 4: Invite one PSTN participant to an existing group call</span></span>

<span data-ttu-id="8524d-189">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="8524d-189">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="8524d-190">步骤 1：创建应用程序实例</span><span class="sxs-lookup"><span data-stu-id="8524d-190">Step 1: Create application instance</span></span>
<span data-ttu-id="8524d-191">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet 以创建应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="8524d-191">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="8524d-192">有关详细信息，请参阅 [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="8524d-192">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="8524d-193">步骤 2：分配 Microsoft 365 许可证</span><span class="sxs-lookup"><span data-stu-id="8524d-193">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="8524d-194">使用租户管理员凭据登录并转到"用户 https://admin.microsoft.com/ **->用户"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="8524d-194">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="8524d-195">选择应用程序实例，分配 **Microsoft 365 国内和国际** 通话套餐和 **Microsoft 365 电话系统 - 虚拟用户** 许可证，然后单击"**保存更改"。**</span><span class="sxs-lookup"><span data-stu-id="8524d-195">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="8524d-196">如果所需许可证在租户中不可用，可以从"计费-> **购买服务"选项卡获取** 它们。</span><span class="sxs-lookup"><span data-stu-id="8524d-196">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="8524d-197">步骤 3：获取 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="8524d-197">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="8524d-198">使用租户管理员凭据登录并单击左侧面板上的"旧版 https://admin.teams.microsoft.com/ 门户"选项卡。 </span><span class="sxs-lookup"><span data-stu-id="8524d-198">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="8524d-199">In the new page， go to the **voice -> phone numbers** tab.</span><span class="sxs-lookup"><span data-stu-id="8524d-199">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="8524d-200">单击 **+** 该按钮， **选择"新建服务号码**"，然后转到 **"添加新服务号码"** 页。</span><span class="sxs-lookup"><span data-stu-id="8524d-200">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="8524d-201">选择 **国家/地区**、 **省/市/自治区/地区**、 **城市**、输入 **数量**，然后单击 **"添加** "进行搜索。</span><span class="sxs-lookup"><span data-stu-id="8524d-201">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="8524d-202">单击 **获取号码**。</span><span class="sxs-lookup"><span data-stu-id="8524d-202">Click **acquire numbers**.</span></span> <span data-ttu-id="8524d-203">新获取的号码会显示在 **电话号码选项卡** 上。</span><span class="sxs-lookup"><span data-stu-id="8524d-203">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="8524d-204">步骤 4：将 PSTN 号码分配给应用程序实例</span><span class="sxs-lookup"><span data-stu-id="8524d-204">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="8524d-205">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet，将 PSTN 号码分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="8524d-205">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="8524d-206">有关详细信息，请参阅 [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="8524d-206">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="8524d-207">请求</span><span class="sxs-lookup"><span data-stu-id="8524d-207">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8524d-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="8524d-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST /communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="8524d-209">C#</span><span class="sxs-lookup"><span data-stu-id="8524d-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8524d-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8524d-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8524d-211">响应</span><span class="sxs-lookup"><span data-stu-id="8524d-211">Response</span></span>

> <span data-ttu-id="8524d-p114">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8524d-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": null,
      "replacesCallId": null,
      "identity": {
        "user": null,
        "guest": null,
        "encrypted": null,
        "onPremises": null,
        "applicationInstance": null,
        "application": null,
        "device": null,
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ]
}
```

#### <a name="notification---operation-completed"></a><span data-ttu-id="8524d-214">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="8524d-214">Notification - operation completed</span></span>

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
                     "phone": {
                        "@odata.type": "#microsoft.graph.identity",
                        "id": "+12345678901"
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

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="8524d-215">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="8524d-215">Notification - roster updated with participant added</span></span>

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
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "phone": {
                        "@odata.type": "#microsoft.graph.identity",
                        "id": "+12345678901"
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

><span data-ttu-id="8524d-216">**注意：** 在状态中，可以预期收到有关原始对等呼叫如何 `completed` 终止和删除的通知。</span><span class="sxs-lookup"><span data-stu-id="8524d-216">**Note:** With a `completed` status, you can expect to receive notifications about how your original peer-to-peer call has been terminated and deleted.</span></span>

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

