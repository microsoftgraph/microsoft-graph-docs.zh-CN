---
title: 页面： copyToSection
description: 将页面复制到特定分区。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2f37685212c48f3afe75a9c7daf2776f08aa92f6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896432"
---
# <a name="page-copytosection"></a><span data-ttu-id="1360c-103">页面： copyToSection</span><span class="sxs-lookup"><span data-stu-id="1360c-103">page: copyToSection</span></span>

<span data-ttu-id="1360c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1360c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1360c-105">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="1360c-105">Copies a page to a specific section.</span></span>

<span data-ttu-id="1360c-106">对于复制操作，请遵循异步调用模式：首先调用复制操作，然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="1360c-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="1360c-107">权限</span><span class="sxs-lookup"><span data-stu-id="1360c-107">Permissions</span></span>
<span data-ttu-id="1360c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1360c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1360c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1360c-110">Permission type</span></span>      | <span data-ttu-id="1360c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1360c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1360c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1360c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1360c-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1360c-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1360c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1360c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1360c-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1360c-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1360c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1360c-116">Application</span></span> | <span data-ttu-id="1360c-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1360c-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1360c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1360c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="1360c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1360c-119">Request headers</span></span>
| <span data-ttu-id="1360c-120">名称</span><span class="sxs-lookup"><span data-stu-id="1360c-120">Name</span></span>       | <span data-ttu-id="1360c-121">类型</span><span class="sxs-lookup"><span data-stu-id="1360c-121">Type</span></span> | <span data-ttu-id="1360c-122">说明</span><span class="sxs-lookup"><span data-stu-id="1360c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1360c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1360c-123">Authorization</span></span>  | <span data-ttu-id="1360c-124">string</span><span class="sxs-lookup"><span data-stu-id="1360c-124">string</span></span>  | <span data-ttu-id="1360c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1360c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1360c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1360c-127">Content-Type</span></span> | <span data-ttu-id="1360c-128">string</span><span class="sxs-lookup"><span data-stu-id="1360c-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1360c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1360c-129">Request body</span></span>
<span data-ttu-id="1360c-130">在请求正文中，提供一个 JSON 对象，其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="1360c-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="1360c-131">参数</span><span class="sxs-lookup"><span data-stu-id="1360c-131">Parameter</span></span>    | <span data-ttu-id="1360c-132">类型</span><span class="sxs-lookup"><span data-stu-id="1360c-132">Type</span></span>   |<span data-ttu-id="1360c-133">说明</span><span class="sxs-lookup"><span data-stu-id="1360c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1360c-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="1360c-134">siteCollectionId</span></span>|<span data-ttu-id="1360c-135">String</span><span class="sxs-lookup"><span data-stu-id="1360c-135">String</span></span>|<span data-ttu-id="1360c-136">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="1360c-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="1360c-137">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="1360c-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="1360c-138">siteId</span><span class="sxs-lookup"><span data-stu-id="1360c-138">siteId</span></span>|<span data-ttu-id="1360c-139">String</span><span class="sxs-lookup"><span data-stu-id="1360c-139">String</span></span>|<span data-ttu-id="1360c-140">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="1360c-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="1360c-141">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="1360c-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="1360c-142">groupId</span><span class="sxs-lookup"><span data-stu-id="1360c-142">groupId</span></span>|<span data-ttu-id="1360c-143">String</span><span class="sxs-lookup"><span data-stu-id="1360c-143">String</span></span>|<span data-ttu-id="1360c-144">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="1360c-144">The id of the group to copy to.</span></span> <span data-ttu-id="1360c-145">仅在复制到 Microsoft 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="1360c-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="1360c-146">id</span><span class="sxs-lookup"><span data-stu-id="1360c-146">id</span></span>|<span data-ttu-id="1360c-147">String</span><span class="sxs-lookup"><span data-stu-id="1360c-147">String</span></span>|<span data-ttu-id="1360c-148">必填。</span><span class="sxs-lookup"><span data-stu-id="1360c-148">Required.</span></span> <span data-ttu-id="1360c-149">目标部分的 id。</span><span class="sxs-lookup"><span data-stu-id="1360c-149">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="1360c-150">响应</span><span class="sxs-lookup"><span data-stu-id="1360c-150">Response</span></span>

<span data-ttu-id="1360c-151">如果成功，此方法将返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="1360c-151">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="1360c-152">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="1360c-152">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="1360c-153">示例</span><span class="sxs-lookup"><span data-stu-id="1360c-153">Example</span></span>
<span data-ttu-id="1360c-154">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1360c-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1360c-155">请求</span><span class="sxs-lookup"><span data-stu-id="1360c-155">Request</span></span>
<span data-ttu-id="1360c-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1360c-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1360c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1360c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1360c-158">C#</span><span class="sxs-lookup"><span data-stu-id="1360c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1360c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1360c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1360c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1360c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1360c-161">响应</span><span class="sxs-lookup"><span data-stu-id="1360c-161">Response</span></span>
<span data-ttu-id="1360c-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1360c-162">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
