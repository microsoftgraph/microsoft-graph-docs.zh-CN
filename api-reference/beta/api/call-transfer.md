---
title: call： transfer
description: 转接活动对等呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dbc7c4b07470ea0de1e4afe492a9accfc9173d1e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664011"
---
# <a name="call-transfer"></a><span data-ttu-id="93489-103">call： transfer</span><span class="sxs-lookup"><span data-stu-id="93489-103">call: transfer</span></span>

<span data-ttu-id="93489-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93489-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93489-105">转接活动对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="93489-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="93489-106">**注意：** 这仅在被转移方和转移目标都Microsoft Teams属于同一租户的用户时受支持。</span><span class="sxs-lookup"><span data-stu-id="93489-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="93489-107">仅应用程序实例支持转接到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="93489-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="93489-108">若要了解有关转移方、被转移方和转移目标有关详细信息，请参阅 [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2)。</span><span class="sxs-lookup"><span data-stu-id="93489-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="93489-109">咨询转接意味着在转接之前，转接人可以通知要呼叫 (转接) 转接给被叫方。</span><span class="sxs-lookup"><span data-stu-id="93489-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="93489-110">这与直接转移呼叫相反。</span><span class="sxs-lookup"><span data-stu-id="93489-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="93489-111">权限</span><span class="sxs-lookup"><span data-stu-id="93489-111">Permissions</span></span>
<span data-ttu-id="93489-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93489-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93489-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="93489-114">Permission type</span></span> | <span data-ttu-id="93489-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93489-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="93489-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93489-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="93489-117">不支持</span><span class="sxs-lookup"><span data-stu-id="93489-117">Not Supported</span></span>                |
| <span data-ttu-id="93489-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93489-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93489-119">不支持</span><span class="sxs-lookup"><span data-stu-id="93489-119">Not Supported</span></span>                |
| <span data-ttu-id="93489-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="93489-120">Application</span></span>     | <span data-ttu-id="93489-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="93489-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="93489-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93489-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="93489-123">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="93489-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="93489-124">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="93489-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93489-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="93489-125">Request headers</span></span>
| <span data-ttu-id="93489-126">名称</span><span class="sxs-lookup"><span data-stu-id="93489-126">Name</span></span>          | <span data-ttu-id="93489-127">说明</span><span class="sxs-lookup"><span data-stu-id="93489-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="93489-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="93489-128">Authorization</span></span> | <span data-ttu-id="93489-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93489-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93489-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="93489-131">Content-type</span></span>  | <span data-ttu-id="93489-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="93489-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93489-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="93489-134">Request body</span></span>
<span data-ttu-id="93489-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="93489-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="93489-136">参数</span><span class="sxs-lookup"><span data-stu-id="93489-136">Parameter</span></span>      | <span data-ttu-id="93489-137">类型</span><span class="sxs-lookup"><span data-stu-id="93489-137">Type</span></span>    |<span data-ttu-id="93489-138">说明</span><span class="sxs-lookup"><span data-stu-id="93489-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93489-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="93489-139">transferTarget</span></span>|[<span data-ttu-id="93489-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="93489-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="93489-141">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="93489-141">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="93489-142">响应</span><span class="sxs-lookup"><span data-stu-id="93489-142">Response</span></span>
<span data-ttu-id="93489-143">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="93489-143">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="93489-144">示例</span><span class="sxs-lookup"><span data-stu-id="93489-144">Examples</span></span>
<span data-ttu-id="93489-145">这些示例显示传入呼叫一向到不同类型的转移通知的流。</span><span class="sxs-lookup"><span data-stu-id="93489-145">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="93489-146">示例 1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="93489-146">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="93489-147">请求</span><span class="sxs-lookup"><span data-stu-id="93489-147">Request</span></span>
<span data-ttu-id="93489-148">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="93489-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93489-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="93489-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-1"
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
    "region": "region-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="93489-150">C#</span><span class="sxs-lookup"><span data-stu-id="93489-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93489-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93489-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93489-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93489-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93489-153">响应</span><span class="sxs-lookup"><span data-stu-id="93489-153">Response</span></span>

> <span data-ttu-id="93489-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="93489-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="93489-155">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="93489-155">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="93489-156">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="93489-156">Notification - transfer accepted</span></span>

> <span data-ttu-id="93489-157">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="93489-157">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="93489-158">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="93489-158">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="93489-159">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="93489-159">Notification - transfer failed</span></span>

> <span data-ttu-id="93489-160">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="93489-160">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="93489-161">示例 2：咨询转接</span><span class="sxs-lookup"><span data-stu-id="93489-161">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="93489-162">请求</span><span class="sxs-lookup"><span data-stu-id="93489-162">Request</span></span>
<span data-ttu-id="93489-163">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="93489-163">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93489-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="93489-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-2"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="93489-165">C#</span><span class="sxs-lookup"><span data-stu-id="93489-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93489-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93489-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93489-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93489-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93489-168">响应</span><span class="sxs-lookup"><span data-stu-id="93489-168">Response</span></span>

> <span data-ttu-id="93489-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="93489-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="93489-170">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="93489-170">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="93489-171">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="93489-171">Notification - transfer accepted</span></span>

> <span data-ttu-id="93489-172">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="93489-172">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="93489-173">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="93489-173">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="93489-174">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="93489-174">Notification - transfer failed</span></span>

> <span data-ttu-id="93489-175">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="93489-175">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="93489-176">示例 3：呼叫转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="93489-176">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="93489-177">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="93489-177">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="93489-178">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="93489-178">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="93489-179">**注意：电话** ID 是 E.164 格式的电话号码。</span><span class="sxs-lookup"><span data-stu-id="93489-179">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="93489-180">请求</span><span class="sxs-lookup"><span data-stu-id="93489-180">Request</span></span>
<span data-ttu-id="93489-181">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="93489-181">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93489-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="93489-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-3"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/transfer
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="93489-183">C#</span><span class="sxs-lookup"><span data-stu-id="93489-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93489-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93489-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93489-185">响应</span><span class="sxs-lookup"><span data-stu-id="93489-185">Response</span></span>

> <span data-ttu-id="93489-186">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="93489-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="93489-187">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="93489-187">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="93489-188">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="93489-188">Notification - transfer accepted</span></span>

> <span data-ttu-id="93489-189">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="93489-189">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="93489-190">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="93489-190">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="93489-191">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="93489-191">Notification - transfer failed</span></span>

> <span data-ttu-id="93489-192">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="93489-192">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="93489-193">示例 4：咨询转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="93489-193">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="93489-194">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="93489-194">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="93489-195">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="93489-195">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="93489-196">**注意：电话** ID 是 E.164 格式的电话号码。</span><span class="sxs-lookup"><span data-stu-id="93489-196">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="93489-197">请求</span><span class="sxs-lookup"><span data-stu-id="93489-197">Request</span></span>
<span data-ttu-id="93489-198">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="93489-198">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93489-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="93489-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-4"
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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="93489-200">C#</span><span class="sxs-lookup"><span data-stu-id="93489-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93489-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93489-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93489-202">响应</span><span class="sxs-lookup"><span data-stu-id="93489-202">Response</span></span>

> <span data-ttu-id="93489-203">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="93489-203">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="93489-204">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="93489-204">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="93489-205">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="93489-205">Notification - transfer accepted</span></span>

> <span data-ttu-id="93489-206">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="93489-206">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="93489-207">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="93489-207">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="93489-208">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="93489-208">Notification - transfer failed</span></span>

> <span data-ttu-id="93489-209">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="93489-209">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


