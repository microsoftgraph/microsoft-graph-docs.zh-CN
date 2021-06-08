---
title: notebook： copyNotebook
description: 将笔记本复制到目标文档库中的笔记本文件夹。 如果文件夹不存在，则创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f46e65f200e87d0f39ef5e9307ee199de5595fb1
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787455"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="da2d8-104">notebook： copyNotebook</span><span class="sxs-lookup"><span data-stu-id="da2d8-104">notebook: copyNotebook</span></span>

<span data-ttu-id="da2d8-105">命名空间：microsoft.graph 将笔记本复制到目标文档库中的笔记本文件夹。</span><span class="sxs-lookup"><span data-stu-id="da2d8-105">Namespace: microsoft.graph Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="da2d8-106">如果文件夹不存在，则创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="da2d8-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="da2d8-107">对于 Copy 操作，你可以遵循异步调用模式：首先调用 Copy 操作，然后轮询操作终结点的结果。</span><span class="sxs-lookup"><span data-stu-id="da2d8-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="da2d8-108">权限</span><span class="sxs-lookup"><span data-stu-id="da2d8-108">Permissions</span></span>
<span data-ttu-id="da2d8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da2d8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da2d8-111">Permission type</span></span>      | <span data-ttu-id="da2d8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da2d8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da2d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da2d8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="da2d8-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2d8-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="da2d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da2d8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da2d8-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da2d8-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="da2d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da2d8-117">Application</span></span> | <span data-ttu-id="da2d8-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2d8-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da2d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da2d8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="da2d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da2d8-120">Request headers</span></span>
| <span data-ttu-id="da2d8-121">名称</span><span class="sxs-lookup"><span data-stu-id="da2d8-121">Name</span></span>       | <span data-ttu-id="da2d8-122">类型</span><span class="sxs-lookup"><span data-stu-id="da2d8-122">Type</span></span> | <span data-ttu-id="da2d8-123">说明</span><span class="sxs-lookup"><span data-stu-id="da2d8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da2d8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2d8-124">Authorization</span></span>  | <span data-ttu-id="da2d8-125">string</span><span class="sxs-lookup"><span data-stu-id="da2d8-125">string</span></span>  | <span data-ttu-id="da2d8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da2d8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da2d8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da2d8-128">Content-Type</span></span> | <span data-ttu-id="da2d8-129">string</span><span class="sxs-lookup"><span data-stu-id="da2d8-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="da2d8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="da2d8-130">Request body</span></span>
<span data-ttu-id="da2d8-131">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="da2d8-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="da2d8-132">如果不需要，可以发送空正文。</span><span class="sxs-lookup"><span data-stu-id="da2d8-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="da2d8-133">参数</span><span class="sxs-lookup"><span data-stu-id="da2d8-133">Parameter</span></span>    | <span data-ttu-id="da2d8-134">类型</span><span class="sxs-lookup"><span data-stu-id="da2d8-134">Type</span></span>   |<span data-ttu-id="da2d8-135">说明</span><span class="sxs-lookup"><span data-stu-id="da2d8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da2d8-136">groupId</span><span class="sxs-lookup"><span data-stu-id="da2d8-136">groupId</span></span>|<span data-ttu-id="da2d8-137">String</span><span class="sxs-lookup"><span data-stu-id="da2d8-137">String</span></span>|<span data-ttu-id="da2d8-138">要复制到的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="da2d8-138">The id of the group to copy to.</span></span> <span data-ttu-id="da2d8-139">仅在复制到组时Microsoft 365使用。</span><span class="sxs-lookup"><span data-stu-id="da2d8-139">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="da2d8-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="da2d8-140">renameAs</span></span>|<span data-ttu-id="da2d8-141">String</span><span class="sxs-lookup"><span data-stu-id="da2d8-141">String</span></span>|<span data-ttu-id="da2d8-142">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="da2d8-142">The name of the copy.</span></span> <span data-ttu-id="da2d8-143">默认为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="da2d8-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="da2d8-144">响应</span><span class="sxs-lookup"><span data-stu-id="da2d8-144">Response</span></span>

<span data-ttu-id="da2d8-145">如果成功，此方法返回 响应 `202 Accepted` 代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="da2d8-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="da2d8-146">轮询Operation-Location [终结点，获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="da2d8-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="da2d8-147">示例</span><span class="sxs-lookup"><span data-stu-id="da2d8-147">Example</span></span>
<span data-ttu-id="da2d8-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="da2d8-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="da2d8-149">请求</span><span class="sxs-lookup"><span data-stu-id="da2d8-149">Request</span></span>
<span data-ttu-id="da2d8-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da2d8-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da2d8-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="da2d8-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="da2d8-152">C#</span><span class="sxs-lookup"><span data-stu-id="da2d8-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da2d8-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da2d8-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da2d8-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da2d8-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da2d8-155">Java</span><span class="sxs-lookup"><span data-stu-id="da2d8-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da2d8-156">响应</span><span class="sxs-lookup"><span data-stu-id="da2d8-156">Response</span></span>
<span data-ttu-id="da2d8-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="da2d8-157">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

