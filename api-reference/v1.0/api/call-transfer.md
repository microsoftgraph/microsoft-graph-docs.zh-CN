---
title: 呼叫：转移
description: 转移活动的对等呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 940c3a7fb1e2f1320e2598d379bd659cec2c1710
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865831"
---
# <a name="call-transfer"></a><span data-ttu-id="e5c63-103">呼叫：转移</span><span class="sxs-lookup"><span data-stu-id="e5c63-103">call: transfer</span></span>

<span data-ttu-id="e5c63-104">转移活动的对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="e5c63-104">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="e5c63-105">**注意：** 仅当受让方和 transfer 目标是属于同一租户的 Microsoft 团队用户时，才支持此项。</span><span class="sxs-lookup"><span data-stu-id="e5c63-105">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="e5c63-106">不支持转移到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="e5c63-106">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="e5c63-107">若要了解有关 transferor、受让方和转让目标的详细信息，请参阅[RFC 5589](https://tools.ietf.org/html/rfc5589#section-2)。</span><span class="sxs-lookup"><span data-stu-id="e5c63-107">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="e5c63-108">咨询转移意味着在进行转移之前，transferor 可以通知他们要将呼叫转接到的人员（受让方）。</span><span class="sxs-lookup"><span data-stu-id="e5c63-108">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="e5c63-109">这与直接传输呼叫相对。</span><span class="sxs-lookup"><span data-stu-id="e5c63-109">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5c63-110">权限</span><span class="sxs-lookup"><span data-stu-id="e5c63-110">Permissions</span></span>
<span data-ttu-id="e5c63-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5c63-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5c63-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5c63-113">Permission type</span></span> | <span data-ttu-id="e5c63-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5c63-114">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="e5c63-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5c63-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5c63-116">不支持</span><span class="sxs-lookup"><span data-stu-id="e5c63-116">Not Supported</span></span>                |
| <span data-ttu-id="e5c63-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5c63-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c63-118">不支持</span><span class="sxs-lookup"><span data-stu-id="e5c63-118">Not Supported</span></span>                |
| <span data-ttu-id="e5c63-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5c63-119">Application</span></span>     | <span data-ttu-id="e5c63-120">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="e5c63-120">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="e5c63-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5c63-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="e5c63-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5c63-122">Request headers</span></span>
| <span data-ttu-id="e5c63-123">名称</span><span class="sxs-lookup"><span data-stu-id="e5c63-123">Name</span></span>          | <span data-ttu-id="e5c63-124">说明</span><span class="sxs-lookup"><span data-stu-id="e5c63-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e5c63-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5c63-125">Authorization</span></span> | <span data-ttu-id="e5c63-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5c63-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5c63-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="e5c63-128">Content-type</span></span>  | <span data-ttu-id="e5c63-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5c63-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5c63-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5c63-131">Request body</span></span>
<span data-ttu-id="e5c63-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e5c63-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5c63-133">参数</span><span class="sxs-lookup"><span data-stu-id="e5c63-133">Parameter</span></span>      | <span data-ttu-id="e5c63-134">类型</span><span class="sxs-lookup"><span data-stu-id="e5c63-134">Type</span></span>    |<span data-ttu-id="e5c63-135">说明</span><span class="sxs-lookup"><span data-stu-id="e5c63-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5c63-136">transferTarget</span><span class="sxs-lookup"><span data-stu-id="e5c63-136">transferTarget</span></span>|[<span data-ttu-id="e5c63-137">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="e5c63-137">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="e5c63-138">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="e5c63-138">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="e5c63-139">适用</span><span class="sxs-lookup"><span data-stu-id="e5c63-139">clientContext</span></span>|<span data-ttu-id="e5c63-140">String</span><span class="sxs-lookup"><span data-stu-id="e5c63-140">String</span></span>|<span data-ttu-id="e5c63-141">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="e5c63-141">Unique Client Context string.</span></span> <span data-ttu-id="e5c63-142">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="e5c63-142">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="e5c63-143">响应</span><span class="sxs-lookup"><span data-stu-id="e5c63-143">Response</span></span>
<span data-ttu-id="e5c63-144">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e5c63-144">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e5c63-145">示例</span><span class="sxs-lookup"><span data-stu-id="e5c63-145">Examples</span></span>
<span data-ttu-id="e5c63-146">这些示例显示传入呼叫在不同类型的转移通知中一直流动的流。</span><span class="sxs-lookup"><span data-stu-id="e5c63-146">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="e5c63-147">示例1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="e5c63-147">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="e5c63-148">请求</span><span class="sxs-lookup"><span data-stu-id="e5c63-148">Request</span></span>
<span data-ttu-id="e5c63-149">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5c63-149">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e5c63-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5c63-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "displayName": "Heidi Steen"
      }
    },
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e5c63-151">C#</span><span class="sxs-lookup"><span data-stu-id="e5c63-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5c63-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5c63-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5c63-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5c63-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e5c63-154">Java</span><span class="sxs-lookup"><span data-stu-id="e5c63-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5c63-155">响应</span><span class="sxs-lookup"><span data-stu-id="e5c63-155">Response</span></span>

> <span data-ttu-id="e5c63-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5c63-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="e5c63-158">通知-转移</span><span class="sxs-lookup"><span data-stu-id="e5c63-158">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="e5c63-159">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="e5c63-159">Notification - transfer accepted</span></span>

> <span data-ttu-id="e5c63-160">**注意：** 在媒体状态音频非活动状态发生之后或之前，接受的传输可能会发生。</span><span class="sxs-lookup"><span data-stu-id="e5c63-160">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="e5c63-161">通知-转移已完成</span><span class="sxs-lookup"><span data-stu-id="e5c63-161">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="e5c63-162">通知-传输失败</span><span class="sxs-lookup"><span data-stu-id="e5c63-162">Notification - transfer failed</span></span>

> <span data-ttu-id="e5c63-163">**注意：** 当呼叫转移失败时，呼叫状态将为`established`。</span><span class="sxs-lookup"><span data-stu-id="e5c63-163">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="e5c63-164">示例2：咨询转移</span><span class="sxs-lookup"><span data-stu-id="e5c63-164">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="e5c63-165">请求</span><span class="sxs-lookup"><span data-stu-id="e5c63-165">Request</span></span>
<span data-ttu-id="e5c63-166">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5c63-166">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
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
        "displayName": "Heidi Steen"
      }
    },
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

##### <a name="response"></a><span data-ttu-id="e5c63-167">响应</span><span class="sxs-lookup"><span data-stu-id="e5c63-167">Response</span></span>

> <span data-ttu-id="e5c63-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5c63-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="e5c63-170">通知-转移</span><span class="sxs-lookup"><span data-stu-id="e5c63-170">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="e5c63-171">通知-传输已接受</span><span class="sxs-lookup"><span data-stu-id="e5c63-171">Notification - transfer accepted</span></span>

> <span data-ttu-id="e5c63-172">**注意：** 在媒体状态音频非活动状态发生之后或之前，接受的传输可能会发生。</span><span class="sxs-lookup"><span data-stu-id="e5c63-172">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="e5c63-173">通知-转移已完成</span><span class="sxs-lookup"><span data-stu-id="e5c63-173">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="e5c63-174">通知-传输失败</span><span class="sxs-lookup"><span data-stu-id="e5c63-174">Notification - transfer failed</span></span>

> <span data-ttu-id="e5c63-175">**注意：** 当呼叫转移失败时，呼叫状态将为`established`。</span><span class="sxs-lookup"><span data-stu-id="e5c63-175">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
