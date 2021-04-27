---
title: participant： configureMixer
description: 配置多方对话中不同参与者的音频混合方式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9b8efa45be5163e088bef06e2d71959e80cae58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037912"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="9244f-103">participant： configureMixer</span><span class="sxs-lookup"><span data-stu-id="9244f-103">participant: configureMixer</span></span>

<span data-ttu-id="9244f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9244f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9244f-105">配置多方对话中不同参与者的音频混合方式。</span><span class="sxs-lookup"><span data-stu-id="9244f-105">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9244f-106">权限</span><span class="sxs-lookup"><span data-stu-id="9244f-106">Permissions</span></span>
<span data-ttu-id="9244f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9244f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9244f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9244f-109">Permission type</span></span> | <span data-ttu-id="9244f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9244f-110">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="9244f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9244f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9244f-112">不支持</span><span class="sxs-lookup"><span data-stu-id="9244f-112">Not Supported</span></span>        |
| <span data-ttu-id="9244f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9244f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9244f-114">不支持</span><span class="sxs-lookup"><span data-stu-id="9244f-114">Not Supported</span></span>        |
| <span data-ttu-id="9244f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9244f-115">Application</span></span>     | <span data-ttu-id="9244f-116">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="9244f-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9244f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9244f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /communications/calls/{id}/participants/configureMixer
```
> <span data-ttu-id="9244f-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="9244f-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="9244f-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="9244f-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9244f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9244f-120">Request headers</span></span>
| <span data-ttu-id="9244f-121">名称</span><span class="sxs-lookup"><span data-stu-id="9244f-121">Name</span></span>          | <span data-ttu-id="9244f-122">说明</span><span class="sxs-lookup"><span data-stu-id="9244f-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9244f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9244f-123">Authorization</span></span> | <span data-ttu-id="9244f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9244f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9244f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9244f-126">Request body</span></span>
<span data-ttu-id="9244f-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9244f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9244f-128">参数</span><span class="sxs-lookup"><span data-stu-id="9244f-128">Parameter</span></span>      | <span data-ttu-id="9244f-129">类型</span><span class="sxs-lookup"><span data-stu-id="9244f-129">Type</span></span>    |<span data-ttu-id="9244f-130">说明</span><span class="sxs-lookup"><span data-stu-id="9244f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9244f-131">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="9244f-131">participantMixerLevels</span></span>|<span data-ttu-id="9244f-132">[participantMixerLevel](../resources/participantmixerlevel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9244f-132">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="9244f-133">给定音频参与者的调频器级别配置。</span><span class="sxs-lookup"><span data-stu-id="9244f-133">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="9244f-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="9244f-134">clientContext</span></span>|<span data-ttu-id="9244f-135">String</span><span class="sxs-lookup"><span data-stu-id="9244f-135">String</span></span>|<span data-ttu-id="9244f-136">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="9244f-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="9244f-137">响应</span><span class="sxs-lookup"><span data-stu-id="9244f-137">Response</span></span>
<span data-ttu-id="9244f-138">返回 `202 Accepted` 响应代码和具有为此请求创建的 [commsOperation](../resources/commsoperation.md) 的 uri 的位置标头。</span><span class="sxs-lookup"><span data-stu-id="9244f-138">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="9244f-139">示例</span><span class="sxs-lookup"><span data-stu-id="9244f-139">Example</span></span>
<span data-ttu-id="9244f-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9244f-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9244f-141">请求</span><span class="sxs-lookup"><span data-stu-id="9244f-141">Request</span></span>
<span data-ttu-id="9244f-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9244f-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9244f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9244f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/configureMixer
Content-Type: application/json
Content-Length: 501

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "participantMixerLevels": [
    {
      "participant": "550fae72-d251-43ec-868c-373732c2704f",
      "exclusive": true,
      "ducking": {
        "rampActive": 50,
        "rampInactive": 50,
        "lowerLevel": 10,
        "upperLevel": 50
      },
      "sourceLevels": [
        {
          "participant": "632899f8-2ea1-4604-8413-27bd2892079f",
          "level": 50,
          "duckOthers": false
        }
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9244f-144">C#</span><span class="sxs-lookup"><span data-stu-id="9244f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9244f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9244f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9244f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9244f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9244f-147">响应</span><span class="sxs-lookup"><span data-stu-id="9244f-147">Response</span></span>

> <span data-ttu-id="9244f-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9244f-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "participant-configureMixer",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "running"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="9244f-149">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="9244f-149">Notification - operation completed</span></span>

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
      "@odata.type": "#microsoft.graph.commsOperation",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "@odata.etag": "W/\"1\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
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
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


