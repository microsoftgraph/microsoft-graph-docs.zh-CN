---
title: 关闭会话
description: '使用此 API 关闭现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 634f3394bc4dcd1de273dcfd67715567f52d7b79
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458409"
---
# <a name="close-session"></a><span data-ttu-id="84db1-103">关闭会话</span><span class="sxs-lookup"><span data-stu-id="84db1-103">Close Session</span></span>

<span data-ttu-id="84db1-104">使用此 API 关闭现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="84db1-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="84db1-105">权限</span><span class="sxs-lookup"><span data-stu-id="84db1-105">Permissions</span></span>
<span data-ttu-id="84db1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84db1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84db1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="84db1-108">Permission type</span></span>      | <span data-ttu-id="84db1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84db1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84db1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84db1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84db1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84db1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84db1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84db1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84db1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="84db1-113">Not supported.</span></span>    |
|<span data-ttu-id="84db1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="84db1-114">Application</span></span> | <span data-ttu-id="84db1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84db1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84db1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84db1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="84db1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="84db1-117">Request headers</span></span>
| <span data-ttu-id="84db1-118">名称</span><span class="sxs-lookup"><span data-stu-id="84db1-118">Name</span></span>       | <span data-ttu-id="84db1-119">说明</span><span class="sxs-lookup"><span data-stu-id="84db1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="84db1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="84db1-120">Authorization</span></span>  | <span data-ttu-id="84db1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84db1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84db1-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="84db1-123">workbook-session-id</span></span> | <span data-ttu-id="84db1-124">要关闭的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="84db1-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="84db1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="84db1-125">Request body</span></span>
<span data-ttu-id="84db1-126">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="84db1-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="84db1-127">响应</span><span class="sxs-lookup"><span data-stu-id="84db1-127">Response</span></span>

<span data-ttu-id="84db1-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="84db1-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84db1-129">示例</span><span class="sxs-lookup"><span data-stu-id="84db1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84db1-130">请求</span><span class="sxs-lookup"><span data-stu-id="84db1-130">Request</span></span>
<span data-ttu-id="84db1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84db1-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84db1-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="84db1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84db1-133">C#</span><span class="sxs-lookup"><span data-stu-id="84db1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84db1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="84db1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84db1-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="84db1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="84db1-136">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="84db1-136">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="84db1-137">响应</span><span class="sxs-lookup"><span data-stu-id="84db1-137">Response</span></span>
<span data-ttu-id="84db1-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="84db1-138">Here is an example of the response.</span></span> 

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
