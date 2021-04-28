---
title: call： subscribeToTone
description: 订阅 DTMF (双音多频信号) 。 这允许你在用户按下"Dialpad"上的键时收到通知。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: bca2ba67be2f62f87c84390a5a1bc3a2799e9498
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051597"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="54bb7-104">call： subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="54bb7-104">call: subscribeToTone</span></span>

<span data-ttu-id="54bb7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54bb7-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="54bb7-106">订阅 DTMF (双音多频信号) 。</span><span class="sxs-lookup"><span data-stu-id="54bb7-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="54bb7-107">这允许你在用户按下"拨号盘"上的键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="54bb7-107">This allows you to be notified when the user presses keys on a "dialpad".</span></span>

> [!Note]
> <span data-ttu-id="54bb7-108">**subscribeToTone** 操作仅支持 [通过](../resources/call.md) [serviceHostedMediaConfig 启动的呼叫](../resources/servicehostedmediaconfig.md)。</span><span class="sxs-lookup"><span data-stu-id="54bb7-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="54bb7-109">权限</span><span class="sxs-lookup"><span data-stu-id="54bb7-109">Permissions</span></span>
<span data-ttu-id="54bb7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54bb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54bb7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="54bb7-112">Permission type</span></span> | <span data-ttu-id="54bb7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54bb7-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="54bb7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54bb7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="54bb7-115">不支持</span><span class="sxs-lookup"><span data-stu-id="54bb7-115">Not Supported</span></span>        |
| <span data-ttu-id="54bb7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54bb7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54bb7-117">不支持</span><span class="sxs-lookup"><span data-stu-id="54bb7-117">Not Supported</span></span>        |
| <span data-ttu-id="54bb7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="54bb7-118">Application</span></span>     | <span data-ttu-id="54bb7-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="54bb7-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="54bb7-120">**注意：** 提供的任何音调数据可能无法保留。</span><span class="sxs-lookup"><span data-stu-id="54bb7-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="54bb7-121">确保你遵守有关通信数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="54bb7-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="54bb7-122">有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="54bb7-122">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="http-request"></a><span data-ttu-id="54bb7-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54bb7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="54bb7-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="54bb7-124">Request headers</span></span>
| <span data-ttu-id="54bb7-125">名称</span><span class="sxs-lookup"><span data-stu-id="54bb7-125">Name</span></span>          | <span data-ttu-id="54bb7-126">说明</span><span class="sxs-lookup"><span data-stu-id="54bb7-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="54bb7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="54bb7-127">Authorization</span></span> | <span data-ttu-id="54bb7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54bb7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54bb7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="54bb7-130">Request body</span></span>
<span data-ttu-id="54bb7-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="54bb7-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="54bb7-132">参数</span><span class="sxs-lookup"><span data-stu-id="54bb7-132">Parameter</span></span>      | <span data-ttu-id="54bb7-133">类型</span><span class="sxs-lookup"><span data-stu-id="54bb7-133">Type</span></span>    | <span data-ttu-id="54bb7-134">说明</span><span class="sxs-lookup"><span data-stu-id="54bb7-134">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="54bb7-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="54bb7-135">clientContext</span></span>  | <span data-ttu-id="54bb7-136">String</span><span class="sxs-lookup"><span data-stu-id="54bb7-136">String</span></span>  | <span data-ttu-id="54bb7-137">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="54bb7-137">Unique client context string.</span></span> <span data-ttu-id="54bb7-138">最多可包含 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="54bb7-138">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="54bb7-139">响应</span><span class="sxs-lookup"><span data-stu-id="54bb7-139">Response</span></span>
<span data-ttu-id="54bb7-140">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="54bb7-140">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="54bb7-141">示例</span><span class="sxs-lookup"><span data-stu-id="54bb7-141">Example</span></span>
<span data-ttu-id="54bb7-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="54bb7-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="54bb7-143">请求</span><span class="sxs-lookup"><span data-stu-id="54bb7-143">Request</span></span>
<span data-ttu-id="54bb7-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="54bb7-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54bb7-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="54bb7-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="c"></a>[<span data-ttu-id="54bb7-146">C#</span><span class="sxs-lookup"><span data-stu-id="54bb7-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54bb7-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54bb7-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54bb7-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54bb7-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54bb7-149">Java</span><span class="sxs-lookup"><span data-stu-id="54bb7-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="54bb7-150">响应</span><span class="sxs-lookup"><span data-stu-id="54bb7-150">Response</span></span>

> <span data-ttu-id="54bb7-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="54bb7-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-subscribeToTone",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "completed"
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="54bb7-152">Notification - 音调通知</span><span class="sxs-lookup"><span data-stu-id="54bb7-152">Notification - tone notification</span></span>

<span data-ttu-id="54bb7-153">通知包含 [toneinfo](../resources/toneinfo.md) 资源中按下的音调的信息。</span><span class="sxs-lookup"><span data-stu-id="54bb7-153">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "toneInfo": {
          "@odata.type": "#microsoft.graph.toneInfo",
          "sequenceId": 1,
          "tone": "tone1"
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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
