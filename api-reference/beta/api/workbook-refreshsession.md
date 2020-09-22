---
title: 刷新会话
description: '使用此 API 刷新现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b9cd1a3762b45bca1f7ce7be15928f99f8fcdd5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974021"
---
# <a name="refresh-session"></a><span data-ttu-id="ad09e-103">刷新会话</span><span class="sxs-lookup"><span data-stu-id="ad09e-103">Refresh Session</span></span>

<span data-ttu-id="ad09e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad09e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad09e-105">使用此 API 刷新现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="ad09e-105">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ad09e-106">权限</span><span class="sxs-lookup"><span data-stu-id="ad09e-106">Permissions</span></span>
<span data-ttu-id="ad09e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad09e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad09e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad09e-109">Permission type</span></span>      | <span data-ttu-id="ad09e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad09e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad09e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad09e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad09e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad09e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ad09e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad09e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad09e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad09e-114">Not supported.</span></span>    |
|<span data-ttu-id="ad09e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad09e-115">Application</span></span> | <span data-ttu-id="ad09e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad09e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad09e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad09e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="ad09e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad09e-118">Request headers</span></span>
| <span data-ttu-id="ad09e-119">名称</span><span class="sxs-lookup"><span data-stu-id="ad09e-119">Name</span></span>       | <span data-ttu-id="ad09e-120">说明</span><span class="sxs-lookup"><span data-stu-id="ad09e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad09e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad09e-121">Authorization</span></span>  | <span data-ttu-id="ad09e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad09e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad09e-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="ad09e-124">workbook-session-id</span></span> | <span data-ttu-id="ad09e-125">要刷新的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="ad09e-125">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad09e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad09e-126">Request body</span></span>
<span data-ttu-id="ad09e-127">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad09e-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="ad09e-128">响应</span><span class="sxs-lookup"><span data-stu-id="ad09e-128">Response</span></span>

<span data-ttu-id="ad09e-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ad09e-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ad09e-130">示例</span><span class="sxs-lookup"><span data-stu-id="ad09e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad09e-131">请求</span><span class="sxs-lookup"><span data-stu-id="ad09e-131">Request</span></span>
<span data-ttu-id="ad09e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad09e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad09e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad09e-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ad09e-134">C#</span><span class="sxs-lookup"><span data-stu-id="ad09e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad09e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad09e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad09e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad09e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ad09e-137">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="ad09e-137">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="ad09e-138">响应</span><span class="sxs-lookup"><span data-stu-id="ad09e-138">Response</span></span>
<span data-ttu-id="ad09e-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ad09e-139">Here is an example of the response.</span></span> 

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


