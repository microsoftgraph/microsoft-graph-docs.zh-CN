---
title: '部分: copyToNotebook'
description: 将分区复制到特定笔记本。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 54e3fbb6fb136c2c0d8491271642d3308fd2d5cb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870553"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="db375-103">部分: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="db375-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db375-104">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="db375-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="db375-105">对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="db375-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="db375-106">权限</span><span class="sxs-lookup"><span data-stu-id="db375-106">Permissions</span></span>
<span data-ttu-id="db375-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db375-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db375-109">Permission type</span></span>      | <span data-ttu-id="db375-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db375-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db375-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db375-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db375-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db375-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="db375-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db375-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db375-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db375-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="db375-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db375-115">Application</span></span> | <span data-ttu-id="db375-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db375-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db375-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db375-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="db375-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db375-118">Request headers</span></span>
| <span data-ttu-id="db375-119">名称</span><span class="sxs-lookup"><span data-stu-id="db375-119">Name</span></span>       | <span data-ttu-id="db375-120">类型</span><span class="sxs-lookup"><span data-stu-id="db375-120">Type</span></span> | <span data-ttu-id="db375-121">说明</span><span class="sxs-lookup"><span data-stu-id="db375-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db375-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db375-122">Authorization</span></span>  | <span data-ttu-id="db375-123">string</span><span class="sxs-lookup"><span data-stu-id="db375-123">string</span></span>  | <span data-ttu-id="db375-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db375-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db375-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db375-126">Content-Type</span></span> | <span data-ttu-id="db375-127">string</span><span class="sxs-lookup"><span data-stu-id="db375-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="db375-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="db375-128">Request body</span></span>
<span data-ttu-id="db375-129">在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="db375-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="db375-130">参数</span><span class="sxs-lookup"><span data-stu-id="db375-130">Parameter</span></span>    | <span data-ttu-id="db375-131">类型</span><span class="sxs-lookup"><span data-stu-id="db375-131">Type</span></span>   |<span data-ttu-id="db375-132">说明</span><span class="sxs-lookup"><span data-stu-id="db375-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db375-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="db375-133">siteCollectionId</span></span>|<span data-ttu-id="db375-134">String</span><span class="sxs-lookup"><span data-stu-id="db375-134">String</span></span>|<span data-ttu-id="db375-135">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="db375-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="db375-136">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="db375-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="db375-137">siteId</span><span class="sxs-lookup"><span data-stu-id="db375-137">siteId</span></span>|<span data-ttu-id="db375-138">String</span><span class="sxs-lookup"><span data-stu-id="db375-138">String</span></span>|<span data-ttu-id="db375-139">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="db375-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="db375-140">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="db375-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="db375-141">groupId</span><span class="sxs-lookup"><span data-stu-id="db375-141">groupId</span></span>|<span data-ttu-id="db375-142">String</span><span class="sxs-lookup"><span data-stu-id="db375-142">String</span></span>|<span data-ttu-id="db375-143">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="db375-143">The id of the group to copy to.</span></span> <span data-ttu-id="db375-144">仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="db375-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="db375-145">id</span><span class="sxs-lookup"><span data-stu-id="db375-145">id</span></span>|<span data-ttu-id="db375-146">String</span><span class="sxs-lookup"><span data-stu-id="db375-146">String</span></span>|<span data-ttu-id="db375-147">必需。</span><span class="sxs-lookup"><span data-stu-id="db375-147">Required.</span></span> <span data-ttu-id="db375-148">目标笔记本的 id。</span><span class="sxs-lookup"><span data-stu-id="db375-148">The id of the destination notebook.</span></span> |
|<span data-ttu-id="db375-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="db375-149">renameAs</span></span>|<span data-ttu-id="db375-150">String</span><span class="sxs-lookup"><span data-stu-id="db375-150">String</span></span>|<span data-ttu-id="db375-151">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="db375-151">The name of the copy.</span></span> <span data-ttu-id="db375-152">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="db375-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="db375-153">响应</span><span class="sxs-lookup"><span data-stu-id="db375-153">Response</span></span>

<span data-ttu-id="db375-154">如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。</span><span class="sxs-lookup"><span data-stu-id="db375-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="db375-155">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="db375-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="db375-156">示例</span><span class="sxs-lookup"><span data-stu-id="db375-156">Example</span></span>
<span data-ttu-id="db375-157">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="db375-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db375-158">请求</span><span class="sxs-lookup"><span data-stu-id="db375-158">Request</span></span>
<span data-ttu-id="db375-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db375-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db375-160">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="db375-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db375-161">C#</span><span class="sxs-lookup"><span data-stu-id="db375-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db375-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="db375-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db375-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="db375-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db375-164">Java</span><span class="sxs-lookup"><span data-stu-id="db375-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db375-165">响应</span><span class="sxs-lookup"><span data-stu-id="db375-165">Response</span></span>
<span data-ttu-id="db375-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="db375-166">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
