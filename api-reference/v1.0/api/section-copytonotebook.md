---
title: 部分： copyToNotebook
description: 将分区复制到特定笔记本。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f2dbd05ebca4f4aad45c40cb1b8b31ca73685144
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088956"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="b7b45-103">部分： copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="b7b45-103">section: copyToNotebook</span></span>

<span data-ttu-id="b7b45-104">命名空间： microsoft. graph 将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="b7b45-104">Namespace: microsoft.graph Copies a section to a specific notebook.</span></span>

<span data-ttu-id="b7b45-105">对于复制操作，请遵循异步调用模式：首先调用复制操作，然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="b7b45-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7b45-106">权限</span><span class="sxs-lookup"><span data-stu-id="b7b45-106">Permissions</span></span>
<span data-ttu-id="b7b45-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7b45-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7b45-109">Permission type</span></span>      | <span data-ttu-id="b7b45-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7b45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7b45-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b45-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7b45-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b45-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7b45-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7b45-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7b45-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b7b45-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7b45-115">Application</span></span> | <span data-ttu-id="b7b45-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b45-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7b45-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7b45-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="b7b45-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7b45-118">Request headers</span></span>
| <span data-ttu-id="b7b45-119">名称</span><span class="sxs-lookup"><span data-stu-id="b7b45-119">Name</span></span>       | <span data-ttu-id="b7b45-120">类型</span><span class="sxs-lookup"><span data-stu-id="b7b45-120">Type</span></span> | <span data-ttu-id="b7b45-121">说明</span><span class="sxs-lookup"><span data-stu-id="b7b45-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b7b45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7b45-122">Authorization</span></span>  | <span data-ttu-id="b7b45-123">string</span><span class="sxs-lookup"><span data-stu-id="b7b45-123">string</span></span>  | <span data-ttu-id="b7b45-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7b45-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7b45-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7b45-126">Content-Type</span></span> | <span data-ttu-id="b7b45-127">string</span><span class="sxs-lookup"><span data-stu-id="b7b45-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b7b45-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7b45-128">Request body</span></span>
<span data-ttu-id="b7b45-129">在请求正文中，提供一个 JSON 对象，其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="b7b45-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="b7b45-130">参数</span><span class="sxs-lookup"><span data-stu-id="b7b45-130">Parameter</span></span>    | <span data-ttu-id="b7b45-131">类型</span><span class="sxs-lookup"><span data-stu-id="b7b45-131">Type</span></span>   |<span data-ttu-id="b7b45-132">说明</span><span class="sxs-lookup"><span data-stu-id="b7b45-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7b45-133">groupId</span><span class="sxs-lookup"><span data-stu-id="b7b45-133">groupId</span></span>|<span data-ttu-id="b7b45-134">String</span><span class="sxs-lookup"><span data-stu-id="b7b45-134">String</span></span>|<span data-ttu-id="b7b45-135">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="b7b45-135">The id of the group to copy to.</span></span> <span data-ttu-id="b7b45-136">仅在复制到 Microsoft 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="b7b45-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="b7b45-137">id</span><span class="sxs-lookup"><span data-stu-id="b7b45-137">id</span></span>|<span data-ttu-id="b7b45-138">String</span><span class="sxs-lookup"><span data-stu-id="b7b45-138">String</span></span>|<span data-ttu-id="b7b45-139">必需。</span><span class="sxs-lookup"><span data-stu-id="b7b45-139">Required.</span></span> <span data-ttu-id="b7b45-140">目标笔记本的 id。</span><span class="sxs-lookup"><span data-stu-id="b7b45-140">The id of the destination notebook.</span></span> |
|<span data-ttu-id="b7b45-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="b7b45-141">renameAs</span></span>|<span data-ttu-id="b7b45-142">String</span><span class="sxs-lookup"><span data-stu-id="b7b45-142">String</span></span>|<span data-ttu-id="b7b45-143">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="b7b45-143">The name of the copy.</span></span> <span data-ttu-id="b7b45-144">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="b7b45-144">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="b7b45-145">响应</span><span class="sxs-lookup"><span data-stu-id="b7b45-145">Response</span></span>

<span data-ttu-id="b7b45-146">如果成功，此方法将返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="b7b45-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="b7b45-147">轮询操作-位置终结点以 [获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="b7b45-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b7b45-148">示例</span><span class="sxs-lookup"><span data-stu-id="b7b45-148">Example</span></span>
<span data-ttu-id="b7b45-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b7b45-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7b45-150">请求</span><span class="sxs-lookup"><span data-stu-id="b7b45-150">Request</span></span>
<span data-ttu-id="b7b45-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7b45-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7b45-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b45-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b7b45-153">C#</span><span class="sxs-lookup"><span data-stu-id="b7b45-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7b45-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7b45-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7b45-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7b45-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7b45-156">Java</span><span class="sxs-lookup"><span data-stu-id="b7b45-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b7b45-157">响应</span><span class="sxs-lookup"><span data-stu-id="b7b45-157">Response</span></span>
<span data-ttu-id="b7b45-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b7b45-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

