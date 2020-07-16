---
title: 笔记本： copyNotebook
description: 将笔记本复制到目标文档库中的 "笔记本" 文件夹。 如果文件夹不存在，则创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 028b6b577e9a018be0cfc97264b6344b51dd8ed2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44894849"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="e5457-104">笔记本： copyNotebook</span><span class="sxs-lookup"><span data-stu-id="e5457-104">notebook: copyNotebook</span></span>

<span data-ttu-id="e5457-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5457-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5457-106">将笔记本复制到目标文档库中的 "笔记本" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="e5457-106">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="e5457-107">如果文件夹不存在，则创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="e5457-107">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="e5457-108">对于复制操作，请遵循异步调用模式：首先调用复制操作，然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="e5457-108">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5457-109">权限</span><span class="sxs-lookup"><span data-stu-id="e5457-109">Permissions</span></span>
<span data-ttu-id="e5457-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5457-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5457-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5457-112">Permission type</span></span>      | <span data-ttu-id="e5457-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5457-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5457-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5457-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e5457-115">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5457-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5457-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5457-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5457-117">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5457-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e5457-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5457-118">Application</span></span> | <span data-ttu-id="e5457-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5457-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5457-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5457-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="e5457-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5457-121">Request headers</span></span>
| <span data-ttu-id="e5457-122">名称</span><span class="sxs-lookup"><span data-stu-id="e5457-122">Name</span></span>       | <span data-ttu-id="e5457-123">类型</span><span class="sxs-lookup"><span data-stu-id="e5457-123">Type</span></span> | <span data-ttu-id="e5457-124">说明</span><span class="sxs-lookup"><span data-stu-id="e5457-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5457-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5457-125">Authorization</span></span>  | <span data-ttu-id="e5457-126">string</span><span class="sxs-lookup"><span data-stu-id="e5457-126">string</span></span>  | <span data-ttu-id="e5457-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5457-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5457-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5457-129">Content-Type</span></span> | <span data-ttu-id="e5457-130">string</span><span class="sxs-lookup"><span data-stu-id="e5457-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e5457-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5457-131">Request body</span></span>
<span data-ttu-id="e5457-132">在请求正文中，提供一个 JSON 对象，其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="e5457-132">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="e5457-133">如果无需，可以发送空正文。</span><span class="sxs-lookup"><span data-stu-id="e5457-133">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="e5457-134">参数</span><span class="sxs-lookup"><span data-stu-id="e5457-134">Parameter</span></span>    | <span data-ttu-id="e5457-135">类型</span><span class="sxs-lookup"><span data-stu-id="e5457-135">Type</span></span>   |<span data-ttu-id="e5457-136">说明</span><span class="sxs-lookup"><span data-stu-id="e5457-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5457-137">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="e5457-137">siteCollectionId</span></span>|<span data-ttu-id="e5457-138">String</span><span class="sxs-lookup"><span data-stu-id="e5457-138">String</span></span>|<span data-ttu-id="e5457-139">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="e5457-139">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="e5457-140">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="e5457-140">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="e5457-141">siteId</span><span class="sxs-lookup"><span data-stu-id="e5457-141">siteId</span></span>|<span data-ttu-id="e5457-142">String</span><span class="sxs-lookup"><span data-stu-id="e5457-142">String</span></span>|<span data-ttu-id="e5457-143">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="e5457-143">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="e5457-144">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="e5457-144">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="e5457-145">groupId</span><span class="sxs-lookup"><span data-stu-id="e5457-145">groupId</span></span>|<span data-ttu-id="e5457-146">String</span><span class="sxs-lookup"><span data-stu-id="e5457-146">String</span></span>|<span data-ttu-id="e5457-147">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="e5457-147">The id of the group to copy to.</span></span> <span data-ttu-id="e5457-148">仅在复制到 Microsoft 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="e5457-148">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="e5457-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="e5457-149">renameAs</span></span>|<span data-ttu-id="e5457-150">String</span><span class="sxs-lookup"><span data-stu-id="e5457-150">String</span></span>|<span data-ttu-id="e5457-151">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="e5457-151">The name of the copy.</span></span> <span data-ttu-id="e5457-152">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="e5457-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="e5457-153">响应</span><span class="sxs-lookup"><span data-stu-id="e5457-153">Response</span></span>

<span data-ttu-id="e5457-154">如果成功，此方法将返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="e5457-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="e5457-155">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="e5457-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="e5457-156">示例</span><span class="sxs-lookup"><span data-stu-id="e5457-156">Example</span></span>
<span data-ttu-id="e5457-157">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e5457-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5457-158">请求</span><span class="sxs-lookup"><span data-stu-id="e5457-158">Request</span></span>
<span data-ttu-id="e5457-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5457-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5457-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5457-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e5457-161">C#</span><span class="sxs-lookup"><span data-stu-id="e5457-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5457-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5457-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5457-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5457-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5457-164">响应</span><span class="sxs-lookup"><span data-stu-id="e5457-164">Response</span></span>
<span data-ttu-id="e5457-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5457-165">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
