---
title: call： transfer
description: 转接活动对等呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f4be30fff38c639ac55d126b0501b3f9f57afa52
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948455"
---
# <a name="call-transfer"></a><span data-ttu-id="9e861-103">call： transfer</span><span class="sxs-lookup"><span data-stu-id="9e861-103">call: transfer</span></span>

<span data-ttu-id="9e861-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e861-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e861-105">转接活动对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="9e861-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="9e861-106">**注意：** 只有当被转移方和转移目标都是属于同一租户的 Microsoft Teams 用户时，才支持此操作。</span><span class="sxs-lookup"><span data-stu-id="9e861-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="9e861-107">仅应用程序实例支持转接到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="9e861-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="9e861-108">若要了解有关转移方、被转移方和转移目标有关详细信息，请参阅 [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2)。</span><span class="sxs-lookup"><span data-stu-id="9e861-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="9e861-109">咨询转接意味着在转接之前，转接人可以通知要呼叫 (转接) 转接给被叫方。</span><span class="sxs-lookup"><span data-stu-id="9e861-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="9e861-110">这与直接转移呼叫相反。</span><span class="sxs-lookup"><span data-stu-id="9e861-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e861-111">权限</span><span class="sxs-lookup"><span data-stu-id="9e861-111">Permissions</span></span>
<span data-ttu-id="9e861-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e861-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e861-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e861-114">Permission type</span></span> | <span data-ttu-id="9e861-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e861-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="9e861-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e861-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e861-117">不支持</span><span class="sxs-lookup"><span data-stu-id="9e861-117">Not Supported</span></span>                |
| <span data-ttu-id="9e861-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e861-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e861-119">不支持</span><span class="sxs-lookup"><span data-stu-id="9e861-119">Not Supported</span></span>                |
| <span data-ttu-id="9e861-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e861-120">Application</span></span>     | <span data-ttu-id="9e861-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="9e861-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="9e861-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e861-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="9e861-123">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="9e861-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="9e861-124">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="9e861-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e861-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e861-125">Request headers</span></span>
| <span data-ttu-id="9e861-126">名称</span><span class="sxs-lookup"><span data-stu-id="9e861-126">Name</span></span>          | <span data-ttu-id="9e861-127">说明</span><span class="sxs-lookup"><span data-stu-id="9e861-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9e861-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e861-128">Authorization</span></span> | <span data-ttu-id="9e861-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e861-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e861-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="9e861-131">Content-type</span></span>  | <span data-ttu-id="9e861-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9e861-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e861-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e861-134">Request body</span></span>
<span data-ttu-id="9e861-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9e861-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9e861-136">参数</span><span class="sxs-lookup"><span data-stu-id="9e861-136">Parameter</span></span>      | <span data-ttu-id="9e861-137">类型</span><span class="sxs-lookup"><span data-stu-id="9e861-137">Type</span></span>    |<span data-ttu-id="9e861-138">说明</span><span class="sxs-lookup"><span data-stu-id="9e861-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e861-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="9e861-139">transferTarget</span></span>|[<span data-ttu-id="9e861-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="9e861-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="9e861-141">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="9e861-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="9e861-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="9e861-142">clientContext</span></span>|<span data-ttu-id="9e861-143">String</span><span class="sxs-lookup"><span data-stu-id="9e861-143">String</span></span>|<span data-ttu-id="9e861-144">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="9e861-144">Unique Client Context string.</span></span> <span data-ttu-id="9e861-145">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="9e861-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="9e861-146">响应</span><span class="sxs-lookup"><span data-stu-id="9e861-146">Response</span></span>
<span data-ttu-id="9e861-147">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9e861-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9e861-148">示例</span><span class="sxs-lookup"><span data-stu-id="9e861-148">Examples</span></span>
<span data-ttu-id="9e861-149">这些示例显示传入呼叫一向到不同类型的转移通知的流。</span><span class="sxs-lookup"><span data-stu-id="9e861-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="9e861-150">示例 1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="9e861-150">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="9e861-151">请求</span><span class="sxs-lookup"><span data-stu-id="9e861-151">Request</span></span>
<span data-ttu-id="9e861-152">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e861-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e861-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e861-153">HTTP</span></span>](#tab/http)
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
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="c"></a>[<span data-ttu-id="9e861-154">C#</span><span class="sxs-lookup"><span data-stu-id="9e861-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e861-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e861-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e861-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e861-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e861-157">响应</span><span class="sxs-lookup"><span data-stu-id="9e861-157">Response</span></span>

> <span data-ttu-id="9e861-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9e861-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="9e861-160">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="9e861-160">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="9e861-161">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="9e861-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="9e861-162">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="9e861-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="9e861-163">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="9e861-163">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="9e861-164">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="9e861-164">Notification - transfer failed</span></span>

> <span data-ttu-id="9e861-165">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="9e861-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="9e861-166">示例 2：咨询转接</span><span class="sxs-lookup"><span data-stu-id="9e861-166">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="9e861-167">请求</span><span class="sxs-lookup"><span data-stu-id="9e861-167">Request</span></span>
<span data-ttu-id="9e861-168">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e861-168">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer-2"
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

#### <a name="response"></a><span data-ttu-id="9e861-169">响应</span><span class="sxs-lookup"><span data-stu-id="9e861-169">Response</span></span>

> <span data-ttu-id="9e861-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9e861-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="9e861-172">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="9e861-172">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="9e861-173">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="9e861-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="9e861-174">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="9e861-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="9e861-175">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="9e861-175">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="9e861-176">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="9e861-176">Notification - transfer failed</span></span>

> <span data-ttu-id="9e861-177">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="9e861-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="9e861-178">示例 3：呼叫转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="9e861-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="9e861-179">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="9e861-179">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="9e861-180">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="9e861-180">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="9e861-181">请求</span><span class="sxs-lookup"><span data-stu-id="9e861-181">Request</span></span>
<span data-ttu-id="9e861-182">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e861-182">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="9e861-183">响应</span><span class="sxs-lookup"><span data-stu-id="9e861-183">Response</span></span>

> <span data-ttu-id="9e861-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9e861-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="9e861-186">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="9e861-186">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="9e861-187">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="9e861-187">Notification - transfer accepted</span></span>

> <span data-ttu-id="9e861-188">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="9e861-188">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="9e861-189">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="9e861-189">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="9e861-190">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="9e861-190">Notification - transfer failed</span></span>

> <span data-ttu-id="9e861-191">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="9e861-191">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="9e861-192">示例 4：咨询转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="9e861-192">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="9e861-193">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="9e861-193">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="9e861-194">有关详细信息，请参阅 [将电话号码分配给自动程序](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="9e861-194">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="9e861-195">请求</span><span class="sxs-lookup"><span data-stu-id="9e861-195">Request</span></span>
<span data-ttu-id="9e861-196">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e861-196">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="9e861-197">响应</span><span class="sxs-lookup"><span data-stu-id="9e861-197">Response</span></span>

> <span data-ttu-id="9e861-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9e861-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="9e861-200">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="9e861-200">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="9e861-201">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="9e861-201">Notification - transfer accepted</span></span>

> <span data-ttu-id="9e861-202">**注意：** 接受的转移可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="9e861-202">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="9e861-203">通知 - 转移已完成</span><span class="sxs-lookup"><span data-stu-id="9e861-203">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="9e861-204">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="9e861-204">Notification - transfer failed</span></span>

> <span data-ttu-id="9e861-205">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="9e861-205">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


