---
title: '参与者: muteAll'
description: 将呼叫中的所有参与者设为静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a322d04dbfa9b35111cbd549564ec39beea7dd8e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453913"
---
# <a name="participant-muteall"></a><span data-ttu-id="ff788-103">参与者: muteAll</span><span class="sxs-lookup"><span data-stu-id="ff788-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff788-104">将呼叫中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="ff788-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff788-105">权限</span><span class="sxs-lookup"><span data-stu-id="ff788-105">Permissions</span></span>
<span data-ttu-id="ff788-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff788-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff788-108">Permission type</span></span>                        | <span data-ttu-id="ff788-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff788-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff788-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff788-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff788-111">不支持</span><span class="sxs-lookup"><span data-stu-id="ff788-111">Not Supported</span></span>                               |
| <span data-ttu-id="ff788-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff788-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff788-113">不支持</span><span class="sxs-lookup"><span data-stu-id="ff788-113">Not Supported</span></span>                               |
| <span data-ttu-id="ff788-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff788-114">Application</span></span>                            | <span data-ttu-id="ff788-115">无</span><span class="sxs-lookup"><span data-stu-id="ff788-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="ff788-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff788-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="ff788-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff788-117">Request headers</span></span>
| <span data-ttu-id="ff788-118">名称</span><span class="sxs-lookup"><span data-stu-id="ff788-118">Name</span></span>          | <span data-ttu-id="ff788-119">说明</span><span class="sxs-lookup"><span data-stu-id="ff788-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ff788-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff788-120">Authorization</span></span> | <span data-ttu-id="ff788-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff788-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff788-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff788-123">Request body</span></span>
<span data-ttu-id="ff788-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ff788-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ff788-125">参数</span><span class="sxs-lookup"><span data-stu-id="ff788-125">Parameter</span></span>      | <span data-ttu-id="ff788-126">类型</span><span class="sxs-lookup"><span data-stu-id="ff788-126">Type</span></span>    |<span data-ttu-id="ff788-127">说明</span><span class="sxs-lookup"><span data-stu-id="ff788-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff788-128">participants</span><span class="sxs-lookup"><span data-stu-id="ff788-128">participants</span></span>|<span data-ttu-id="ff788-129">String collection</span><span class="sxs-lookup"><span data-stu-id="ff788-129">String collection</span></span>|<span data-ttu-id="ff788-130">要静音的参与者。</span><span class="sxs-lookup"><span data-stu-id="ff788-130">The participants to be muted.</span></span>|
|<span data-ttu-id="ff788-131">适用</span><span class="sxs-lookup"><span data-stu-id="ff788-131">clientContext</span></span>|<span data-ttu-id="ff788-132">String</span><span class="sxs-lookup"><span data-stu-id="ff788-132">String</span></span>|<span data-ttu-id="ff788-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="ff788-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="ff788-134">响应</span><span class="sxs-lookup"><span data-stu-id="ff788-134">Response</span></span>
<span data-ttu-id="ff788-135">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff788-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff788-136">示例</span><span class="sxs-lookup"><span data-stu-id="ff788-136">Example</span></span>
<span data-ttu-id="ff788-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ff788-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ff788-138">请求</span><span class="sxs-lookup"><span data-stu-id="ff788-138">Request</span></span>
<span data-ttu-id="ff788-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff788-139">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff788-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ff788-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff788-141">C#</span><span class="sxs-lookup"><span data-stu-id="ff788-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff788-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff788-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff788-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="ff788-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff788-144">响应</span><span class="sxs-lookup"><span data-stu-id="ff788-144">Response</span></span>

> <span data-ttu-id="ff788-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ff788-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
