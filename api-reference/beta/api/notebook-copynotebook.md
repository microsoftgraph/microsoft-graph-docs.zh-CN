---
title: notebook： copyNotebook
description: 将笔记本复制到目标文档库中的笔记本文件夹。 如果文件夹不存在，则创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6f22838e9af2103f83f2c065e1376f931152fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786129"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="5c44a-104">notebook： copyNotebook</span><span class="sxs-lookup"><span data-stu-id="5c44a-104">notebook: copyNotebook</span></span>

<span data-ttu-id="5c44a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c44a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c44a-106">将笔记本复制到目标文档库中的笔记本文件夹。</span><span class="sxs-lookup"><span data-stu-id="5c44a-106">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="5c44a-107">如果文件夹不存在，则创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="5c44a-107">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="5c44a-108">对于 Copy 操作，你可以遵循异步调用模式：首先调用 Copy 操作，然后轮询操作终结点的结果。</span><span class="sxs-lookup"><span data-stu-id="5c44a-108">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c44a-109">权限</span><span class="sxs-lookup"><span data-stu-id="5c44a-109">Permissions</span></span>
<span data-ttu-id="5c44a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c44a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c44a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c44a-112">Permission type</span></span>      | <span data-ttu-id="5c44a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c44a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c44a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c44a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5c44a-115">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c44a-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c44a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c44a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c44a-117">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c44a-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5c44a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c44a-118">Application</span></span> | <span data-ttu-id="5c44a-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c44a-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c44a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c44a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="5c44a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c44a-121">Request headers</span></span>
| <span data-ttu-id="5c44a-122">名称</span><span class="sxs-lookup"><span data-stu-id="5c44a-122">Name</span></span>       | <span data-ttu-id="5c44a-123">类型</span><span class="sxs-lookup"><span data-stu-id="5c44a-123">Type</span></span> | <span data-ttu-id="5c44a-124">说明</span><span class="sxs-lookup"><span data-stu-id="5c44a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c44a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c44a-125">Authorization</span></span>  | <span data-ttu-id="5c44a-126">string</span><span class="sxs-lookup"><span data-stu-id="5c44a-126">string</span></span>  | <span data-ttu-id="5c44a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c44a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c44a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c44a-129">Content-Type</span></span> | <span data-ttu-id="5c44a-130">string</span><span class="sxs-lookup"><span data-stu-id="5c44a-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5c44a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c44a-131">Request body</span></span>
<span data-ttu-id="5c44a-132">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5c44a-132">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="5c44a-133">如果不需要，可以发送空正文。</span><span class="sxs-lookup"><span data-stu-id="5c44a-133">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="5c44a-134">参数</span><span class="sxs-lookup"><span data-stu-id="5c44a-134">Parameter</span></span>    | <span data-ttu-id="5c44a-135">类型</span><span class="sxs-lookup"><span data-stu-id="5c44a-135">Type</span></span>   |<span data-ttu-id="5c44a-136">说明</span><span class="sxs-lookup"><span data-stu-id="5c44a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c44a-137">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="5c44a-137">siteCollectionId</span></span>|<span data-ttu-id="5c44a-138">String</span><span class="sxs-lookup"><span data-stu-id="5c44a-138">String</span></span>|<span data-ttu-id="5c44a-139">要复制到SharePoint网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="5c44a-139">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="5c44a-140">仅在复制到网站时SharePoint使用。</span><span class="sxs-lookup"><span data-stu-id="5c44a-140">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="5c44a-141">siteId</span><span class="sxs-lookup"><span data-stu-id="5c44a-141">siteId</span></span>|<span data-ttu-id="5c44a-142">String</span><span class="sxs-lookup"><span data-stu-id="5c44a-142">String</span></span>|<span data-ttu-id="5c44a-143">要复制到SharePoint Web 的 ID。</span><span class="sxs-lookup"><span data-stu-id="5c44a-143">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="5c44a-144">仅在复制到网站时SharePoint使用。</span><span class="sxs-lookup"><span data-stu-id="5c44a-144">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="5c44a-145">groupId</span><span class="sxs-lookup"><span data-stu-id="5c44a-145">groupId</span></span>|<span data-ttu-id="5c44a-146">String</span><span class="sxs-lookup"><span data-stu-id="5c44a-146">String</span></span>|<span data-ttu-id="5c44a-147">要复制到的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="5c44a-147">The id of the group to copy to.</span></span> <span data-ttu-id="5c44a-148">仅在复制到组时Microsoft 365使用。</span><span class="sxs-lookup"><span data-stu-id="5c44a-148">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="5c44a-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="5c44a-149">renameAs</span></span>|<span data-ttu-id="5c44a-150">String</span><span class="sxs-lookup"><span data-stu-id="5c44a-150">String</span></span>|<span data-ttu-id="5c44a-151">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="5c44a-151">The name of the copy.</span></span> <span data-ttu-id="5c44a-152">默认为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="5c44a-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="5c44a-153">响应</span><span class="sxs-lookup"><span data-stu-id="5c44a-153">Response</span></span>

<span data-ttu-id="5c44a-154">如果成功，此方法返回 响应 `202 Accepted` 代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="5c44a-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="5c44a-155">轮询Operation-Location [终结点，获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="5c44a-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="5c44a-156">示例</span><span class="sxs-lookup"><span data-stu-id="5c44a-156">Example</span></span>
<span data-ttu-id="5c44a-157">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5c44a-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c44a-158">请求</span><span class="sxs-lookup"><span data-stu-id="5c44a-158">Request</span></span>
<span data-ttu-id="5c44a-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c44a-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c44a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c44a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="5c44a-161">C#</span><span class="sxs-lookup"><span data-stu-id="5c44a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c44a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c44a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c44a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c44a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c44a-164">Java</span><span class="sxs-lookup"><span data-stu-id="5c44a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c44a-165">响应</span><span class="sxs-lookup"><span data-stu-id="5c44a-165">Response</span></span>
<span data-ttu-id="5c44a-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5c44a-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


