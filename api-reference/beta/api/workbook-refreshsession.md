---
title: 刷新会话
description: '使用此 API 刷新现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c09100fd5607bd78561e8635acc9c2579f6e55eb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421657"
---
# <a name="refresh-session"></a><span data-ttu-id="f389e-103">刷新会话</span><span class="sxs-lookup"><span data-stu-id="f389e-103">Refresh Session</span></span>

<span data-ttu-id="f389e-104">使用此 API 刷新现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="f389e-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f389e-105">权限</span><span class="sxs-lookup"><span data-stu-id="f389e-105">Permissions</span></span>
<span data-ttu-id="f389e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f389e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f389e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f389e-108">Permission type</span></span>      | <span data-ttu-id="f389e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f389e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f389e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f389e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f389e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f389e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f389e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f389e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f389e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f389e-113">Not supported.</span></span>    |
|<span data-ttu-id="f389e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f389e-114">Application</span></span> | <span data-ttu-id="f389e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f389e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f389e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f389e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="f389e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f389e-117">Request headers</span></span>
| <span data-ttu-id="f389e-118">名称</span><span class="sxs-lookup"><span data-stu-id="f389e-118">Name</span></span>       | <span data-ttu-id="f389e-119">说明</span><span class="sxs-lookup"><span data-stu-id="f389e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f389e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f389e-120">Authorization</span></span>  | <span data-ttu-id="f389e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f389e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f389e-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="f389e-123">workbook-session-id</span></span> | <span data-ttu-id="f389e-124">要刷新的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="f389e-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="f389e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f389e-125">Request body</span></span>
<span data-ttu-id="f389e-126">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="f389e-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="f389e-127">响应</span><span class="sxs-lookup"><span data-stu-id="f389e-127">Response</span></span>

<span data-ttu-id="f389e-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f389e-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f389e-129">示例</span><span class="sxs-lookup"><span data-stu-id="f389e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f389e-130">请求</span><span class="sxs-lookup"><span data-stu-id="f389e-130">Request</span></span>
<span data-ttu-id="f389e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f389e-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f389e-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f389e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f389e-133">C#</span><span class="sxs-lookup"><span data-stu-id="f389e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f389e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f389e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f389e-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="f389e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f389e-136">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="f389e-136">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="f389e-137">响应</span><span class="sxs-lookup"><span data-stu-id="f389e-137">Response</span></span>
<span data-ttu-id="f389e-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f389e-138">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
