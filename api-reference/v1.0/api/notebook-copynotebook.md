---
title: '笔记本: copyNotebook'
description: 将笔记本复制到目标文档库中的 "笔记本" 文件夹。 如果文件夹不存在, 则创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d29b5b8c05fe85ebf98d77872cb143979150a341
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612174"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="57b82-104">笔记本: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="57b82-104">notebook: copyNotebook</span></span>
<span data-ttu-id="57b82-105">将笔记本复制到目标文档库中的 "笔记本" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="57b82-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="57b82-106">如果文件夹不存在, 则创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="57b82-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="57b82-107">对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="57b82-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="57b82-108">权限</span><span class="sxs-lookup"><span data-stu-id="57b82-108">Permissions</span></span>
<span data-ttu-id="57b82-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57b82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57b82-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="57b82-111">Permission type</span></span>      | <span data-ttu-id="57b82-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57b82-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57b82-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57b82-113">Delegated (work or school account)</span></span> | <span data-ttu-id="57b82-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b82-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="57b82-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57b82-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57b82-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57b82-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="57b82-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="57b82-117">Application</span></span> | <span data-ttu-id="57b82-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b82-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57b82-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57b82-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="57b82-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="57b82-120">Request headers</span></span>
| <span data-ttu-id="57b82-121">名称</span><span class="sxs-lookup"><span data-stu-id="57b82-121">Name</span></span>       | <span data-ttu-id="57b82-122">类型</span><span class="sxs-lookup"><span data-stu-id="57b82-122">Type</span></span> | <span data-ttu-id="57b82-123">说明</span><span class="sxs-lookup"><span data-stu-id="57b82-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57b82-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="57b82-124">Authorization</span></span>  | <span data-ttu-id="57b82-125">string</span><span class="sxs-lookup"><span data-stu-id="57b82-125">string</span></span>  | <span data-ttu-id="57b82-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57b82-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57b82-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57b82-128">Content-Type</span></span> | <span data-ttu-id="57b82-129">string</span><span class="sxs-lookup"><span data-stu-id="57b82-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="57b82-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="57b82-130">Request body</span></span>
<span data-ttu-id="57b82-131">在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="57b82-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="57b82-132">如果无需, 可以发送空正文。</span><span class="sxs-lookup"><span data-stu-id="57b82-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="57b82-133">参数</span><span class="sxs-lookup"><span data-stu-id="57b82-133">Parameter</span></span>    | <span data-ttu-id="57b82-134">类型</span><span class="sxs-lookup"><span data-stu-id="57b82-134">Type</span></span>   |<span data-ttu-id="57b82-135">说明</span><span class="sxs-lookup"><span data-stu-id="57b82-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57b82-136">groupId</span><span class="sxs-lookup"><span data-stu-id="57b82-136">groupId</span></span>|<span data-ttu-id="57b82-137">String</span><span class="sxs-lookup"><span data-stu-id="57b82-137">String</span></span>|<span data-ttu-id="57b82-138">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="57b82-138">The id of the group to copy to.</span></span> <span data-ttu-id="57b82-139">仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="57b82-139">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="57b82-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="57b82-140">renameAs</span></span>|<span data-ttu-id="57b82-141">字符串</span><span class="sxs-lookup"><span data-stu-id="57b82-141">String</span></span>|<span data-ttu-id="57b82-142">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="57b82-142">The name of the copy.</span></span> <span data-ttu-id="57b82-143">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="57b82-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="57b82-144">响应</span><span class="sxs-lookup"><span data-stu-id="57b82-144">Response</span></span>

<span data-ttu-id="57b82-145">如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。</span><span class="sxs-lookup"><span data-stu-id="57b82-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="57b82-146">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="57b82-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="57b82-147">示例</span><span class="sxs-lookup"><span data-stu-id="57b82-147">Example</span></span>
<span data-ttu-id="57b82-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="57b82-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57b82-149">请求</span><span class="sxs-lookup"><span data-stu-id="57b82-149">Request</span></span>
<span data-ttu-id="57b82-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57b82-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="57b82-151">响应</span><span class="sxs-lookup"><span data-stu-id="57b82-151">Response</span></span>
<span data-ttu-id="57b82-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="57b82-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="57b82-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="57b82-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="57b82-154">语言</span><span class="sxs-lookup"><span data-stu-id="57b82-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57b82-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="57b82-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
