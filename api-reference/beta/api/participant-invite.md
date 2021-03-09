---
title: 参与者：invite
description: 邀请参与者加入活动呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 295a8aa728754d8e4ffc6d2f412c44059a63c794
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578344"
---
# <a name="participant-invite"></a><span data-ttu-id="d7155-103">参与者：invite</span><span class="sxs-lookup"><span data-stu-id="d7155-103">participant: invite</span></span>

<span data-ttu-id="d7155-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7155-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7155-105">邀请参与者加入活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="d7155-105">Invite participants to the active call.</span></span>

<span data-ttu-id="d7155-106">若要详细了解如何处理操作，请参阅[通信。](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="d7155-106">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="d7155-107">**注意：** 此 API 仅支持组调用。</span><span class="sxs-lookup"><span data-stu-id="d7155-107">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7155-108">权限</span><span class="sxs-lookup"><span data-stu-id="d7155-108">Permissions</span></span>
<span data-ttu-id="d7155-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7155-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7155-111">Permission type</span></span> | <span data-ttu-id="d7155-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7155-112">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="d7155-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7155-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7155-114">不支持</span><span class="sxs-lookup"><span data-stu-id="d7155-114">Not supported</span></span>                       |
| <span data-ttu-id="d7155-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7155-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7155-116">不支持</span><span class="sxs-lookup"><span data-stu-id="d7155-116">Not supported</span></span>                       |
| <span data-ttu-id="d7155-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7155-117">Application</span></span>     | <span data-ttu-id="d7155-118">Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="d7155-118">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="d7155-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7155-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /communications/calls/{id}/participants/invite
```
> <span data-ttu-id="d7155-120">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="d7155-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d7155-121">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="d7155-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7155-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7155-122">Request headers</span></span>
| <span data-ttu-id="d7155-123">名称</span><span class="sxs-lookup"><span data-stu-id="d7155-123">Name</span></span>          | <span data-ttu-id="d7155-124">说明</span><span class="sxs-lookup"><span data-stu-id="d7155-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d7155-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7155-125">Authorization</span></span> | <span data-ttu-id="d7155-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7155-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7155-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="d7155-128">Content-type</span></span>  | <span data-ttu-id="d7155-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d7155-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7155-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7155-131">Request body</span></span>
<span data-ttu-id="d7155-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d7155-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7155-133">参数</span><span class="sxs-lookup"><span data-stu-id="d7155-133">Parameter</span></span>      | <span data-ttu-id="d7155-134">类型</span><span class="sxs-lookup"><span data-stu-id="d7155-134">Type</span></span>    |<span data-ttu-id="d7155-135">说明</span><span class="sxs-lookup"><span data-stu-id="d7155-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7155-136">participants</span><span class="sxs-lookup"><span data-stu-id="d7155-136">participants</span></span>|<span data-ttu-id="d7155-137">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7155-137">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="d7155-138">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="d7155-138">The participants to be invited.</span></span>|
|<span data-ttu-id="d7155-139">clientContext</span><span class="sxs-lookup"><span data-stu-id="d7155-139">clientContext</span></span>|<span data-ttu-id="d7155-140">字符串</span><span class="sxs-lookup"><span data-stu-id="d7155-140">String</span></span>|<span data-ttu-id="d7155-141">唯一客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="d7155-141">Unique Client Context string.</span></span> <span data-ttu-id="d7155-142">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="d7155-142">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="d7155-143">响应</span><span class="sxs-lookup"><span data-stu-id="d7155-143">Response</span></span>
<span data-ttu-id="d7155-144">如果成功，此方法会向为此请求创建的 `200 OK` [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) 返回响应代码和具有 URI 的位置标头。</span><span class="sxs-lookup"><span data-stu-id="d7155-144">If succsessful, this method returns a `200 OK` response code and a Location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> <span data-ttu-id="d7155-145">响应的正文包含[创建的 inviteParticipantsOperation。](../resources/inviteparticipantsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="d7155-145">The body of the response contains the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created.</span></span>

><span data-ttu-id="d7155-146">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="d7155-146">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="d7155-147">示例</span><span class="sxs-lookup"><span data-stu-id="d7155-147">Examples</span></span>
<span data-ttu-id="d7155-148">以下示例显示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d7155-148">The following examples show how to call this API.</span></span>

> <span data-ttu-id="d7155-149">**注意：** 为了可读性，可能会缩短响应对象。</span><span class="sxs-lookup"><span data-stu-id="d7155-149">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="d7155-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d7155-150">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="d7155-151">示例 1：邀请一个参与者加入现有组通话</span><span class="sxs-lookup"><span data-stu-id="d7155-151">Example 1: Invite one participant to an existing group call</span></span>

#### <a name="request"></a><span data-ttu-id="d7155-152">请求</span><span class="sxs-lookup"><span data-stu-id="d7155-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d7155-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7155-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

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
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="d7155-154">C#</span><span class="sxs-lookup"><span data-stu-id="d7155-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7155-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7155-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7155-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7155-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7155-157">响应</span><span class="sxs-lookup"><span data-stu-id="d7155-157">Response</span></span>

> <span data-ttu-id="d7155-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d7155-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

#### <a name="notification---operation-completed"></a><span data-ttu-id="d7155-160">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="d7155-160">Notification - operation completed</span></span>

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
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="d7155-161">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="d7155-161">Notification - roster updated with participant added</span></span>

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
                     "application":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="d7155-162">示例 2：邀请多个参与者加入现有组呼叫</span><span class="sxs-lookup"><span data-stu-id="d7155-162">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="d7155-163">**注意**：现有组呼叫必须具有有效的 [chatInfo](../resources/chatInfo.md)。</span><span class="sxs-lookup"><span data-stu-id="d7155-163">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="d7155-164">最多支持邀请 5 个参与者。</span><span class="sxs-lookup"><span data-stu-id="d7155-164">Inviting up to 5 participants is supported.</span></span>

#### <a name="request"></a><span data-ttu-id="d7155-165">请求</span><span class="sxs-lookup"><span data-stu-id="d7155-165">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d7155-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7155-166">HTTP</span></span>](#tab/http)
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
          "identityProvider": "AAD"
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
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="d7155-167">C#</span><span class="sxs-lookup"><span data-stu-id="d7155-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7155-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7155-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7155-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7155-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d7155-170">响应</span><span class="sxs-lookup"><span data-stu-id="d7155-170">Response</span></span>

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
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      },
      {
         "endpointType":null,
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      }
   ]
}

```
#### <a name="notification---operation-completed"></a><span data-ttu-id="d7155-171">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="d7155-171">Notification - operation completed</span></span>
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
                "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            }
          },
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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
#### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="d7155-172">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="d7155-172">Notification - roster updated with participants added</span></span>
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
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
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
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="d7155-173">示例 3：邀请参与者加入现有组呼叫，替换现有的对等呼叫</span><span class="sxs-lookup"><span data-stu-id="d7155-173">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="d7155-174">替换现有对等调用时，邀请 API 仅支持一个参与者。</span><span class="sxs-lookup"><span data-stu-id="d7155-174">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="d7155-175">当请求正文中提供了多个参与者时，只会读取第一个参与者，其余参与者将被忽略。</span><span class="sxs-lookup"><span data-stu-id="d7155-175">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="d7155-176">**注意：** 提供邀请 API 时，仅支持一 `replacesCallId` 个参与者。</span><span class="sxs-lookup"><span data-stu-id="d7155-176">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="d7155-177">有关使用替换现有对等呼叫的详细信息，请参阅 `replacesCallId` [invitationParticipantInfo。](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="d7155-177">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

#### <a name="request"></a><span data-ttu-id="d7155-178">请求</span><span class="sxs-lookup"><span data-stu-id="d7155-178">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d7155-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7155-179">HTTP</span></span>](#tab/http)
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
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="d7155-180">C#</span><span class="sxs-lookup"><span data-stu-id="d7155-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7155-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7155-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7155-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7155-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7155-183">响应</span><span class="sxs-lookup"><span data-stu-id="d7155-183">Response</span></span>

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
      "id": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "Participant",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

#### <a name="notification---operation-completed"></a><span data-ttu-id="d7155-184">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="d7155-184">Notification - operation completed</span></span>

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
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="d7155-185">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="d7155-185">Notification - roster updated with participant added</span></span>

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
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

><span data-ttu-id="d7155-186">**注意：** 对于"已完成"状态，您可以预期收到有关原始对等呼叫如何终止和删除的通知。</span><span class="sxs-lookup"><span data-stu-id="d7155-186">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

### <a name="example-4-invite-one-pstn-participant-to-an-existing-group-call"></a><span data-ttu-id="d7155-187">示例 4：邀请一个 PSTN 参与者加入现有组呼叫</span><span class="sxs-lookup"><span data-stu-id="d7155-187">Example 4: Invite one PSTN participant to an existing group call</span></span>

<span data-ttu-id="d7155-188">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="d7155-188">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="d7155-189">有关详细信息，请参阅 [为自动程序分配电话号码](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="d7155-189">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="d7155-190">请求</span><span class="sxs-lookup"><span data-stu-id="d7155-190">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/invite
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

#### <a name="response"></a><span data-ttu-id="d7155-191">响应</span><span class="sxs-lookup"><span data-stu-id="d7155-191">Response</span></span>

> <span data-ttu-id="d7155-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d7155-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="notification---operation-completed"></a><span data-ttu-id="d7155-194">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="d7155-194">Notification - operation completed</span></span>

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

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="d7155-195">通知 - 已添加参与者更新名单</span><span class="sxs-lookup"><span data-stu-id="d7155-195">Notification - roster updated with participant added</span></span>

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

><span data-ttu-id="d7155-196">**注意：** 在状态中，可以预期收到有关原始对等呼叫如何 `completed` 终止和删除的通知。</span><span class="sxs-lookup"><span data-stu-id="d7155-196">**Note:** With a `completed` status, you can expect to receive notifications about how your original peer-to-peer call has been terminated and deleted.</span></span>

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


