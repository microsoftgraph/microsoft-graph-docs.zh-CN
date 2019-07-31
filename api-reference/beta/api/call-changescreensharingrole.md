---
title: '调用: changeScreenSharingRole'
description: 在呼叫中开始和停止共享屏幕。 此 API 用于允许应用程序与呼叫或会议的参与者共享屏幕内容。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fbcc26cc534702ba1c136725a8fbbca2867ece57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944523"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="2af74-104">调用: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="2af74-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2af74-105">在呼叫中开始和停止共享屏幕。</span><span class="sxs-lookup"><span data-stu-id="2af74-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="2af74-106">此 API 用于允许应用程序与呼叫或会议的参与者共享屏幕内容。</span><span class="sxs-lookup"><span data-stu-id="2af74-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="2af74-107">权限</span><span class="sxs-lookup"><span data-stu-id="2af74-107">Permissions</span></span>
<span data-ttu-id="2af74-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2af74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2af74-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2af74-110">Permission type</span></span>                        | <span data-ttu-id="2af74-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2af74-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2af74-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2af74-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2af74-113">不支持</span><span class="sxs-lookup"><span data-stu-id="2af74-113">Not Supported</span></span>                               |
| <span data-ttu-id="2af74-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2af74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2af74-115">不支持</span><span class="sxs-lookup"><span data-stu-id="2af74-115">Not Supported</span></span>                               |
| <span data-ttu-id="2af74-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2af74-116">Application</span></span>                            | <span data-ttu-id="2af74-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="2af74-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="2af74-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2af74-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="2af74-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2af74-119">Request headers</span></span>
| <span data-ttu-id="2af74-120">名称</span><span class="sxs-lookup"><span data-stu-id="2af74-120">Name</span></span>          | <span data-ttu-id="2af74-121">说明</span><span class="sxs-lookup"><span data-stu-id="2af74-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2af74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2af74-122">Authorization</span></span> | <span data-ttu-id="2af74-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2af74-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2af74-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2af74-125">Request body</span></span>
<span data-ttu-id="2af74-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2af74-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2af74-127">参数</span><span class="sxs-lookup"><span data-stu-id="2af74-127">Parameter</span></span>      | <span data-ttu-id="2af74-128">类型</span><span class="sxs-lookup"><span data-stu-id="2af74-128">Type</span></span>    |<span data-ttu-id="2af74-129">说明</span><span class="sxs-lookup"><span data-stu-id="2af74-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2af74-130">role</span><span class="sxs-lookup"><span data-stu-id="2af74-130">role</span></span>|<span data-ttu-id="2af74-131">String</span><span class="sxs-lookup"><span data-stu-id="2af74-131">String</span></span>|<span data-ttu-id="2af74-132">可能的值为: "查看器"、"共享资源"</span><span class="sxs-lookup"><span data-stu-id="2af74-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="2af74-133">响应</span><span class="sxs-lookup"><span data-stu-id="2af74-133">Response</span></span>
<span data-ttu-id="2af74-134">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="2af74-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2af74-135">示例</span><span class="sxs-lookup"><span data-stu-id="2af74-135">Example</span></span>
<span data-ttu-id="2af74-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2af74-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2af74-137">请求</span><span class="sxs-lookup"><span data-stu-id="2af74-137">Request</span></span>
<span data-ttu-id="2af74-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="2af74-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2af74-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2af74-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2af74-140">C#</span><span class="sxs-lookup"><span data-stu-id="2af74-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2af74-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="2af74-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2af74-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="2af74-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2af74-143">Java</span><span class="sxs-lookup"><span data-stu-id="2af74-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2af74-144">响应</span><span class="sxs-lookup"><span data-stu-id="2af74-144">Response</span></span>
<span data-ttu-id="2af74-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2af74-145">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

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
  ]
}
-->
