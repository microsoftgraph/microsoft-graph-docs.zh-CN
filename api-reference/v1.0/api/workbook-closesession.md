---
title: 关闭会话
description: '使用此 API 关闭现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 78ae4d0c9eca6dbf54dde2870c3691b2f5e4cd6f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364943"
---
# <a name="close-session"></a><span data-ttu-id="90751-103">关闭会话</span><span class="sxs-lookup"><span data-stu-id="90751-103">Close Session</span></span>

<span data-ttu-id="90751-104">使用此 API 关闭现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="90751-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="90751-105">权限</span><span class="sxs-lookup"><span data-stu-id="90751-105">Permissions</span></span>
<span data-ttu-id="90751-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90751-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90751-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="90751-108">Permission type</span></span>      | <span data-ttu-id="90751-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90751-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90751-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90751-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90751-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90751-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90751-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90751-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90751-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="90751-113">Not supported.</span></span>    |
|<span data-ttu-id="90751-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="90751-114">Application</span></span> | <span data-ttu-id="90751-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90751-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90751-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90751-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="90751-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="90751-117">Request headers</span></span>
| <span data-ttu-id="90751-118">名称</span><span class="sxs-lookup"><span data-stu-id="90751-118">Name</span></span>       | <span data-ttu-id="90751-119">说明</span><span class="sxs-lookup"><span data-stu-id="90751-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90751-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="90751-120">Authorization</span></span>  | <span data-ttu-id="90751-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90751-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="90751-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="90751-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="90751-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="90751-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="90751-126">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="90751-126">workbook-session-id</span></span> | <span data-ttu-id="90751-127">要关闭的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="90751-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="90751-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="90751-128">Request body</span></span>
<span data-ttu-id="90751-129">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="90751-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="90751-130">响应</span><span class="sxs-lookup"><span data-stu-id="90751-130">Response</span></span>

<span data-ttu-id="90751-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="90751-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90751-132">示例</span><span class="sxs-lookup"><span data-stu-id="90751-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90751-133">请求</span><span class="sxs-lookup"><span data-stu-id="90751-133">Request</span></span>
<span data-ttu-id="90751-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90751-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90751-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="90751-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90751-136">C#</span><span class="sxs-lookup"><span data-stu-id="90751-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90751-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90751-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90751-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="90751-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="90751-139">Java</span><span class="sxs-lookup"><span data-stu-id="90751-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/close-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="90751-140">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="90751-140">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="90751-141">响应</span><span class="sxs-lookup"><span data-stu-id="90751-141">Response</span></span>
<span data-ttu-id="90751-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="90751-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
