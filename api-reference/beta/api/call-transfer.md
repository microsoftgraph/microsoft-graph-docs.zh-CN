---
title: '呼叫: 转移'
description: 转移活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 92cb446303278d95eeb9f852491566b6305d468b
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536062"
---
# <a name="call-transfer"></a><span data-ttu-id="f2312-103">呼叫: 转移</span><span class="sxs-lookup"><span data-stu-id="f2312-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2312-104">转移活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="f2312-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2312-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2312-105">Permissions</span></span>
<span data-ttu-id="f2312-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2312-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2312-108">Permission type</span></span> | <span data-ttu-id="f2312-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2312-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="f2312-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2312-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2312-111">不支持</span><span class="sxs-lookup"><span data-stu-id="f2312-111">Not Supported</span></span>                |
| <span data-ttu-id="f2312-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2312-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2312-113">不支持</span><span class="sxs-lookup"><span data-stu-id="f2312-113">Not Supported</span></span>                |
| <span data-ttu-id="f2312-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2312-114">Application</span></span>     | <span data-ttu-id="f2312-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="f2312-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="f2312-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2312-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="f2312-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2312-117">Request headers</span></span>
| <span data-ttu-id="f2312-118">名称</span><span class="sxs-lookup"><span data-stu-id="f2312-118">Name</span></span>          | <span data-ttu-id="f2312-119">说明</span><span class="sxs-lookup"><span data-stu-id="f2312-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f2312-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2312-120">Authorization</span></span> | <span data-ttu-id="f2312-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2312-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2312-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2312-123">Request body</span></span>
<span data-ttu-id="f2312-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f2312-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f2312-125">参数</span><span class="sxs-lookup"><span data-stu-id="f2312-125">Parameter</span></span>      | <span data-ttu-id="f2312-126">类型</span><span class="sxs-lookup"><span data-stu-id="f2312-126">Type</span></span>    |<span data-ttu-id="f2312-127">说明</span><span class="sxs-lookup"><span data-stu-id="f2312-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2312-128">transferTarget</span><span class="sxs-lookup"><span data-stu-id="f2312-128">transferTarget</span></span>|[<span data-ttu-id="f2312-129">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="f2312-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="f2312-130">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="f2312-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="f2312-131">适用</span><span class="sxs-lookup"><span data-stu-id="f2312-131">clientContext</span></span>|<span data-ttu-id="f2312-132">String</span><span class="sxs-lookup"><span data-stu-id="f2312-132">String</span></span>|<span data-ttu-id="f2312-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="f2312-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="f2312-134">响应</span><span class="sxs-lookup"><span data-stu-id="f2312-134">Response</span></span>
<span data-ttu-id="f2312-135">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2312-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2312-136">示例</span><span class="sxs-lookup"><span data-stu-id="f2312-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="f2312-137">直接转接呼叫, 无用户参与</span><span class="sxs-lookup"><span data-stu-id="f2312-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="f2312-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f2312-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f2312-139">请求</span><span class="sxs-lookup"><span data-stu-id="f2312-139">Request</span></span>
<span data-ttu-id="f2312-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2312-140">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f2312-141">响应</span><span class="sxs-lookup"><span data-stu-id="f2312-141">Response</span></span>

> <span data-ttu-id="f2312-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f2312-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f2312-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f2312-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f2312-145">C#</span><span class="sxs-lookup"><span data-stu-id="f2312-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-transfer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2312-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2312-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-transfer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---transferring"></a><span data-ttu-id="f2312-147">通知-转移</span><span class="sxs-lookup"><span data-stu-id="f2312-147">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="f2312-148">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="f2312-148">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="f2312-149">通知终止</span><span class="sxs-lookup"><span data-stu-id="f2312-149">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="f2312-150">咨询转移</span><span class="sxs-lookup"><span data-stu-id="f2312-150">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="f2312-151">请求</span><span class="sxs-lookup"><span data-stu-id="f2312-151">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="f2312-152">响应</span><span class="sxs-lookup"><span data-stu-id="f2312-152">Response</span></span>

> <span data-ttu-id="f2312-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f2312-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="f2312-155">通知-转移</span><span class="sxs-lookup"><span data-stu-id="f2312-155">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="f2312-156">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="f2312-156">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="f2312-157">通知终止</span><span class="sxs-lookup"><span data-stu-id="f2312-157">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-transfer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-transfer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
