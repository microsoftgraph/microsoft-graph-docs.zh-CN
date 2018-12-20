---
title: 呼叫： 传输
description: 将活动呼叫转接。
author: VinodRavichandran
ms.openlocfilehash: 71d250453051c705dcc0646a8e4ad298253d0ee6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380504"
---
# <a name="call-transfer"></a><span data-ttu-id="19eba-103">呼叫： 传输</span><span class="sxs-lookup"><span data-stu-id="19eba-103">call: transfer</span></span>

> <span data-ttu-id="19eba-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="19eba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19eba-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19eba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19eba-106">将活动呼叫转接。</span><span class="sxs-lookup"><span data-stu-id="19eba-106">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="19eba-107">权限</span><span class="sxs-lookup"><span data-stu-id="19eba-107">Permissions</span></span>
<span data-ttu-id="19eba-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19eba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19eba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="19eba-110">Permission type</span></span> | <span data-ttu-id="19eba-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19eba-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="19eba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19eba-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="19eba-113">不支持</span><span class="sxs-lookup"><span data-stu-id="19eba-113">Not Supported</span></span>                |
| <span data-ttu-id="19eba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19eba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19eba-115">不支持</span><span class="sxs-lookup"><span data-stu-id="19eba-115">Not Supported</span></span>                |
| <span data-ttu-id="19eba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="19eba-116">Application</span></span>     | <span data-ttu-id="19eba-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="19eba-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="19eba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19eba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="19eba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="19eba-119">Request headers</span></span>
| <span data-ttu-id="19eba-120">名称</span><span class="sxs-lookup"><span data-stu-id="19eba-120">Name</span></span>          | <span data-ttu-id="19eba-121">说明</span><span class="sxs-lookup"><span data-stu-id="19eba-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="19eba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19eba-122">Authorization</span></span> | <span data-ttu-id="19eba-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19eba-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19eba-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="19eba-125">Request body</span></span>
<span data-ttu-id="19eba-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19eba-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19eba-127">参数</span><span class="sxs-lookup"><span data-stu-id="19eba-127">Parameter</span></span>      | <span data-ttu-id="19eba-128">类型</span><span class="sxs-lookup"><span data-stu-id="19eba-128">Type</span></span>    |<span data-ttu-id="19eba-129">说明</span><span class="sxs-lookup"><span data-stu-id="19eba-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19eba-130">transferTarget</span><span class="sxs-lookup"><span data-stu-id="19eba-130">transferTarget</span></span>|[<span data-ttu-id="19eba-131">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="19eba-131">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="19eba-132">这是目标转接的参与者。</span><span class="sxs-lookup"><span data-stu-id="19eba-132">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="19eba-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="19eba-133">clientContext</span></span>|<span data-ttu-id="19eba-134">字符串</span><span class="sxs-lookup"><span data-stu-id="19eba-134">String</span></span>|<span data-ttu-id="19eba-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="19eba-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="19eba-136">响应</span><span class="sxs-lookup"><span data-stu-id="19eba-136">Response</span></span>
<span data-ttu-id="19eba-137">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="19eba-137">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="19eba-138">示例</span><span class="sxs-lookup"><span data-stu-id="19eba-138">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="19eba-139">与没有用户参与直接转接呼叫</span><span class="sxs-lookup"><span data-stu-id="19eba-139">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="19eba-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="19eba-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="19eba-141">请求</span><span class="sxs-lookup"><span data-stu-id="19eba-141">Request</span></span>
<span data-ttu-id="19eba-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="19eba-142">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-transfer"
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

##### <a name="response"></a><span data-ttu-id="19eba-143">响应</span><span class="sxs-lookup"><span data-stu-id="19eba-143">Response</span></span>

> <span data-ttu-id="19eba-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="19eba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="19eba-146">通知-传输</span><span class="sxs-lookup"><span data-stu-id="19eba-146">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="19eba-147">通知-接受转接</span><span class="sxs-lookup"><span data-stu-id="19eba-147">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="19eba-148">通知-终止</span><span class="sxs-lookup"><span data-stu-id="19eba-148">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="19eba-149">咨询转接</span><span class="sxs-lookup"><span data-stu-id="19eba-149">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="19eba-150">请求</span><span class="sxs-lookup"><span data-stu-id="19eba-150">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/transfer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```
<!-- {
  "blockType": "ignored",
  "@odata.type": "call-transfer"
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

##### <a name="response"></a><span data-ttu-id="19eba-151">响应</span><span class="sxs-lookup"><span data-stu-id="19eba-151">Response</span></span>

> <span data-ttu-id="19eba-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="19eba-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="19eba-154">通知-传输</span><span class="sxs-lookup"><span data-stu-id="19eba-154">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="19eba-155">通知-接受转接</span><span class="sxs-lookup"><span data-stu-id="19eba-155">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="19eba-156">通知-终止</span><span class="sxs-lookup"><span data-stu-id="19eba-156">Notification - terminated</span></span>

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
