---
title: '调用: changeScreenSharingRole'
description: 在呼叫中开始和停止共享屏幕。 此 API 用于允许应用程序与呼叫或会议的参与者共享屏幕内容。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 87a2c56810d80af8f38e0a3b7ae84b5c6f787e22
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262319"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="d5d7a-104">调用: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="d5d7a-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5d7a-105">在呼叫中开始和停止共享屏幕。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="d5d7a-106">此 API 用于允许应用程序与呼叫或会议的参与者共享屏幕内容。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5d7a-107">权限</span><span class="sxs-lookup"><span data-stu-id="d5d7a-107">Permissions</span></span>
<span data-ttu-id="d5d7a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5d7a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5d7a-110">Permission type</span></span>                        | <span data-ttu-id="d5d7a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5d7a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d5d7a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5d7a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5d7a-113">不支持</span><span class="sxs-lookup"><span data-stu-id="d5d7a-113">Not Supported</span></span>                               |
| <span data-ttu-id="d5d7a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5d7a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5d7a-115">不支持</span><span class="sxs-lookup"><span data-stu-id="d5d7a-115">Not Supported</span></span>                               |
| <span data-ttu-id="d5d7a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5d7a-116">Application</span></span>                            | <span data-ttu-id="d5d7a-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="d5d7a-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="d5d7a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5d7a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="d5d7a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5d7a-119">Request headers</span></span>
| <span data-ttu-id="d5d7a-120">名称</span><span class="sxs-lookup"><span data-stu-id="d5d7a-120">Name</span></span>          | <span data-ttu-id="d5d7a-121">说明</span><span class="sxs-lookup"><span data-stu-id="d5d7a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d5d7a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5d7a-122">Authorization</span></span> | <span data-ttu-id="d5d7a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5d7a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5d7a-125">Request body</span></span>
<span data-ttu-id="d5d7a-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5d7a-127">参数</span><span class="sxs-lookup"><span data-stu-id="d5d7a-127">Parameter</span></span>      | <span data-ttu-id="d5d7a-128">类型</span><span class="sxs-lookup"><span data-stu-id="d5d7a-128">Type</span></span>    |<span data-ttu-id="d5d7a-129">说明</span><span class="sxs-lookup"><span data-stu-id="d5d7a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5d7a-130">role</span><span class="sxs-lookup"><span data-stu-id="d5d7a-130">role</span></span>|<span data-ttu-id="d5d7a-131">String</span><span class="sxs-lookup"><span data-stu-id="d5d7a-131">String</span></span>|<span data-ttu-id="d5d7a-132">可能的值为: "查看器"、"共享资源"</span><span class="sxs-lookup"><span data-stu-id="d5d7a-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="d5d7a-133">响应</span><span class="sxs-lookup"><span data-stu-id="d5d7a-133">Response</span></span>
<span data-ttu-id="d5d7a-134">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5d7a-135">示例</span><span class="sxs-lookup"><span data-stu-id="d5d7a-135">Example</span></span>
<span data-ttu-id="d5d7a-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d5d7a-137">请求</span><span class="sxs-lookup"><span data-stu-id="d5d7a-137">Request</span></span>
<span data-ttu-id="d5d7a-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="d5d7a-139">响应</span><span class="sxs-lookup"><span data-stu-id="d5d7a-139">Response</span></span>
<span data-ttu-id="d5d7a-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d5d7a-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5d7a-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d5d7a-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d5d7a-142">C#</span><span class="sxs-lookup"><span data-stu-id="d5d7a-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5d7a-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5d7a-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d5d7a-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="d5d7a-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
