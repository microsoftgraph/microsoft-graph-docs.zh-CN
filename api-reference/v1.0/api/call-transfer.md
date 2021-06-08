---
title: call： transfer
description: 转接活动对等呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2214d4276fc16c198ced411fe125e13389be3480
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784911"
---
# <a name="call-transfer"></a><span data-ttu-id="838c4-103">call： transfer</span><span class="sxs-lookup"><span data-stu-id="838c4-103">call: transfer</span></span>

<span data-ttu-id="838c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="838c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="838c4-105">转接活动对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="838c4-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="838c4-106">**注意：** 这仅在被转移方和转移目标都Microsoft Teams属于同一租户的用户时受支持。</span><span class="sxs-lookup"><span data-stu-id="838c4-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="838c4-107">仅应用程序实例支持转接到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="838c4-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="838c4-108">若要了解有关转移方、被转移方和转移目标有关详细信息，请参阅 [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2)。</span><span class="sxs-lookup"><span data-stu-id="838c4-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="838c4-109">咨询转接意味着在转接之前，转接人可以通知要呼叫 (转接) 转接给被叫方。</span><span class="sxs-lookup"><span data-stu-id="838c4-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="838c4-110">这与直接转移呼叫相反。</span><span class="sxs-lookup"><span data-stu-id="838c4-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="838c4-111">权限</span><span class="sxs-lookup"><span data-stu-id="838c4-111">Permissions</span></span>
<span data-ttu-id="838c4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="838c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="838c4-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="838c4-114">Permission type</span></span> | <span data-ttu-id="838c4-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="838c4-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="838c4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="838c4-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="838c4-117">不支持</span><span class="sxs-lookup"><span data-stu-id="838c4-117">Not Supported</span></span>                |
| <span data-ttu-id="838c4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="838c4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="838c4-119">不支持</span><span class="sxs-lookup"><span data-stu-id="838c4-119">Not Supported</span></span>                |
| <span data-ttu-id="838c4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="838c4-120">Application</span></span>     | <span data-ttu-id="838c4-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="838c4-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="838c4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="838c4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="838c4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="838c4-123">Request headers</span></span>
| <span data-ttu-id="838c4-124">名称</span><span class="sxs-lookup"><span data-stu-id="838c4-124">Name</span></span>          | <span data-ttu-id="838c4-125">说明</span><span class="sxs-lookup"><span data-stu-id="838c4-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="838c4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="838c4-126">Authorization</span></span> | <span data-ttu-id="838c4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="838c4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="838c4-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="838c4-129">Content-type</span></span>  | <span data-ttu-id="838c4-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="838c4-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="838c4-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="838c4-132">Request body</span></span>
<span data-ttu-id="838c4-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="838c4-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="838c4-134">参数</span><span class="sxs-lookup"><span data-stu-id="838c4-134">Parameter</span></span>      | <span data-ttu-id="838c4-135">类型</span><span class="sxs-lookup"><span data-stu-id="838c4-135">Type</span></span>    |<span data-ttu-id="838c4-136">说明</span><span class="sxs-lookup"><span data-stu-id="838c4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="838c4-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="838c4-137">transferTarget</span></span>|[<span data-ttu-id="838c4-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="838c4-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="838c4-139">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="838c4-139">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="838c4-140">响应</span><span class="sxs-lookup"><span data-stu-id="838c4-140">Response</span></span>
<span data-ttu-id="838c4-141">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="838c4-141">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="838c4-142">示例</span><span class="sxs-lookup"><span data-stu-id="838c4-142">Examples</span></span>
<span data-ttu-id="838c4-143">这些示例显示传入呼叫一向到不同类型的转移通知的流。</span><span class="sxs-lookup"><span data-stu-id="838c4-143">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="838c4-144">示例 1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="838c4-144">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="838c4-145">请求</span><span class="sxs-lookup"><span data-stu-id="838c4-145">Request</span></span>
<span data-ttu-id="838c4-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="838c4-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="838c4-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="838c4-147">HTTP</span></span>](#tab/http)
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="838c4-148">C#</span><span class="sxs-lookup"><span data-stu-id="838c4-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="838c4-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="838c4-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="838c4-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="838c4-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="838c4-151">Java</span><span class="sxs-lookup"><span data-stu-id="838c4-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="838c4-152">响应</span><span class="sxs-lookup"><span data-stu-id="838c4-152">Response</span></span>

> <span data-ttu-id="838c4-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="838c4-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="838c4-154">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="838c4-154">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="838c4-155">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="838c4-155">Notification - transfer accepted</span></span>

> <span data-ttu-id="838c4-156">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="838c4-156">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="838c4-157">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="838c4-157">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="838c4-158">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="838c4-158">Notification - transfer failed</span></span>

> <span data-ttu-id="838c4-159">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="838c4-159">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="838c4-160">示例 2：咨询转接</span><span class="sxs-lookup"><span data-stu-id="838c4-160">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="838c4-161">请求</span><span class="sxs-lookup"><span data-stu-id="838c4-161">Request</span></span>
<span data-ttu-id="838c4-162">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="838c4-162">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="838c4-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="838c4-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-2"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="838c4-164">C#</span><span class="sxs-lookup"><span data-stu-id="838c4-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="838c4-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="838c4-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="838c4-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="838c4-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="838c4-167">响应</span><span class="sxs-lookup"><span data-stu-id="838c4-167">Response</span></span>

> <span data-ttu-id="838c4-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="838c4-168">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="838c4-169">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="838c4-169">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="838c4-170">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="838c4-170">Notification - transfer accepted</span></span>

> <span data-ttu-id="838c4-171">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="838c4-171">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="838c4-172">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="838c4-172">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="838c4-173">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="838c4-173">Notification - transfer failed</span></span>

> <span data-ttu-id="838c4-174">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="838c4-174">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="838c4-175">示例 3：呼叫转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="838c4-175">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="838c4-176">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="838c4-176">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="838c4-177">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="838c4-177">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="838c4-178">**注意：电话** ID 是 E.164 格式的电话号码。</span><span class="sxs-lookup"><span data-stu-id="838c4-178">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="838c4-179">请求</span><span class="sxs-lookup"><span data-stu-id="838c4-179">Request</span></span>
<span data-ttu-id="838c4-180">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="838c4-180">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="838c4-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="838c4-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-3"
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
# <a name="javascript"></a>[<span data-ttu-id="838c4-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="838c4-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="838c4-183">响应</span><span class="sxs-lookup"><span data-stu-id="838c4-183">Response</span></span>

> <span data-ttu-id="838c4-184">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="838c4-184">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="838c4-185">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="838c4-185">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="838c4-186">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="838c4-186">Notification - transfer accepted</span></span>

> <span data-ttu-id="838c4-187">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="838c4-187">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="838c4-188">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="838c4-188">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="838c4-189">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="838c4-189">Notification - transfer failed</span></span>

> <span data-ttu-id="838c4-190">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="838c4-190">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="838c4-191">示例 4：咨询转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="838c4-191">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="838c4-192">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="838c4-192">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="838c4-193">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="838c4-193">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="838c4-194">**注意：电话** ID 是 E.164 格式的电话号码。</span><span class="sxs-lookup"><span data-stu-id="838c4-194">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="838c4-195">请求</span><span class="sxs-lookup"><span data-stu-id="838c4-195">Request</span></span>
<span data-ttu-id="838c4-196">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="838c4-196">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="838c4-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="838c4-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-4"
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
# <a name="javascript"></a>[<span data-ttu-id="838c4-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="838c4-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="838c4-199">响应</span><span class="sxs-lookup"><span data-stu-id="838c4-199">Response</span></span>

> <span data-ttu-id="838c4-200">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="838c4-200">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="838c4-201">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="838c4-201">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="838c4-202">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="838c4-202">Notification - transfer accepted</span></span>

> <span data-ttu-id="838c4-203">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="838c4-203">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="838c4-204">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="838c4-204">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="838c4-205">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="838c4-205">Notification - transfer failed</span></span>

> <span data-ttu-id="838c4-206">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="838c4-206">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

