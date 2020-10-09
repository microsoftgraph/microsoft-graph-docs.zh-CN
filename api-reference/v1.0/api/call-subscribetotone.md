---
title: 调用： subscribeToTone
description: 订阅 DTMF (双音多频信号) 。 这样，您就可以在用户按 "Dialpad" 上的键时收到通知。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 93c5c5c7bd7b04baa70af9fffd2c7319f50af4ad
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404341"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="58da9-104">调用： subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="58da9-104">call: subscribeToTone</span></span>

<span data-ttu-id="58da9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58da9-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="58da9-106">订阅 DTMF (双音多频信号) 。</span><span class="sxs-lookup"><span data-stu-id="58da9-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="58da9-107">这样，您就可以在用户按 "dialpad" 上的键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="58da9-107">This allows you to be notified when the user presses keys on a "dialpad".</span></span>

> [!Note]
> <span data-ttu-id="58da9-108">仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持**subscribeToTone**操作。</span><span class="sxs-lookup"><span data-stu-id="58da9-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="58da9-109">权限</span><span class="sxs-lookup"><span data-stu-id="58da9-109">Permissions</span></span>
<span data-ttu-id="58da9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58da9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58da9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="58da9-112">Permission type</span></span> | <span data-ttu-id="58da9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58da9-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="58da9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58da9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="58da9-115">不支持</span><span class="sxs-lookup"><span data-stu-id="58da9-115">Not Supported</span></span>        |
| <span data-ttu-id="58da9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58da9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58da9-117">不支持</span><span class="sxs-lookup"><span data-stu-id="58da9-117">Not Supported</span></span>        |
| <span data-ttu-id="58da9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="58da9-118">Application</span></span>     | <span data-ttu-id="58da9-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="58da9-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="58da9-120">**注意：** 提供的任何音调数据不能持久化。</span><span class="sxs-lookup"><span data-stu-id="58da9-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="58da9-121">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="58da9-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="58da9-122">有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="58da9-122">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="http-request"></a><span data-ttu-id="58da9-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58da9-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="58da9-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="58da9-124">Request headers</span></span>
| <span data-ttu-id="58da9-125">名称</span><span class="sxs-lookup"><span data-stu-id="58da9-125">Name</span></span>          | <span data-ttu-id="58da9-126">说明</span><span class="sxs-lookup"><span data-stu-id="58da9-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="58da9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="58da9-127">Authorization</span></span> | <span data-ttu-id="58da9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58da9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58da9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="58da9-130">Request body</span></span>
<span data-ttu-id="58da9-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="58da9-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58da9-132">参数</span><span class="sxs-lookup"><span data-stu-id="58da9-132">Parameter</span></span>      | <span data-ttu-id="58da9-133">类型</span><span class="sxs-lookup"><span data-stu-id="58da9-133">Type</span></span>    | <span data-ttu-id="58da9-134">说明</span><span class="sxs-lookup"><span data-stu-id="58da9-134">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="58da9-135">适用</span><span class="sxs-lookup"><span data-stu-id="58da9-135">clientContext</span></span>  | <span data-ttu-id="58da9-136">字符串</span><span class="sxs-lookup"><span data-stu-id="58da9-136">String</span></span>  | <span data-ttu-id="58da9-137">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="58da9-137">Unique client context string.</span></span> <span data-ttu-id="58da9-138">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="58da9-138">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="58da9-139">响应</span><span class="sxs-lookup"><span data-stu-id="58da9-139">Response</span></span>
<span data-ttu-id="58da9-140">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="58da9-140">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="58da9-141">示例</span><span class="sxs-lookup"><span data-stu-id="58da9-141">Example</span></span>
<span data-ttu-id="58da9-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="58da9-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="58da9-143">请求</span><span class="sxs-lookup"><span data-stu-id="58da9-143">Request</span></span>
<span data-ttu-id="58da9-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="58da9-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="58da9-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="58da9-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="58da9-146">C#</span><span class="sxs-lookup"><span data-stu-id="58da9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58da9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58da9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58da9-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58da9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58da9-149">Java</span><span class="sxs-lookup"><span data-stu-id="58da9-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="58da9-150">响应</span><span class="sxs-lookup"><span data-stu-id="58da9-150">Response</span></span>

> <span data-ttu-id="58da9-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="58da9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


##### <a name="notification---tone-notification"></a><span data-ttu-id="58da9-153">通知-音调通知</span><span class="sxs-lookup"><span data-stu-id="58da9-153">Notification - tone notification</span></span>

<span data-ttu-id="58da9-154">通知包含 [toneinfo](../resources/toneinfo.md) 资源中所按音调的信息。</span><span class="sxs-lookup"><span data-stu-id="58da9-154">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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