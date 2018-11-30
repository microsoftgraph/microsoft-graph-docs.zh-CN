---
title: 'notebook: copyNotebook'
description: 将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。
ms.openlocfilehash: 4d22c6904f14d0ccc5d4f3de35cdf46fbd3afd6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045334"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="878d5-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="878d5-104">notebook: copyNotebook</span></span>

> <span data-ttu-id="878d5-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="878d5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="878d5-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="878d5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="878d5-p103">将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="878d5-p103">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="878d5-109">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="878d5-109">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="878d5-110">权限</span><span class="sxs-lookup"><span data-stu-id="878d5-110">Permissions</span></span>
<span data-ttu-id="878d5-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="878d5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="878d5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="878d5-113">Permission type</span></span>      | <span data-ttu-id="878d5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="878d5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="878d5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="878d5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="878d5-116">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="878d5-116">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="878d5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="878d5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="878d5-118">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="878d5-118">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="878d5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="878d5-119">Application</span></span> | <span data-ttu-id="878d5-120">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="878d5-120">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="878d5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="878d5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="878d5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="878d5-122">Request headers</span></span>
| <span data-ttu-id="878d5-123">名称</span><span class="sxs-lookup"><span data-stu-id="878d5-123">Name</span></span>       | <span data-ttu-id="878d5-124">类型</span><span class="sxs-lookup"><span data-stu-id="878d5-124">Type</span></span> | <span data-ttu-id="878d5-125">说明</span><span class="sxs-lookup"><span data-stu-id="878d5-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="878d5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="878d5-126">Authorization</span></span>  | <span data-ttu-id="878d5-127">string</span><span class="sxs-lookup"><span data-stu-id="878d5-127">string</span></span>  | <span data-ttu-id="878d5-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="878d5-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="878d5-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="878d5-130">Content-Type</span></span> | <span data-ttu-id="878d5-131">string</span><span class="sxs-lookup"><span data-stu-id="878d5-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="878d5-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="878d5-132">Request body</span></span>
<span data-ttu-id="878d5-p106">在请求正文中，提供包含操作所需参数的 JSON 对象。如果无需任何参数，则可以发送空的正文。</span><span class="sxs-lookup"><span data-stu-id="878d5-p106">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="878d5-135">参数</span><span class="sxs-lookup"><span data-stu-id="878d5-135">Parameter</span></span>    | <span data-ttu-id="878d5-136">类型</span><span class="sxs-lookup"><span data-stu-id="878d5-136">Type</span></span>   |<span data-ttu-id="878d5-137">说明</span><span class="sxs-lookup"><span data-stu-id="878d5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="878d5-138">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="878d5-138">siteCollectionId</span></span>|<span data-ttu-id="878d5-139">字符串</span><span class="sxs-lookup"><span data-stu-id="878d5-139">String</span></span>|<span data-ttu-id="878d5-140">若要将复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="878d5-140">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="878d5-141">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="878d5-141">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="878d5-142">siteId</span><span class="sxs-lookup"><span data-stu-id="878d5-142">siteId</span></span>|<span data-ttu-id="878d5-143">字符串</span><span class="sxs-lookup"><span data-stu-id="878d5-143">String</span></span>|<span data-ttu-id="878d5-144">SharePoint 网站复制到的 id。</span><span class="sxs-lookup"><span data-stu-id="878d5-144">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="878d5-145">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="878d5-145">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="878d5-146">groupId</span><span class="sxs-lookup"><span data-stu-id="878d5-146">groupId</span></span>|<span data-ttu-id="878d5-147">字符串</span><span class="sxs-lookup"><span data-stu-id="878d5-147">String</span></span>|<span data-ttu-id="878d5-p109">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="878d5-p109">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="878d5-150">renameAs</span><span class="sxs-lookup"><span data-stu-id="878d5-150">renameAs</span></span>|<span data-ttu-id="878d5-151">字符串</span><span class="sxs-lookup"><span data-stu-id="878d5-151">String</span></span>|<span data-ttu-id="878d5-p110">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="878d5-p110">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="878d5-154">响应</span><span class="sxs-lookup"><span data-stu-id="878d5-154">Response</span></span>

<span data-ttu-id="878d5-p111">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="878d5-p111">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="878d5-157">示例</span><span class="sxs-lookup"><span data-stu-id="878d5-157">Example</span></span>
<span data-ttu-id="878d5-158">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="878d5-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="878d5-159">请求</span><span class="sxs-lookup"><span data-stu-id="878d5-159">Request</span></span>
<span data-ttu-id="878d5-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="878d5-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="878d5-161">响应</span><span class="sxs-lookup"><span data-stu-id="878d5-161">Response</span></span>
<span data-ttu-id="878d5-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="878d5-162">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
