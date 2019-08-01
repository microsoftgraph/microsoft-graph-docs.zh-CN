---
title: '页面: copyToSection'
description: 将页面复制到特定分区。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: d3b626f6c982488826b698f82c57436c0976724e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022647"
---
# <a name="page-copytosection"></a><span data-ttu-id="c2cec-103">页面: copyToSection</span><span class="sxs-lookup"><span data-stu-id="c2cec-103">page: copyToSection</span></span>
<span data-ttu-id="c2cec-104">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="c2cec-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="c2cec-105">对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="c2cec-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2cec-106">权限</span><span class="sxs-lookup"><span data-stu-id="c2cec-106">Permissions</span></span>
<span data-ttu-id="c2cec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2cec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2cec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2cec-109">Permission type</span></span>      | <span data-ttu-id="c2cec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2cec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2cec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2cec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2cec-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2cec-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2cec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2cec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2cec-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2cec-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c2cec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2cec-115">Application</span></span> | <span data-ttu-id="c2cec-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2cec-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2cec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2cec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="c2cec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2cec-118">Request headers</span></span>
| <span data-ttu-id="c2cec-119">名称</span><span class="sxs-lookup"><span data-stu-id="c2cec-119">Name</span></span>       | <span data-ttu-id="c2cec-120">类型</span><span class="sxs-lookup"><span data-stu-id="c2cec-120">Type</span></span> | <span data-ttu-id="c2cec-121">说明</span><span class="sxs-lookup"><span data-stu-id="c2cec-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2cec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2cec-122">Authorization</span></span>  | <span data-ttu-id="c2cec-123">string</span><span class="sxs-lookup"><span data-stu-id="c2cec-123">string</span></span>  | <span data-ttu-id="c2cec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2cec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2cec-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2cec-126">Content-Type</span></span> | <span data-ttu-id="c2cec-127">string</span><span class="sxs-lookup"><span data-stu-id="c2cec-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c2cec-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2cec-128">Request body</span></span>
<span data-ttu-id="c2cec-129">在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="c2cec-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="c2cec-130">参数</span><span class="sxs-lookup"><span data-stu-id="c2cec-130">Parameter</span></span>    | <span data-ttu-id="c2cec-131">类型</span><span class="sxs-lookup"><span data-stu-id="c2cec-131">Type</span></span>   |<span data-ttu-id="c2cec-132">说明</span><span class="sxs-lookup"><span data-stu-id="c2cec-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2cec-133">groupId</span><span class="sxs-lookup"><span data-stu-id="c2cec-133">groupId</span></span>|<span data-ttu-id="c2cec-134">String</span><span class="sxs-lookup"><span data-stu-id="c2cec-134">String</span></span>|<span data-ttu-id="c2cec-135">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="c2cec-135">The id of the group to copy to.</span></span> <span data-ttu-id="c2cec-136">仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="c2cec-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="c2cec-137">id</span><span class="sxs-lookup"><span data-stu-id="c2cec-137">id</span></span>|<span data-ttu-id="c2cec-138">String</span><span class="sxs-lookup"><span data-stu-id="c2cec-138">String</span></span>|<span data-ttu-id="c2cec-139">必需。</span><span class="sxs-lookup"><span data-stu-id="c2cec-139">Required.</span></span> <span data-ttu-id="c2cec-140">目标部分的 id。</span><span class="sxs-lookup"><span data-stu-id="c2cec-140">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="c2cec-141">响应</span><span class="sxs-lookup"><span data-stu-id="c2cec-141">Response</span></span>

<span data-ttu-id="c2cec-142">如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。</span><span class="sxs-lookup"><span data-stu-id="c2cec-142">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="c2cec-143">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="c2cec-143">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="c2cec-144">示例</span><span class="sxs-lookup"><span data-stu-id="c2cec-144">Example</span></span>
<span data-ttu-id="c2cec-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c2cec-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2cec-146">请求</span><span class="sxs-lookup"><span data-stu-id="c2cec-146">Request</span></span>
<span data-ttu-id="c2cec-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2cec-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2cec-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2cec-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2cec-149">C#</span><span class="sxs-lookup"><span data-stu-id="c2cec-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2cec-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2cec-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2cec-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2cec-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2cec-152">Java</span><span class="sxs-lookup"><span data-stu-id="c2cec-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c2cec-153">响应</span><span class="sxs-lookup"><span data-stu-id="c2cec-153">Response</span></span>
<span data-ttu-id="c2cec-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2cec-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
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
