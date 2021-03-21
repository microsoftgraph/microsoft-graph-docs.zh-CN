---
title: call： transfer
description: 转接活动对等呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 52b9d681c9eb56fe7428634d253adf5b6c0cc545
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958618"
---
# <a name="call-transfer"></a><span data-ttu-id="0211b-103">call： transfer</span><span class="sxs-lookup"><span data-stu-id="0211b-103">call: transfer</span></span>

<span data-ttu-id="0211b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0211b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0211b-105">转接活动对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="0211b-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="0211b-106">**注意：** 只有当被转移方和转移目标都是属于同一租户的 Microsoft Teams 用户时，才支持此操作。</span><span class="sxs-lookup"><span data-stu-id="0211b-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="0211b-107">仅应用程序实例支持转接到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="0211b-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="0211b-108">若要了解有关转移方、被转移方和转移目标有关详细信息，请参阅 [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2)。</span><span class="sxs-lookup"><span data-stu-id="0211b-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="0211b-109">咨询转接意味着在转接之前，转接人可以通知要呼叫 (转接) 转接给被叫方。</span><span class="sxs-lookup"><span data-stu-id="0211b-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="0211b-110">这与直接转移呼叫相反。</span><span class="sxs-lookup"><span data-stu-id="0211b-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="0211b-111">权限</span><span class="sxs-lookup"><span data-stu-id="0211b-111">Permissions</span></span>
<span data-ttu-id="0211b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0211b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0211b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="0211b-114">Permission type</span></span> | <span data-ttu-id="0211b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0211b-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="0211b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0211b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0211b-117">不支持</span><span class="sxs-lookup"><span data-stu-id="0211b-117">Not Supported</span></span>                |
| <span data-ttu-id="0211b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0211b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0211b-119">不支持</span><span class="sxs-lookup"><span data-stu-id="0211b-119">Not Supported</span></span>                |
| <span data-ttu-id="0211b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0211b-120">Application</span></span>     | <span data-ttu-id="0211b-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="0211b-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="0211b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0211b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="0211b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0211b-123">Request headers</span></span>
| <span data-ttu-id="0211b-124">名称</span><span class="sxs-lookup"><span data-stu-id="0211b-124">Name</span></span>          | <span data-ttu-id="0211b-125">说明</span><span class="sxs-lookup"><span data-stu-id="0211b-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0211b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0211b-126">Authorization</span></span> | <span data-ttu-id="0211b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0211b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0211b-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="0211b-129">Content-type</span></span>  | <span data-ttu-id="0211b-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0211b-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0211b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="0211b-132">Request body</span></span>
<span data-ttu-id="0211b-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0211b-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0211b-134">参数</span><span class="sxs-lookup"><span data-stu-id="0211b-134">Parameter</span></span>      | <span data-ttu-id="0211b-135">类型</span><span class="sxs-lookup"><span data-stu-id="0211b-135">Type</span></span>    |<span data-ttu-id="0211b-136">说明</span><span class="sxs-lookup"><span data-stu-id="0211b-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0211b-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="0211b-137">transferTarget</span></span>|[<span data-ttu-id="0211b-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="0211b-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="0211b-139">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="0211b-139">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="0211b-140">clientContext</span><span class="sxs-lookup"><span data-stu-id="0211b-140">clientContext</span></span>|<span data-ttu-id="0211b-141">String</span><span class="sxs-lookup"><span data-stu-id="0211b-141">String</span></span>|<span data-ttu-id="0211b-142">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="0211b-142">Unique Client Context string.</span></span> <span data-ttu-id="0211b-143">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="0211b-143">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="0211b-144">响应</span><span class="sxs-lookup"><span data-stu-id="0211b-144">Response</span></span>
<span data-ttu-id="0211b-145">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0211b-145">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0211b-146">示例</span><span class="sxs-lookup"><span data-stu-id="0211b-146">Examples</span></span>
<span data-ttu-id="0211b-147">这些示例显示传入呼叫一向到不同类型的转移通知的流。</span><span class="sxs-lookup"><span data-stu-id="0211b-147">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="0211b-148">示例 1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="0211b-148">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="0211b-149">请求</span><span class="sxs-lookup"><span data-stu-id="0211b-149">Request</span></span>
<span data-ttu-id="0211b-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0211b-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0211b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0211b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-1"
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
# <a name="c"></a>[<span data-ttu-id="0211b-152">C#</span><span class="sxs-lookup"><span data-stu-id="0211b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0211b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0211b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0211b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0211b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0211b-155">Java</span><span class="sxs-lookup"><span data-stu-id="0211b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0211b-156">响应</span><span class="sxs-lookup"><span data-stu-id="0211b-156">Response</span></span>

> <span data-ttu-id="0211b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0211b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="0211b-159">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="0211b-159">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="0211b-160">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="0211b-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="0211b-161">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="0211b-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="0211b-162">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="0211b-162">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="0211b-163">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="0211b-163">Notification - transfer failed</span></span>

> <span data-ttu-id="0211b-164">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="0211b-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="0211b-165">示例 2：咨询转接</span><span class="sxs-lookup"><span data-stu-id="0211b-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="0211b-166">请求</span><span class="sxs-lookup"><span data-stu-id="0211b-166">Request</span></span>
<span data-ttu-id="0211b-167">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0211b-167">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer-2"
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

##### <a name="response"></a><span data-ttu-id="0211b-168">响应</span><span class="sxs-lookup"><span data-stu-id="0211b-168">Response</span></span>

> <span data-ttu-id="0211b-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0211b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="0211b-171">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="0211b-171">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="0211b-172">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="0211b-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="0211b-173">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="0211b-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="0211b-174">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="0211b-174">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="0211b-175">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="0211b-175">Notification - transfer failed</span></span>

> <span data-ttu-id="0211b-176">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="0211b-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="0211b-177">示例 3：呼叫转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="0211b-177">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="0211b-178">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="0211b-178">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="0211b-179">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="0211b-179">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="0211b-180">请求</span><span class="sxs-lookup"><span data-stu-id="0211b-180">Request</span></span>
<span data-ttu-id="0211b-181">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0211b-181">The following example shows the request.</span></span>

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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

#### <a name="response"></a><span data-ttu-id="0211b-182">响应</span><span class="sxs-lookup"><span data-stu-id="0211b-182">Response</span></span>

> <span data-ttu-id="0211b-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0211b-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="0211b-185">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="0211b-185">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="0211b-186">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="0211b-186">Notification - transfer accepted</span></span>

> <span data-ttu-id="0211b-187">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="0211b-187">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="0211b-188">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="0211b-188">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="0211b-189">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="0211b-189">Notification - transfer failed</span></span>

> <span data-ttu-id="0211b-190">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="0211b-190">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
        }
      }
    }
  ]
}
```

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="0211b-191">示例 4：咨询转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="0211b-191">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="0211b-192">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="0211b-192">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="0211b-193">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="0211b-193">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="0211b-194">请求</span><span class="sxs-lookup"><span data-stu-id="0211b-194">Request</span></span>
<span data-ttu-id="0211b-195">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0211b-195">The following example shows the request.</span></span>

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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

#### <a name="response"></a><span data-ttu-id="0211b-196">响应</span><span class="sxs-lookup"><span data-stu-id="0211b-196">Response</span></span>

> <span data-ttu-id="0211b-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0211b-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="0211b-199">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="0211b-199">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="0211b-200">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="0211b-200">Notification - transfer accepted</span></span>

> <span data-ttu-id="0211b-201">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="0211b-201">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="0211b-202">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="0211b-202">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="0211b-203">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="0211b-203">Notification - transfer failed</span></span>

> <span data-ttu-id="0211b-204">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="0211b-204">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
        }
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

