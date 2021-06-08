---
title: page： copyToSection
description: 将页面复制到特定节。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c9bdd57eaa929c47ed6dfe5429086e0f78760e06
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788064"
---
# <a name="page-copytosection"></a><span data-ttu-id="db411-103">page： copyToSection</span><span class="sxs-lookup"><span data-stu-id="db411-103">page: copyToSection</span></span>

<span data-ttu-id="db411-104">命名空间：microsoft.graph 将页面复制到特定部分。</span><span class="sxs-lookup"><span data-stu-id="db411-104">Namespace: microsoft.graph Copies a page to a specific section.</span></span>

<span data-ttu-id="db411-105">对于 Copy 操作，你可以遵循异步调用模式：首先调用 Copy 操作，然后轮询操作终结点的结果。</span><span class="sxs-lookup"><span data-stu-id="db411-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="db411-106">权限</span><span class="sxs-lookup"><span data-stu-id="db411-106">Permissions</span></span>
<span data-ttu-id="db411-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db411-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db411-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db411-109">Permission type</span></span>      | <span data-ttu-id="db411-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db411-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db411-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db411-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db411-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db411-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="db411-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db411-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db411-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db411-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="db411-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db411-115">Application</span></span> | <span data-ttu-id="db411-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db411-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db411-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db411-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="db411-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db411-118">Request headers</span></span>
| <span data-ttu-id="db411-119">名称</span><span class="sxs-lookup"><span data-stu-id="db411-119">Name</span></span>       | <span data-ttu-id="db411-120">类型</span><span class="sxs-lookup"><span data-stu-id="db411-120">Type</span></span> | <span data-ttu-id="db411-121">说明</span><span class="sxs-lookup"><span data-stu-id="db411-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db411-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db411-122">Authorization</span></span>  | <span data-ttu-id="db411-123">string</span><span class="sxs-lookup"><span data-stu-id="db411-123">string</span></span>  | <span data-ttu-id="db411-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db411-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db411-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db411-126">Content-Type</span></span> | <span data-ttu-id="db411-127">string</span><span class="sxs-lookup"><span data-stu-id="db411-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="db411-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="db411-128">Request body</span></span>
<span data-ttu-id="db411-129">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="db411-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="db411-130">参数</span><span class="sxs-lookup"><span data-stu-id="db411-130">Parameter</span></span>    | <span data-ttu-id="db411-131">类型</span><span class="sxs-lookup"><span data-stu-id="db411-131">Type</span></span>   |<span data-ttu-id="db411-132">说明</span><span class="sxs-lookup"><span data-stu-id="db411-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db411-133">groupId</span><span class="sxs-lookup"><span data-stu-id="db411-133">groupId</span></span>|<span data-ttu-id="db411-134">String</span><span class="sxs-lookup"><span data-stu-id="db411-134">String</span></span>|<span data-ttu-id="db411-135">要复制到的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="db411-135">The id of the group to copy to.</span></span> <span data-ttu-id="db411-136">仅在复制到组时Microsoft 365使用。</span><span class="sxs-lookup"><span data-stu-id="db411-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="db411-137">id</span><span class="sxs-lookup"><span data-stu-id="db411-137">id</span></span>|<span data-ttu-id="db411-138">String</span><span class="sxs-lookup"><span data-stu-id="db411-138">String</span></span>|<span data-ttu-id="db411-139">必填。</span><span class="sxs-lookup"><span data-stu-id="db411-139">Required.</span></span> <span data-ttu-id="db411-140">目标节的 ID。</span><span class="sxs-lookup"><span data-stu-id="db411-140">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="db411-141">响应</span><span class="sxs-lookup"><span data-stu-id="db411-141">Response</span></span>

<span data-ttu-id="db411-142">如果成功，此方法返回 响应 `202 Accepted` 代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="db411-142">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="db411-143">轮询Operation-Location [终结点，获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="db411-143">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="db411-144">示例</span><span class="sxs-lookup"><span data-stu-id="db411-144">Example</span></span>
<span data-ttu-id="db411-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="db411-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db411-146">请求</span><span class="sxs-lookup"><span data-stu-id="db411-146">Request</span></span>
<span data-ttu-id="db411-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db411-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db411-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="db411-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="db411-149">C#</span><span class="sxs-lookup"><span data-stu-id="db411-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db411-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db411-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db411-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db411-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db411-152">Java</span><span class="sxs-lookup"><span data-stu-id="db411-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db411-153">响应</span><span class="sxs-lookup"><span data-stu-id="db411-153">Response</span></span>
<span data-ttu-id="db411-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="db411-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

