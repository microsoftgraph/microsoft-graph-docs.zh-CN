---
title: call： transfer
description: 转接活动对等呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b8186913aa54afc02266216666d82bce28568fc4
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177233"
---
# <a name="call-transfer"></a><span data-ttu-id="d4f8f-103">call： transfer</span><span class="sxs-lookup"><span data-stu-id="d4f8f-103">call: transfer</span></span>

<span data-ttu-id="d4f8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4f8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4f8f-105">转接活动对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="d4f8f-106">**注意：** 只有当被转移方和转移目标都是属于同一租户的 Microsoft Teams 用户时，才支持此操作。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="d4f8f-107">不支持转移到 PSTN 号码。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-107">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="d4f8f-108">若要了解有关转移方、被转移方和转移目标有关详细信息，请参阅[RFC 5589。](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="d4f8f-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="d4f8f-109">咨询转接意味着，在转接之前，转接人可以通知要 (转接) 转接给被叫方。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="d4f8f-110">这与直接转移呼叫相反。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4f8f-111">权限</span><span class="sxs-lookup"><span data-stu-id="d4f8f-111">Permissions</span></span>
<span data-ttu-id="d4f8f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4f8f-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4f8f-114">Permission type</span></span> | <span data-ttu-id="d4f8f-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4f8f-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="d4f8f-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4f8f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4f8f-117">不支持</span><span class="sxs-lookup"><span data-stu-id="d4f8f-117">Not Supported</span></span>                |
| <span data-ttu-id="d4f8f-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4f8f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4f8f-119">不支持</span><span class="sxs-lookup"><span data-stu-id="d4f8f-119">Not Supported</span></span>                |
| <span data-ttu-id="d4f8f-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4f8f-120">Application</span></span>     | <span data-ttu-id="d4f8f-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="d4f8f-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="d4f8f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4f8f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="d4f8f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4f8f-123">Request headers</span></span>
| <span data-ttu-id="d4f8f-124">名称</span><span class="sxs-lookup"><span data-stu-id="d4f8f-124">Name</span></span>          | <span data-ttu-id="d4f8f-125">说明</span><span class="sxs-lookup"><span data-stu-id="d4f8f-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d4f8f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4f8f-126">Authorization</span></span> | <span data-ttu-id="d4f8f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4f8f-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="d4f8f-129">Content-type</span></span>  | <span data-ttu-id="d4f8f-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4f8f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4f8f-132">Request body</span></span>
<span data-ttu-id="d4f8f-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4f8f-134">参数</span><span class="sxs-lookup"><span data-stu-id="d4f8f-134">Parameter</span></span>      | <span data-ttu-id="d4f8f-135">类型</span><span class="sxs-lookup"><span data-stu-id="d4f8f-135">Type</span></span>    |<span data-ttu-id="d4f8f-136">说明</span><span class="sxs-lookup"><span data-stu-id="d4f8f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4f8f-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="d4f8f-137">transferTarget</span></span>|[<span data-ttu-id="d4f8f-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="d4f8f-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="d4f8f-139">作为转移目标的参与者。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-139">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="d4f8f-140">clientContext</span><span class="sxs-lookup"><span data-stu-id="d4f8f-140">clientContext</span></span>|<span data-ttu-id="d4f8f-141">String</span><span class="sxs-lookup"><span data-stu-id="d4f8f-141">String</span></span>|<span data-ttu-id="d4f8f-142">唯一客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-142">Unique Client Context string.</span></span> <span data-ttu-id="d4f8f-143">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-143">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="d4f8f-144">响应</span><span class="sxs-lookup"><span data-stu-id="d4f8f-144">Response</span></span>
<span data-ttu-id="d4f8f-145">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-145">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d4f8f-146">示例</span><span class="sxs-lookup"><span data-stu-id="d4f8f-146">Examples</span></span>
<span data-ttu-id="d4f8f-147">这些示例显示了传入呼叫到不同类型的传输通知的流。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-147">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="d4f8f-148">示例 1：呼叫转移</span><span class="sxs-lookup"><span data-stu-id="d4f8f-148">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="d4f8f-149">请求</span><span class="sxs-lookup"><span data-stu-id="d4f8f-149">Request</span></span>
<span data-ttu-id="d4f8f-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d4f8f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4f8f-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4f8f-152">C#</span><span class="sxs-lookup"><span data-stu-id="d4f8f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4f8f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4f8f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4f8f-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4f8f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4f8f-155">Java</span><span class="sxs-lookup"><span data-stu-id="d4f8f-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d4f8f-156">响应</span><span class="sxs-lookup"><span data-stu-id="d4f8f-156">Response</span></span>

> <span data-ttu-id="d4f8f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="d4f8f-159">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="d4f8f-159">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="d4f8f-160">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="d4f8f-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="d4f8f-161">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="d4f8f-162">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="d4f8f-162">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="d4f8f-163">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="d4f8f-163">Notification - transfer failed</span></span>

> <span data-ttu-id="d4f8f-164">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="d4f8f-165">示例 2：咨询转接</span><span class="sxs-lookup"><span data-stu-id="d4f8f-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="d4f8f-166">请求</span><span class="sxs-lookup"><span data-stu-id="d4f8f-166">Request</span></span>
<span data-ttu-id="d4f8f-167">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-167">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="d4f8f-168">响应</span><span class="sxs-lookup"><span data-stu-id="d4f8f-168">Response</span></span>

> <span data-ttu-id="d4f8f-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="d4f8f-171">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="d4f8f-171">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="d4f8f-172">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="d4f8f-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="d4f8f-173">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="d4f8f-174">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="d4f8f-174">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="d4f8f-175">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="d4f8f-175">Notification - transfer failed</span></span>

> <span data-ttu-id="d4f8f-176">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="d4f8f-177">示例 3：呼叫转移到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="d4f8f-177">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="d4f8f-178">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-178">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="d4f8f-179">步骤 1：创建应用程序实例</span><span class="sxs-lookup"><span data-stu-id="d4f8f-179">Step 1: Create application instance</span></span>
<span data-ttu-id="d4f8f-180">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet 以创建应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-180">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="d4f8f-181">有关详细信息，请参阅 [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-181">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="d4f8f-182">步骤 2：分配 Microsoft 365 许可证</span><span class="sxs-lookup"><span data-stu-id="d4f8f-182">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="d4f8f-183">使用租户管理员凭据登录并转到"用户 https://admin.microsoft.com/ **->活动用户"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-183">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="d4f8f-184">选择应用程序实例，分配 **Microsoft 365 国内和国际** 通话套餐和 **Microsoft 365 电话系统 - 虚拟用户** 许可证，然后单击"**保存更改"。**</span><span class="sxs-lookup"><span data-stu-id="d4f8f-184">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="d4f8f-185">如果所需的许可证在租户中不可用，可以从"计费-> **购买服务"** 选项卡获取它们。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-185">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="d4f8f-186">步骤 3：获取 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="d4f8f-186">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="d4f8f-187">使用租户管理员凭据登录并单击左侧面板上的"旧版 https://admin.teams.microsoft.com/ 门户"选项卡。 </span><span class="sxs-lookup"><span data-stu-id="d4f8f-187">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="d4f8f-188">In the new page， go to the **voice -> phone numbers** tab.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-188">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="d4f8f-189">单击 **+** 该按钮， **选择"新建服务号码**"，然后转到 **"添加新服务号码"** 页。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-189">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="d4f8f-190">选择 **"国家/地区\*\*\*\*"、"省/地区**"、"**城市**"和"输入 **数量**"，然后单击 **"添加**"进行搜索。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-190">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="d4f8f-191">单击 **获取号码**。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-191">Click **acquire numbers**.</span></span> <span data-ttu-id="d4f8f-192">新获取的号码会显示在 **电话号码选项卡** 上。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-192">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="d4f8f-193">步骤 4：将 PSTN 号码分配给应用程序实例</span><span class="sxs-lookup"><span data-stu-id="d4f8f-193">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="d4f8f-194">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet，将 PSTN 号码分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-194">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="d4f8f-195">有关详细信息，请参阅 [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-195">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="d4f8f-196">请求</span><span class="sxs-lookup"><span data-stu-id="d4f8f-196">Request</span></span>
<span data-ttu-id="d4f8f-197">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-197">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d4f8f-198">响应</span><span class="sxs-lookup"><span data-stu-id="d4f8f-198">Response</span></span>

> <span data-ttu-id="d4f8f-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="d4f8f-201">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="d4f8f-201">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="d4f8f-202">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="d4f8f-202">Notification - transfer accepted</span></span>

> <span data-ttu-id="d4f8f-203">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-203">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="d4f8f-204">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="d4f8f-204">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="d4f8f-205">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="d4f8f-205">Notification - transfer failed</span></span>

> <span data-ttu-id="d4f8f-206">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-206">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="d4f8f-207">示例 4：咨询转接到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="d4f8f-207">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="d4f8f-208">此呼叫需要分配有 PSTN 号码的应用程序实例，如示例 3 中所述。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-208">This call requires an application instance with PSTN number assigned, as described in Example 3.</span></span>

#### <a name="request"></a><span data-ttu-id="d4f8f-209">请求</span><span class="sxs-lookup"><span data-stu-id="d4f8f-209">Request</span></span>
<span data-ttu-id="d4f8f-210">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-210">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d4f8f-211">响应</span><span class="sxs-lookup"><span data-stu-id="d4f8f-211">Response</span></span>

> <span data-ttu-id="d4f8f-p114">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="d4f8f-214">通知 - 传输</span><span class="sxs-lookup"><span data-stu-id="d4f8f-214">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="d4f8f-215">通知 - 接受转移</span><span class="sxs-lookup"><span data-stu-id="d4f8f-215">Notification - transfer accepted</span></span>

> <span data-ttu-id="d4f8f-216">**注意：** 接受的传输可能在媒体状态音频处于非活动状态之后或之前发生。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-216">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="d4f8f-217">通知 - 传输已完成</span><span class="sxs-lookup"><span data-stu-id="d4f8f-217">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="d4f8f-218">通知 - 转移失败</span><span class="sxs-lookup"><span data-stu-id="d4f8f-218">Notification - transfer failed</span></span>

> <span data-ttu-id="d4f8f-219">**注意：** 当呼叫转移失败时，呼叫状态将为 `established` 。</span><span class="sxs-lookup"><span data-stu-id="d4f8f-219">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

