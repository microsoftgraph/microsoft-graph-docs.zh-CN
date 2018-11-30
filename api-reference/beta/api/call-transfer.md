---
title: 呼叫： 传输
description: 将活动呼叫转接。
ms.openlocfilehash: d02e028c4d7e3b51f3aee371e22d00b95841d9a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046112"
---
# <a name="call-transfer"></a><span data-ttu-id="8956c-103">呼叫： 传输</span><span class="sxs-lookup"><span data-stu-id="8956c-103">call: transfer</span></span>

> <span data-ttu-id="8956c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8956c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8956c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8956c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8956c-106">将活动呼叫转接。</span><span class="sxs-lookup"><span data-stu-id="8956c-106">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8956c-107">权限</span><span class="sxs-lookup"><span data-stu-id="8956c-107">Permissions</span></span>
<span data-ttu-id="8956c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8956c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8956c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8956c-110">Permission type</span></span> | <span data-ttu-id="8956c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8956c-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="8956c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8956c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8956c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="8956c-113">Not Supported</span></span>                |
| <span data-ttu-id="8956c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8956c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8956c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="8956c-115">Not Supported</span></span>                |
| <span data-ttu-id="8956c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8956c-116">Application</span></span>     | <span data-ttu-id="8956c-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="8956c-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8956c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8956c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="8956c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8956c-119">Request headers</span></span>
| <span data-ttu-id="8956c-120">名称</span><span class="sxs-lookup"><span data-stu-id="8956c-120">Name</span></span>          | <span data-ttu-id="8956c-121">说明</span><span class="sxs-lookup"><span data-stu-id="8956c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8956c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8956c-122">Authorization</span></span> | <span data-ttu-id="8956c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8956c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8956c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8956c-125">Request body</span></span>
<span data-ttu-id="8956c-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8956c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8956c-127">参数</span><span class="sxs-lookup"><span data-stu-id="8956c-127">Parameter</span></span>      | <span data-ttu-id="8956c-128">类型</span><span class="sxs-lookup"><span data-stu-id="8956c-128">Type</span></span>    |<span data-ttu-id="8956c-129">说明</span><span class="sxs-lookup"><span data-stu-id="8956c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8956c-130">transferTarget</span><span class="sxs-lookup"><span data-stu-id="8956c-130">transferTarget</span></span>|[<span data-ttu-id="8956c-131">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="8956c-131">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="8956c-132">这是目标转接的参与者。</span><span class="sxs-lookup"><span data-stu-id="8956c-132">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="8956c-133">target</span><span class="sxs-lookup"><span data-stu-id="8956c-133">target</span></span>|[<span data-ttu-id="8956c-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="8956c-134">identitySet</span></span>](../resources/identityset.md)||
|<span data-ttu-id="8956c-135">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="8956c-135">replacesCallId</span></span>|<span data-ttu-id="8956c-136">字符串</span><span class="sxs-lookup"><span data-stu-id="8956c-136">String</span></span>|<span data-ttu-id="8956c-137">要转接的参与者的原始呼叫 id。</span><span class="sxs-lookup"><span data-stu-id="8956c-137">Original call id of the participant that is being transferred.</span></span>|
|<span data-ttu-id="8956c-138">clientContext</span><span class="sxs-lookup"><span data-stu-id="8956c-138">clientContext</span></span>|<span data-ttu-id="8956c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="8956c-139">String</span></span>|<span data-ttu-id="8956c-140">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="8956c-140">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8956c-141">响应</span><span class="sxs-lookup"><span data-stu-id="8956c-141">Response</span></span>
<span data-ttu-id="8956c-142">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="8956c-142">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8956c-143">示例</span><span class="sxs-lookup"><span data-stu-id="8956c-143">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="8956c-144">与没有用户参与直接转接呼叫</span><span class="sxs-lookup"><span data-stu-id="8956c-144">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="8956c-145">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8956c-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8956c-146">请求</span><span class="sxs-lookup"><span data-stu-id="8956c-146">Request</span></span>
<span data-ttu-id="8956c-147">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8956c-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_transfer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value",
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="8956c-148">响应</span><span class="sxs-lookup"><span data-stu-id="8956c-148">Response</span></span>

> <span data-ttu-id="8956c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8956c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="8956c-151">通知-传输</span><span class="sxs-lookup"><span data-stu-id="8956c-151">Notification - transferring</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="8956c-152">通知-接受转接</span><span class="sxs-lookup"><span data-stu-id="8956c-152">Notification - transfer accepted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="8956c-153">通知-终止</span><span class="sxs-lookup"><span data-stu-id="8956c-153">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

### <a name="consultative-transfer"></a><span data-ttu-id="8956c-154">咨询转接</span><span class="sxs-lookup"><span data-stu-id="8956c-154">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="8956c-155">请求</span><span class="sxs-lookup"><span data-stu-id="8956c-155">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/transfer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```
<!-- {
  "blockType": "ignored",
  "@odata.type": "call_transfer"
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```

##### <a name="response"></a><span data-ttu-id="8956c-156">响应</span><span class="sxs-lookup"><span data-stu-id="8956c-156">Response</span></span>

> <span data-ttu-id="8956c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8956c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="8956c-159">通知-传输</span><span class="sxs-lookup"><span data-stu-id="8956c-159">Notification - transferring</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="8956c-160">通知-接受转接</span><span class="sxs-lookup"><span data-stu-id="8956c-160">Notification - transfer accepted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="8956c-161">通知-终止</span><span class="sxs-lookup"><span data-stu-id="8956c-161">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
