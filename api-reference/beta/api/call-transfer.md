---
title: call： transfer
description: 转接活动对等呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7c23ea17f1bc68b88490d8a54a68e50fe0604a78
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719774"
---
# <a name="call-transfer"></a><span data-ttu-id="6cf8c-103">call： transfer</span><span class="sxs-lookup"><span data-stu-id="6cf8c-103">call: transfer</span></span>

<span data-ttu-id="6cf8c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cf8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cf8c-105">转接活动对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="6cf8c-106">**注意：** 只有当被转移方和转移目标都是属于同一租户的 Microsoft Teams 用户时，才支持此操作。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="6cf8c-107">仅应用程序实例支持转移到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="6cf8c-108">若要了解有关转移方、被转移方和转移目标有关详细信息，请参阅[RFC 5589。](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="6cf8c-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="6cf8c-109">咨询转接意味着，在转接之前，转接人可以通知要 (转接) 转接给被叫方。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="6cf8c-110">这与直接转移呼叫相反。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cf8c-111">权限</span><span class="sxs-lookup"><span data-stu-id="6cf8c-111">Permissions</span></span>
<span data-ttu-id="6cf8c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cf8c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cf8c-114">Permission type</span></span> | <span data-ttu-id="6cf8c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cf8c-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="6cf8c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cf8c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cf8c-117">不支持</span><span class="sxs-lookup"><span data-stu-id="6cf8c-117">Not Supported</span></span>                |
| <span data-ttu-id="6cf8c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cf8c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cf8c-119">不支持</span><span class="sxs-lookup"><span data-stu-id="6cf8c-119">Not Supported</span></span>                |
| <span data-ttu-id="6cf8c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cf8c-120">Application</span></span>     | <span data-ttu-id="6cf8c-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="6cf8c-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="6cf8c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cf8c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="6cf8c-123">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6cf8c-124">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cf8c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cf8c-125">Request headers</span></span>
| <span data-ttu-id="6cf8c-126">名称</span><span class="sxs-lookup"><span data-stu-id="6cf8c-126">Name</span></span>          | <span data-ttu-id="6cf8c-127">说明</span><span class="sxs-lookup"><span data-stu-id="6cf8c-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6cf8c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cf8c-128">Authorization</span></span> | <span data-ttu-id="6cf8c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cf8c-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="6cf8c-131">Content-type</span></span>  | <span data-ttu-id="6cf8c-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6cf8c-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cf8c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cf8c-134">Request body</span></span>
<span data-ttu-id="6cf8c-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cf8c-136">参数</span><span class="sxs-lookup"><span data-stu-id="6cf8c-136">Parameter</span></span>      | <span data-ttu-id="6cf8c-137">类型</span><span class="sxs-lookup"><span data-stu-id="6cf8c-137">Type</span></span>    |<span data-ttu-id="6cf8c-138">说明</span><span class="sxs-lookup"><span data-stu-id="6cf8c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cf8c-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="6cf8c-139">transferTarget</span></span>|[<span data-ttu-id="6cf8c-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="6cf8c-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="6cf8c-141">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="6cf8c-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="6cf8c-142">clientContext</span></span>|<span data-ttu-id="6cf8c-143">String</span><span class="sxs-lookup"><span data-stu-id="6cf8c-143">String</span></span>|<span data-ttu-id="6cf8c-144">唯一客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-144">Unique Client Context string.</span></span> <span data-ttu-id="6cf8c-145">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="6cf8c-146">响应</span><span class="sxs-lookup"><span data-stu-id="6cf8c-146">Response</span></span>
<span data-ttu-id="6cf8c-147">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6cf8c-148">示例</span><span class="sxs-lookup"><span data-stu-id="6cf8c-148">Examples</span></span>
<span data-ttu-id="6cf8c-149">这些示例显示了传入呼叫到不同类型的传输通知的流。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="6cf8c-150">示例 1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="6cf8c-150">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="6cf8c-151">请求</span><span class="sxs-lookup"><span data-stu-id="6cf8c-151">Request</span></span>
<span data-ttu-id="6cf8c-152">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6cf8c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf8c-153">HTTP</span></span>](#tab/http)
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
    "region": "region-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="c"></a>[<span data-ttu-id="6cf8c-154">C#</span><span class="sxs-lookup"><span data-stu-id="6cf8c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cf8c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cf8c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cf8c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cf8c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6cf8c-157">响应</span><span class="sxs-lookup"><span data-stu-id="6cf8c-157">Response</span></span>

> <span data-ttu-id="6cf8c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6cf8c-160">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="6cf8c-160">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6cf8c-161">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="6cf8c-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="6cf8c-162">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6cf8c-163">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="6cf8c-163">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="6cf8c-164">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="6cf8c-164">Notification - transfer failed</span></span>

> <span data-ttu-id="6cf8c-165">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="6cf8c-166">示例 2：咨询转接</span><span class="sxs-lookup"><span data-stu-id="6cf8c-166">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="6cf8c-167">请求</span><span class="sxs-lookup"><span data-stu-id="6cf8c-167">Request</span></span>
<span data-ttu-id="6cf8c-168">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-168">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6cf8c-169">响应</span><span class="sxs-lookup"><span data-stu-id="6cf8c-169">Response</span></span>

> <span data-ttu-id="6cf8c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6cf8c-172">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="6cf8c-172">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6cf8c-173">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="6cf8c-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="6cf8c-174">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6cf8c-175">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="6cf8c-175">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="6cf8c-176">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="6cf8c-176">Notification - transfer failed</span></span>

> <span data-ttu-id="6cf8c-177">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="6cf8c-178">示例 3：呼叫转移到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="6cf8c-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="6cf8c-179">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-179">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="6cf8c-180">步骤 1：创建应用程序实例</span><span class="sxs-lookup"><span data-stu-id="6cf8c-180">Step 1: Create application instance</span></span>
<span data-ttu-id="6cf8c-181">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet 以创建应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-181">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="6cf8c-182">有关详细信息，请参阅 [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-182">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="6cf8c-183">步骤 2：分配 Microsoft 365 许可证</span><span class="sxs-lookup"><span data-stu-id="6cf8c-183">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="6cf8c-184">使用租户管理员凭据登录并转到"用户 https://admin.microsoft.com/ **->活动用户"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-184">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="6cf8c-185">选择应用程序实例，分配 **Microsoft 365 国内和国际** 通话套餐和 **Microsoft 365 电话系统 - 虚拟用户** 许可证，然后单击"**保存更改"。**</span><span class="sxs-lookup"><span data-stu-id="6cf8c-185">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="6cf8c-186">如果所需的许可证在租户中不可用，可以从"计费-> **购买服务"** 选项卡获取它们。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-186">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="6cf8c-187">步骤 3：获取 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="6cf8c-187">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="6cf8c-188">使用租户管理员凭据登录并单击左侧面板上的"旧版 https://admin.teams.microsoft.com/ 门户"选项卡。 </span><span class="sxs-lookup"><span data-stu-id="6cf8c-188">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="6cf8c-189">In the new page， go to the **voice -> phone numbers** tab.</span><span class="sxs-lookup"><span data-stu-id="6cf8c-189">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="6cf8c-190">单击 **+** 该按钮， **选择"新建服务号码**"，然后转到 **"添加新服务号码"** 页。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-190">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="6cf8c-191">选择 **"国家/地区\*\*\*\*"、"省/地区**"、"**城市**"和"输入 **数量**"，然后单击 **"添加**"进行搜索。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-191">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="6cf8c-192">单击 **获取号码**。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-192">Click **acquire numbers**.</span></span> <span data-ttu-id="6cf8c-193">新获取的号码会显示在 **电话号码选项卡** 上。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-193">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="6cf8c-194">步骤 4：将 PSTN 号码分配给应用程序实例</span><span class="sxs-lookup"><span data-stu-id="6cf8c-194">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="6cf8c-195">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet，将 PSTN 号码分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-195">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="6cf8c-196">有关详细信息，请参阅 [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-196">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
> <span data-ttu-id="6cf8c-197">**注意：** 如果租户具有分配给任何应用程序实例的澳大利亚 PSTN 号码，则此呼叫可能会失败。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-197">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might fail.</span></span> <span data-ttu-id="6cf8c-198">如果租户是新创建的，可能需要几天时间，此功能可用。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-198">If a tenant is newly created, it might take several days for this feature to be available.</span></span>

#### <a name="request"></a><span data-ttu-id="6cf8c-199">请求</span><span class="sxs-lookup"><span data-stu-id="6cf8c-199">Request</span></span>
<span data-ttu-id="6cf8c-200">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-200">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6cf8c-201">响应</span><span class="sxs-lookup"><span data-stu-id="6cf8c-201">Response</span></span>

> <span data-ttu-id="6cf8c-p115">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6cf8c-204">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="6cf8c-204">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6cf8c-205">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="6cf8c-205">Notification - transfer accepted</span></span>

> <span data-ttu-id="6cf8c-206">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-206">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6cf8c-207">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="6cf8c-207">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="6cf8c-208">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="6cf8c-208">Notification - transfer failed</span></span>

> <span data-ttu-id="6cf8c-209">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-209">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="6cf8c-210">示例 4：咨询转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="6cf8c-210">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="6cf8c-211">此呼叫需要分配有 PSTN 号码的应用程序实例，如示例 3 中所述。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-211">This call requires an application instance with PSTN number assigned, as described in Example 3.</span></span>

> <span data-ttu-id="6cf8c-212">**注意：** 如果租户向任何应用程序实例分配了澳大利亚 PSTN 号码，则此呼叫可能会失败。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-212">**Note:** This call may fail if a tenant has Australian PSTN numbers assigned to any application instances.</span></span> <span data-ttu-id="6cf8c-213">如果租户是新创建的，可能需要几天时间，此功能可用。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-213">If a tenant is newly created, it might take several days for this feature to be available.</span></span>


#### <a name="request"></a><span data-ttu-id="6cf8c-214">请求</span><span class="sxs-lookup"><span data-stu-id="6cf8c-214">Request</span></span>
<span data-ttu-id="6cf8c-215">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-215">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6cf8c-216">响应</span><span class="sxs-lookup"><span data-stu-id="6cf8c-216">Response</span></span>

> <span data-ttu-id="6cf8c-p117">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-p117">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6cf8c-219">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="6cf8c-219">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6cf8c-220">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="6cf8c-220">Notification - transfer accepted</span></span>

> <span data-ttu-id="6cf8c-221">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-221">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6cf8c-222">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="6cf8c-222">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="6cf8c-223">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="6cf8c-223">Notification - transfer failed</span></span>

> <span data-ttu-id="6cf8c-224">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="6cf8c-224">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


