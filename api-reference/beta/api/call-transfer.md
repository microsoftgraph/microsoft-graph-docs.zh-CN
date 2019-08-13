---
title: '呼叫: 转移'
description: 转移活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 15d29ef213765fa374f1d6d958e6bf0079a5caab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317560"
---
# <a name="call-transfer"></a><span data-ttu-id="32cb1-103">呼叫: 转移</span><span class="sxs-lookup"><span data-stu-id="32cb1-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32cb1-104">转移活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="32cb1-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="32cb1-105">权限</span><span class="sxs-lookup"><span data-stu-id="32cb1-105">Permissions</span></span>
<span data-ttu-id="32cb1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32cb1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="32cb1-108">Permission type</span></span> | <span data-ttu-id="32cb1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32cb1-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="32cb1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32cb1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="32cb1-111">不支持</span><span class="sxs-lookup"><span data-stu-id="32cb1-111">Not Supported</span></span>                |
| <span data-ttu-id="32cb1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32cb1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32cb1-113">不支持</span><span class="sxs-lookup"><span data-stu-id="32cb1-113">Not Supported</span></span>                |
| <span data-ttu-id="32cb1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="32cb1-114">Application</span></span>     | <span data-ttu-id="32cb1-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="32cb1-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="32cb1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32cb1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="32cb1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="32cb1-117">Request headers</span></span>
| <span data-ttu-id="32cb1-118">名称</span><span class="sxs-lookup"><span data-stu-id="32cb1-118">Name</span></span>          | <span data-ttu-id="32cb1-119">说明</span><span class="sxs-lookup"><span data-stu-id="32cb1-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="32cb1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="32cb1-120">Authorization</span></span> | <span data-ttu-id="32cb1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32cb1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32cb1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="32cb1-123">Request body</span></span>
<span data-ttu-id="32cb1-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="32cb1-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32cb1-125">参数</span><span class="sxs-lookup"><span data-stu-id="32cb1-125">Parameter</span></span>      | <span data-ttu-id="32cb1-126">类型</span><span class="sxs-lookup"><span data-stu-id="32cb1-126">Type</span></span>    |<span data-ttu-id="32cb1-127">说明</span><span class="sxs-lookup"><span data-stu-id="32cb1-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32cb1-128">transferTarget</span><span class="sxs-lookup"><span data-stu-id="32cb1-128">transferTarget</span></span>|[<span data-ttu-id="32cb1-129">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="32cb1-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="32cb1-130">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="32cb1-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="32cb1-131">适用</span><span class="sxs-lookup"><span data-stu-id="32cb1-131">clientContext</span></span>|<span data-ttu-id="32cb1-132">String</span><span class="sxs-lookup"><span data-stu-id="32cb1-132">String</span></span>|<span data-ttu-id="32cb1-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="32cb1-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="32cb1-134">响应</span><span class="sxs-lookup"><span data-stu-id="32cb1-134">Response</span></span>
<span data-ttu-id="32cb1-135">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="32cb1-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="32cb1-136">示例</span><span class="sxs-lookup"><span data-stu-id="32cb1-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="32cb1-137">直接转接呼叫, 无用户参与</span><span class="sxs-lookup"><span data-stu-id="32cb1-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="32cb1-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="32cb1-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="32cb1-139">请求</span><span class="sxs-lookup"><span data-stu-id="32cb1-139">Request</span></span>
<span data-ttu-id="32cb1-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="32cb1-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="32cb1-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="32cb1-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="32cb1-142">C#</span><span class="sxs-lookup"><span data-stu-id="32cb1-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32cb1-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32cb1-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32cb1-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="32cb1-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="32cb1-145">Java</span><span class="sxs-lookup"><span data-stu-id="32cb1-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32cb1-146">响应</span><span class="sxs-lookup"><span data-stu-id="32cb1-146">Response</span></span>

> <span data-ttu-id="32cb1-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="32cb1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="32cb1-149">通知-转移</span><span class="sxs-lookup"><span data-stu-id="32cb1-149">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="32cb1-150">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="32cb1-150">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="32cb1-151">通知终止</span><span class="sxs-lookup"><span data-stu-id="32cb1-151">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="32cb1-152">咨询转移</span><span class="sxs-lookup"><span data-stu-id="32cb1-152">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="32cb1-153">请求</span><span class="sxs-lookup"><span data-stu-id="32cb1-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="32cb1-154">响应</span><span class="sxs-lookup"><span data-stu-id="32cb1-154">Response</span></span>

> <span data-ttu-id="32cb1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="32cb1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="32cb1-157">通知-转移</span><span class="sxs-lookup"><span data-stu-id="32cb1-157">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="32cb1-158">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="32cb1-158">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="32cb1-159">通知终止</span><span class="sxs-lookup"><span data-stu-id="32cb1-159">Notification - terminated</span></span>

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
  ]
}
-->
