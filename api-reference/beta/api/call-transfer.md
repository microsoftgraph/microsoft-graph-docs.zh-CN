---
title: 呼叫：转移
description: 转移活动的对等呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 14c2e1abae0dcc7729bfd7aa89a7a668555e60e8
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005897"
---
# <a name="call-transfer"></a><span data-ttu-id="35b00-103">呼叫：转移</span><span class="sxs-lookup"><span data-stu-id="35b00-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b00-104">转移活动的对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="35b00-104">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="35b00-105">**注意：** 仅当受让方和 transfer 目标是属于同一租户的 Microsoft 团队用户时，才支持此项。</span><span class="sxs-lookup"><span data-stu-id="35b00-105">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="35b00-106">不支持转移到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="35b00-106">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="35b00-107">若要了解有关 transferor、受让方和转让目标的详细信息，请参阅[RFC 5589](https://tools.ietf.org/html/rfc5589#section-2)。</span><span class="sxs-lookup"><span data-stu-id="35b00-107">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="35b00-108">咨询转移意味着在进行转移之前，transferor 可以通知他们要将呼叫转接到的人员（受让方）。</span><span class="sxs-lookup"><span data-stu-id="35b00-108">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="35b00-109">这与直接传输呼叫相对。</span><span class="sxs-lookup"><span data-stu-id="35b00-109">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="35b00-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="35b00-110">Permissions</span></span>
<span data-ttu-id="35b00-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35b00-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35b00-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="35b00-113">Permission type</span></span> | <span data-ttu-id="35b00-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35b00-114">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="35b00-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35b00-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="35b00-116">不支持</span><span class="sxs-lookup"><span data-stu-id="35b00-116">Not Supported</span></span>                |
| <span data-ttu-id="35b00-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35b00-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35b00-118">不支持</span><span class="sxs-lookup"><span data-stu-id="35b00-118">Not Supported</span></span>                |
| <span data-ttu-id="35b00-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="35b00-119">Application</span></span>     | <span data-ttu-id="35b00-120">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="35b00-120">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="35b00-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35b00-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="35b00-122">**注意：**`/app`路径已被弃用。</span><span class="sxs-lookup"><span data-stu-id="35b00-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="35b00-123">接下来，请使用`/communications`路径。</span><span class="sxs-lookup"><span data-stu-id="35b00-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35b00-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="35b00-124">Request headers</span></span>
| <span data-ttu-id="35b00-125">名称</span><span class="sxs-lookup"><span data-stu-id="35b00-125">Name</span></span>          | <span data-ttu-id="35b00-126">说明</span><span class="sxs-lookup"><span data-stu-id="35b00-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="35b00-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="35b00-127">Authorization</span></span> | <span data-ttu-id="35b00-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35b00-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35b00-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="35b00-130">Content-type</span></span>  | <span data-ttu-id="35b00-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="35b00-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35b00-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="35b00-133">Request body</span></span>
<span data-ttu-id="35b00-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="35b00-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="35b00-135">参数</span><span class="sxs-lookup"><span data-stu-id="35b00-135">Parameter</span></span>      | <span data-ttu-id="35b00-136">类型</span><span class="sxs-lookup"><span data-stu-id="35b00-136">Type</span></span>    |<span data-ttu-id="35b00-137">说明</span><span class="sxs-lookup"><span data-stu-id="35b00-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35b00-138">transferTarget</span><span class="sxs-lookup"><span data-stu-id="35b00-138">transferTarget</span></span>|[<span data-ttu-id="35b00-139">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="35b00-139">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="35b00-140">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="35b00-140">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="35b00-141">适用</span><span class="sxs-lookup"><span data-stu-id="35b00-141">clientContext</span></span>|<span data-ttu-id="35b00-142">String</span><span class="sxs-lookup"><span data-stu-id="35b00-142">String</span></span>|<span data-ttu-id="35b00-143">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="35b00-143">Unique Client Context string.</span></span> <span data-ttu-id="35b00-144">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="35b00-144">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="35b00-145">响应</span><span class="sxs-lookup"><span data-stu-id="35b00-145">Response</span></span>
<span data-ttu-id="35b00-146">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="35b00-146">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="35b00-147">示例</span><span class="sxs-lookup"><span data-stu-id="35b00-147">Examples</span></span>
<span data-ttu-id="35b00-148">这些示例显示传入呼叫在不同类型的转移通知中一直流动的流。</span><span class="sxs-lookup"><span data-stu-id="35b00-148">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="35b00-149">示例1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="35b00-149">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="35b00-150">请求</span><span class="sxs-lookup"><span data-stu-id="35b00-150">Request</span></span>
<span data-ttu-id="35b00-151">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="35b00-151">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="35b00-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="35b00-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/transfer
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
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35b00-153">C#</span><span class="sxs-lookup"><span data-stu-id="35b00-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35b00-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35b00-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35b00-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35b00-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="35b00-156">响应</span><span class="sxs-lookup"><span data-stu-id="35b00-156">Response</span></span>

> <span data-ttu-id="35b00-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="35b00-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="35b00-159">通知-转移</span><span class="sxs-lookup"><span data-stu-id="35b00-159">Notification - transferring</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="35b00-160">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="35b00-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="35b00-161">**注意：** 在媒体状态音频非活动状态发生之后或之前，接受的传输可能会发生。</span><span class="sxs-lookup"><span data-stu-id="35b00-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

##### <a name="notification---transfer-completed"></a><span data-ttu-id="35b00-162">通知-转移已完成</span><span class="sxs-lookup"><span data-stu-id="35b00-162">Notification - transfer completed</span></span>

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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 0,
          "subcode": 7015,
          "message": "GracefulTransferCompleted"
        }
      }
    }
  ]
}
```

##### <a name="notification---transfer-failed"></a><span data-ttu-id="35b00-163">通知-传输失败</span><span class="sxs-lookup"><span data-stu-id="35b00-163">Notification - transfer failed</span></span>

> <span data-ttu-id="35b00-164">**注意：** 当呼叫转移失败时，呼叫状态将为`established`。</span><span class="sxs-lookup"><span data-stu-id="35b00-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7000,
          "message": "<message>"
        },
        "replacesContext": "<replacesContext>"
      }
    }
  ]
}
```

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="35b00-165">示例2：咨询转移</span><span class="sxs-lookup"><span data-stu-id="35b00-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="35b00-166">请求</span><span class="sxs-lookup"><span data-stu-id="35b00-166">Request</span></span>
<span data-ttu-id="35b00-167">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="35b00-167">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
Content-Type: application/json

{
  "transferTarget": {
    "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    "endpointType": "default",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

##### <a name="response"></a><span data-ttu-id="35b00-168">响应</span><span class="sxs-lookup"><span data-stu-id="35b00-168">Response</span></span>

> <span data-ttu-id="35b00-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="35b00-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="35b00-171">通知-转移</span><span class="sxs-lookup"><span data-stu-id="35b00-171">Notification - transferring</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="35b00-172">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="35b00-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="35b00-173">**注意：** 在媒体状态音频非活动状态发生之后或之前，接受的传输可能会发生。</span><span class="sxs-lookup"><span data-stu-id="35b00-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

##### <a name="notification---transfer-completed"></a><span data-ttu-id="35b00-174">通知-转移已完成</span><span class="sxs-lookup"><span data-stu-id="35b00-174">Notification - transfer completed</span></span>

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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

##### <a name="notification---transfer-failed"></a><span data-ttu-id="35b00-175">通知-传输失败</span><span class="sxs-lookup"><span data-stu-id="35b00-175">Notification - transfer failed</span></span>

> <span data-ttu-id="35b00-176">**注意：** 当呼叫转移失败时，呼叫状态将为`established`。</span><span class="sxs-lookup"><span data-stu-id="35b00-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7700,
          "message": "<message>"
        },
        "replacesContext": "<replacesContext>"
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
