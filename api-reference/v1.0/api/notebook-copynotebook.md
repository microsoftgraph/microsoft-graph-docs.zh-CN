---
title: '笔记本: copyNotebook'
description: 将笔记本复制到目标文档库中的 "笔记本" 文件夹。 如果文件夹不存在, 则创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 473d2904c2b5ea5b44aaa85cc5a535cda6318535
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374517"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="5412c-104">笔记本: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="5412c-104">notebook: copyNotebook</span></span>
<span data-ttu-id="5412c-105">将笔记本复制到目标文档库中的 "笔记本" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="5412c-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="5412c-106">如果文件夹不存在, 则创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="5412c-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="5412c-107">对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="5412c-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="5412c-108">权限</span><span class="sxs-lookup"><span data-stu-id="5412c-108">Permissions</span></span>
<span data-ttu-id="5412c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5412c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5412c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5412c-111">Permission type</span></span>      | <span data-ttu-id="5412c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5412c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5412c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5412c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5412c-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5412c-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5412c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5412c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5412c-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5412c-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5412c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5412c-117">Application</span></span> | <span data-ttu-id="5412c-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5412c-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5412c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5412c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="5412c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5412c-120">Request headers</span></span>
| <span data-ttu-id="5412c-121">名称</span><span class="sxs-lookup"><span data-stu-id="5412c-121">Name</span></span>       | <span data-ttu-id="5412c-122">类型</span><span class="sxs-lookup"><span data-stu-id="5412c-122">Type</span></span> | <span data-ttu-id="5412c-123">说明</span><span class="sxs-lookup"><span data-stu-id="5412c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5412c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5412c-124">Authorization</span></span>  | <span data-ttu-id="5412c-125">string</span><span class="sxs-lookup"><span data-stu-id="5412c-125">string</span></span>  | <span data-ttu-id="5412c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5412c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5412c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5412c-128">Content-Type</span></span> | <span data-ttu-id="5412c-129">string</span><span class="sxs-lookup"><span data-stu-id="5412c-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5412c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5412c-130">Request body</span></span>
<span data-ttu-id="5412c-131">在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="5412c-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="5412c-132">如果无需, 可以发送空正文。</span><span class="sxs-lookup"><span data-stu-id="5412c-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="5412c-133">参数</span><span class="sxs-lookup"><span data-stu-id="5412c-133">Parameter</span></span>    | <span data-ttu-id="5412c-134">类型</span><span class="sxs-lookup"><span data-stu-id="5412c-134">Type</span></span>   |<span data-ttu-id="5412c-135">说明</span><span class="sxs-lookup"><span data-stu-id="5412c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5412c-136">groupId</span><span class="sxs-lookup"><span data-stu-id="5412c-136">groupId</span></span>|<span data-ttu-id="5412c-137">String</span><span class="sxs-lookup"><span data-stu-id="5412c-137">String</span></span>|<span data-ttu-id="5412c-138">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="5412c-138">The id of the group to copy to.</span></span> <span data-ttu-id="5412c-139">仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="5412c-139">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="5412c-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="5412c-140">renameAs</span></span>|<span data-ttu-id="5412c-141">String</span><span class="sxs-lookup"><span data-stu-id="5412c-141">String</span></span>|<span data-ttu-id="5412c-142">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="5412c-142">The name of the copy.</span></span> <span data-ttu-id="5412c-143">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="5412c-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="5412c-144">响应</span><span class="sxs-lookup"><span data-stu-id="5412c-144">Response</span></span>

<span data-ttu-id="5412c-145">如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。</span><span class="sxs-lookup"><span data-stu-id="5412c-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="5412c-146">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="5412c-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="5412c-147">示例</span><span class="sxs-lookup"><span data-stu-id="5412c-147">Example</span></span>
<span data-ttu-id="5412c-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5412c-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5412c-149">请求</span><span class="sxs-lookup"><span data-stu-id="5412c-149">Request</span></span>
<span data-ttu-id="5412c-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5412c-150">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5412c-151">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5412c-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5412c-152">C#</span><span class="sxs-lookup"><span data-stu-id="5412c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5412c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5412c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5412c-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="5412c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5412c-155">Java</span><span class="sxs-lookup"><span data-stu-id="5412c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5412c-156">响应</span><span class="sxs-lookup"><span data-stu-id="5412c-156">Response</span></span>
<span data-ttu-id="5412c-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5412c-157">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
