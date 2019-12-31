---
title: 参与者： configureMixer
description: 为多方对话中的不同参与者配置音频的混合方式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d1aa61efeafe26dde904787bf723c8352594c424
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913126"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="54da3-103">参与者： configureMixer</span><span class="sxs-lookup"><span data-stu-id="54da3-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54da3-104">为多方对话中的不同参与者配置音频的混合方式。</span><span class="sxs-lookup"><span data-stu-id="54da3-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="54da3-105">权限</span><span class="sxs-lookup"><span data-stu-id="54da3-105">Permissions</span></span>
<span data-ttu-id="54da3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54da3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54da3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="54da3-108">Permission type</span></span> | <span data-ttu-id="54da3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54da3-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="54da3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54da3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="54da3-111">不支持</span><span class="sxs-lookup"><span data-stu-id="54da3-111">Not Supported</span></span>        |
| <span data-ttu-id="54da3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54da3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54da3-113">不支持</span><span class="sxs-lookup"><span data-stu-id="54da3-113">Not Supported</span></span>        |
| <span data-ttu-id="54da3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="54da3-114">Application</span></span>     | <span data-ttu-id="54da3-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="54da3-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54da3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54da3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /communications/calls/{id}/participants/configureMixer
```
> <span data-ttu-id="54da3-117">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="54da3-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="54da3-118">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="54da3-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54da3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54da3-119">Request headers</span></span>
| <span data-ttu-id="54da3-120">名称</span><span class="sxs-lookup"><span data-stu-id="54da3-120">Name</span></span>          | <span data-ttu-id="54da3-121">说明</span><span class="sxs-lookup"><span data-stu-id="54da3-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="54da3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54da3-122">Authorization</span></span> | <span data-ttu-id="54da3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54da3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54da3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="54da3-125">Request body</span></span>
<span data-ttu-id="54da3-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="54da3-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="54da3-127">参数</span><span class="sxs-lookup"><span data-stu-id="54da3-127">Parameter</span></span>      | <span data-ttu-id="54da3-128">类型</span><span class="sxs-lookup"><span data-stu-id="54da3-128">Type</span></span>    |<span data-ttu-id="54da3-129">说明</span><span class="sxs-lookup"><span data-stu-id="54da3-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54da3-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="54da3-130">participantMixerLevels</span></span>|<span data-ttu-id="54da3-131">[participantMixerLevel](../resources/participantmixerlevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="54da3-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="54da3-132">指定的音频参与者的混音器级别配置。</span><span class="sxs-lookup"><span data-stu-id="54da3-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="54da3-133">适用</span><span class="sxs-lookup"><span data-stu-id="54da3-133">clientContext</span></span>|<span data-ttu-id="54da3-134">String</span><span class="sxs-lookup"><span data-stu-id="54da3-134">String</span></span>|<span data-ttu-id="54da3-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="54da3-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="54da3-136">响应</span><span class="sxs-lookup"><span data-stu-id="54da3-136">Response</span></span>
<span data-ttu-id="54da3-137">返回`202 Accepted`响应代码和位置标头，其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="54da3-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="54da3-138">示例</span><span class="sxs-lookup"><span data-stu-id="54da3-138">Example</span></span>
<span data-ttu-id="54da3-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="54da3-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="54da3-140">请求</span><span class="sxs-lookup"><span data-stu-id="54da3-140">Request</span></span>
<span data-ttu-id="54da3-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="54da3-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="54da3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="54da3-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="54da3-143">C#</span><span class="sxs-lookup"><span data-stu-id="54da3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54da3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54da3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54da3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54da3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="54da3-146">响应</span><span class="sxs-lookup"><span data-stu-id="54da3-146">Response</span></span>

> <span data-ttu-id="54da3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="54da3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="54da3-149">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="54da3-149">Notification - operation completed</span></span>

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
