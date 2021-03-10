---
title: call： transfer
description: 转移活动对等呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2feec9b37375da3b76191ec84869346c07af36f3
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573766"
---
# <a name="call-transfer"></a><span data-ttu-id="71ab0-103">call： transfer</span><span class="sxs-lookup"><span data-stu-id="71ab0-103">call: transfer</span></span>

<span data-ttu-id="71ab0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71ab0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71ab0-105">转移活动对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="71ab0-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="71ab0-106">**注意：** 这仅在被转移方和转移目标都是属于同一租户的 Microsoft Teams 用户时受支持。</span><span class="sxs-lookup"><span data-stu-id="71ab0-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="71ab0-107">仅应用程序实例支持转移到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="71ab0-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="71ab0-108">若要了解有关转移方、被转移方和转移目标更多信息，请参阅[RFC 5589。](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="71ab0-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="71ab0-109">咨询转接意味着，在转接之前，转接方可以通知 (呼叫) 转接给被叫方。</span><span class="sxs-lookup"><span data-stu-id="71ab0-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="71ab0-110">这与直接转移呼叫相反。</span><span class="sxs-lookup"><span data-stu-id="71ab0-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="71ab0-111">权限</span><span class="sxs-lookup"><span data-stu-id="71ab0-111">Permissions</span></span>
<span data-ttu-id="71ab0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71ab0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71ab0-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="71ab0-114">Permission type</span></span> | <span data-ttu-id="71ab0-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71ab0-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="71ab0-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71ab0-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="71ab0-117">不支持</span><span class="sxs-lookup"><span data-stu-id="71ab0-117">Not Supported</span></span>                |
| <span data-ttu-id="71ab0-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71ab0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71ab0-119">不支持</span><span class="sxs-lookup"><span data-stu-id="71ab0-119">Not Supported</span></span>                |
| <span data-ttu-id="71ab0-120">Application</span><span class="sxs-lookup"><span data-stu-id="71ab0-120">Application</span></span>     | <span data-ttu-id="71ab0-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="71ab0-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="71ab0-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71ab0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="71ab0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="71ab0-123">Request headers</span></span>
| <span data-ttu-id="71ab0-124">名称</span><span class="sxs-lookup"><span data-stu-id="71ab0-124">Name</span></span>          | <span data-ttu-id="71ab0-125">说明</span><span class="sxs-lookup"><span data-stu-id="71ab0-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="71ab0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="71ab0-126">Authorization</span></span> | <span data-ttu-id="71ab0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71ab0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71ab0-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="71ab0-129">Content-type</span></span>  | <span data-ttu-id="71ab0-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="71ab0-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ab0-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="71ab0-132">Request body</span></span>
<span data-ttu-id="71ab0-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="71ab0-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71ab0-134">参数</span><span class="sxs-lookup"><span data-stu-id="71ab0-134">Parameter</span></span>      | <span data-ttu-id="71ab0-135">类型</span><span class="sxs-lookup"><span data-stu-id="71ab0-135">Type</span></span>    |<span data-ttu-id="71ab0-136">说明</span><span class="sxs-lookup"><span data-stu-id="71ab0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71ab0-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="71ab0-137">transferTarget</span></span>|[<span data-ttu-id="71ab0-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="71ab0-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="71ab0-139">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="71ab0-139">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="71ab0-140">clientContext</span><span class="sxs-lookup"><span data-stu-id="71ab0-140">clientContext</span></span>|<span data-ttu-id="71ab0-141">String</span><span class="sxs-lookup"><span data-stu-id="71ab0-141">String</span></span>|<span data-ttu-id="71ab0-142">唯一客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="71ab0-142">Unique Client Context string.</span></span> <span data-ttu-id="71ab0-143">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="71ab0-143">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="71ab0-144">响应</span><span class="sxs-lookup"><span data-stu-id="71ab0-144">Response</span></span>
<span data-ttu-id="71ab0-145">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="71ab0-145">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="71ab0-146">示例</span><span class="sxs-lookup"><span data-stu-id="71ab0-146">Examples</span></span>
<span data-ttu-id="71ab0-147">这些示例显示了传入呼叫一路流向不同类型的传输通知。</span><span class="sxs-lookup"><span data-stu-id="71ab0-147">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="71ab0-148">示例 1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="71ab0-148">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="71ab0-149">请求</span><span class="sxs-lookup"><span data-stu-id="71ab0-149">Request</span></span>
<span data-ttu-id="71ab0-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="71ab0-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="71ab0-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ab0-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="71ab0-152">C#</span><span class="sxs-lookup"><span data-stu-id="71ab0-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71ab0-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ab0-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71ab0-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ab0-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71ab0-155">Java</span><span class="sxs-lookup"><span data-stu-id="71ab0-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71ab0-156">响应</span><span class="sxs-lookup"><span data-stu-id="71ab0-156">Response</span></span>

> <span data-ttu-id="71ab0-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71ab0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="71ab0-159">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="71ab0-159">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="71ab0-160">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="71ab0-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="71ab0-161">**注意：** 在媒体状态音频处于非活动状态之后或之前，可能会接受传输。</span><span class="sxs-lookup"><span data-stu-id="71ab0-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="71ab0-162">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="71ab0-162">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="71ab0-163">通知 - 传输失败</span><span class="sxs-lookup"><span data-stu-id="71ab0-163">Notification - transfer failed</span></span>

> <span data-ttu-id="71ab0-164">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="71ab0-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="71ab0-165">示例 2：咨询转接</span><span class="sxs-lookup"><span data-stu-id="71ab0-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="71ab0-166">请求</span><span class="sxs-lookup"><span data-stu-id="71ab0-166">Request</span></span>
<span data-ttu-id="71ab0-167">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="71ab0-167">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="71ab0-168">响应</span><span class="sxs-lookup"><span data-stu-id="71ab0-168">Response</span></span>

> <span data-ttu-id="71ab0-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71ab0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="71ab0-171">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="71ab0-171">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="71ab0-172">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="71ab0-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="71ab0-173">**注意：** 在媒体状态音频处于非活动状态之后或之前，可能会接受传输。</span><span class="sxs-lookup"><span data-stu-id="71ab0-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="71ab0-174">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="71ab0-174">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="71ab0-175">通知 - 传输失败</span><span class="sxs-lookup"><span data-stu-id="71ab0-175">Notification - transfer failed</span></span>

> <span data-ttu-id="71ab0-176">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="71ab0-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="71ab0-177">示例 3：呼叫转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="71ab0-177">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="71ab0-178">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="71ab0-178">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="71ab0-179">有关详细信息，请参阅 [为自动程序分配电话号码](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="71ab0-179">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="71ab0-180">请求</span><span class="sxs-lookup"><span data-stu-id="71ab0-180">Request</span></span>
<span data-ttu-id="71ab0-181">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="71ab0-181">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="71ab0-182">响应</span><span class="sxs-lookup"><span data-stu-id="71ab0-182">Response</span></span>

> <span data-ttu-id="71ab0-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71ab0-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="71ab0-185">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="71ab0-185">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="71ab0-186">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="71ab0-186">Notification - transfer accepted</span></span>

> <span data-ttu-id="71ab0-187">**注意：** 在媒体状态音频处于非活动状态之后或之前，可能会接受传输。</span><span class="sxs-lookup"><span data-stu-id="71ab0-187">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="71ab0-188">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="71ab0-188">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="71ab0-189">通知 - 传输失败</span><span class="sxs-lookup"><span data-stu-id="71ab0-189">Notification - transfer failed</span></span>

> <span data-ttu-id="71ab0-190">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="71ab0-190">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="71ab0-191">示例 4：咨询转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="71ab0-191">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="71ab0-192">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="71ab0-192">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="71ab0-193">有关详细信息，请参阅 [为自动程序分配电话号码](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="71ab0-193">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="71ab0-194">请求</span><span class="sxs-lookup"><span data-stu-id="71ab0-194">Request</span></span>
<span data-ttu-id="71ab0-195">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="71ab0-195">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="71ab0-196">响应</span><span class="sxs-lookup"><span data-stu-id="71ab0-196">Response</span></span>

> <span data-ttu-id="71ab0-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71ab0-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="71ab0-199">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="71ab0-199">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="71ab0-200">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="71ab0-200">Notification - transfer accepted</span></span>

> <span data-ttu-id="71ab0-201">**注意：** 在媒体状态音频处于非活动状态之后或之前，可能会接受传输。</span><span class="sxs-lookup"><span data-stu-id="71ab0-201">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="71ab0-202">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="71ab0-202">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="71ab0-203">通知 - 传输失败</span><span class="sxs-lookup"><span data-stu-id="71ab0-203">Notification - transfer failed</span></span>

> <span data-ttu-id="71ab0-204">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="71ab0-204">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

