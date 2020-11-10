---
title: 部分： copyToNotebook
description: 将分区复制到特定笔记本。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5a1d99f93df7acd6c964ae690784ab3df8cca43c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978682"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="760eb-103">部分： copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="760eb-103">section: copyToNotebook</span></span>

<span data-ttu-id="760eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="760eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="760eb-105">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="760eb-105">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="760eb-106">对于复制操作，请遵循异步调用模式：首先调用复制操作，然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="760eb-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="760eb-107">权限</span><span class="sxs-lookup"><span data-stu-id="760eb-107">Permissions</span></span>
<span data-ttu-id="760eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="760eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="760eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="760eb-110">Permission type</span></span>      | <span data-ttu-id="760eb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="760eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="760eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="760eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="760eb-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="760eb-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="760eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="760eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="760eb-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="760eb-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="760eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="760eb-116">Application</span></span> | <span data-ttu-id="760eb-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="760eb-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="760eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="760eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="760eb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="760eb-119">Request headers</span></span>
| <span data-ttu-id="760eb-120">名称</span><span class="sxs-lookup"><span data-stu-id="760eb-120">Name</span></span>       | <span data-ttu-id="760eb-121">类型</span><span class="sxs-lookup"><span data-stu-id="760eb-121">Type</span></span> | <span data-ttu-id="760eb-122">说明</span><span class="sxs-lookup"><span data-stu-id="760eb-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="760eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="760eb-123">Authorization</span></span>  | <span data-ttu-id="760eb-124">string</span><span class="sxs-lookup"><span data-stu-id="760eb-124">string</span></span>  | <span data-ttu-id="760eb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="760eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="760eb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="760eb-127">Content-Type</span></span> | <span data-ttu-id="760eb-128">string</span><span class="sxs-lookup"><span data-stu-id="760eb-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="760eb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="760eb-129">Request body</span></span>
<span data-ttu-id="760eb-130">在请求正文中，提供一个 JSON 对象，其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="760eb-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="760eb-131">参数</span><span class="sxs-lookup"><span data-stu-id="760eb-131">Parameter</span></span>    | <span data-ttu-id="760eb-132">类型</span><span class="sxs-lookup"><span data-stu-id="760eb-132">Type</span></span>   |<span data-ttu-id="760eb-133">说明</span><span class="sxs-lookup"><span data-stu-id="760eb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="760eb-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="760eb-134">siteCollectionId</span></span>|<span data-ttu-id="760eb-135">String</span><span class="sxs-lookup"><span data-stu-id="760eb-135">String</span></span>|<span data-ttu-id="760eb-136">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="760eb-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="760eb-137">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="760eb-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="760eb-138">siteId</span><span class="sxs-lookup"><span data-stu-id="760eb-138">siteId</span></span>|<span data-ttu-id="760eb-139">String</span><span class="sxs-lookup"><span data-stu-id="760eb-139">String</span></span>|<span data-ttu-id="760eb-140">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="760eb-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="760eb-141">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="760eb-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="760eb-142">groupId</span><span class="sxs-lookup"><span data-stu-id="760eb-142">groupId</span></span>|<span data-ttu-id="760eb-143">String</span><span class="sxs-lookup"><span data-stu-id="760eb-143">String</span></span>|<span data-ttu-id="760eb-144">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="760eb-144">The id of the group to copy to.</span></span> <span data-ttu-id="760eb-145">仅在复制到 Microsoft 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="760eb-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="760eb-146">id</span><span class="sxs-lookup"><span data-stu-id="760eb-146">id</span></span>|<span data-ttu-id="760eb-147">String</span><span class="sxs-lookup"><span data-stu-id="760eb-147">String</span></span>|<span data-ttu-id="760eb-148">必填。</span><span class="sxs-lookup"><span data-stu-id="760eb-148">Required.</span></span> <span data-ttu-id="760eb-149">目标笔记本的 id。</span><span class="sxs-lookup"><span data-stu-id="760eb-149">The id of the destination notebook.</span></span> |
|<span data-ttu-id="760eb-150">renameAs</span><span class="sxs-lookup"><span data-stu-id="760eb-150">renameAs</span></span>|<span data-ttu-id="760eb-151">String</span><span class="sxs-lookup"><span data-stu-id="760eb-151">String</span></span>|<span data-ttu-id="760eb-152">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="760eb-152">The name of the copy.</span></span> <span data-ttu-id="760eb-153">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="760eb-153">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="760eb-154">响应</span><span class="sxs-lookup"><span data-stu-id="760eb-154">Response</span></span>

<span data-ttu-id="760eb-155">如果成功，此方法将返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="760eb-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="760eb-156">轮询 Operation-Location 终结点以 [获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="760eb-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="760eb-157">示例</span><span class="sxs-lookup"><span data-stu-id="760eb-157">Example</span></span>
<span data-ttu-id="760eb-158">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="760eb-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="760eb-159">请求</span><span class="sxs-lookup"><span data-stu-id="760eb-159">Request</span></span>
<span data-ttu-id="760eb-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="760eb-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="760eb-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="760eb-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="760eb-162">C#</span><span class="sxs-lookup"><span data-stu-id="760eb-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="760eb-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="760eb-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="760eb-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="760eb-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="760eb-165">Java</span><span class="sxs-lookup"><span data-stu-id="760eb-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="760eb-166">响应</span><span class="sxs-lookup"><span data-stu-id="760eb-166">Response</span></span>
<span data-ttu-id="760eb-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="760eb-167">Here is an example of the response.</span></span>
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


