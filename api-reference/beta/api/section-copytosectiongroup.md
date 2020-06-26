---
title: 部分： copyToSectionGroup
description: 将分区复制到特定分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: dc5ad2f046d13bde7d562d5221174cc9138a4b9e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896565"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="4917d-103">部分： copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="4917d-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="4917d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4917d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4917d-105">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="4917d-105">Copies a section to a specific section group.</span></span>

<span data-ttu-id="4917d-106">对于复制操作，请遵循异步调用模式：首先调用复制操作，然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="4917d-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="4917d-107">权限</span><span class="sxs-lookup"><span data-stu-id="4917d-107">Permissions</span></span>
<span data-ttu-id="4917d-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4917d-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4917d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4917d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4917d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4917d-110">Permission type</span></span>      | <span data-ttu-id="4917d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4917d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4917d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4917d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4917d-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4917d-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4917d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4917d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4917d-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4917d-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4917d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4917d-116">Application</span></span> | <span data-ttu-id="4917d-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4917d-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4917d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4917d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="4917d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4917d-119">Request headers</span></span>
| <span data-ttu-id="4917d-120">名称</span><span class="sxs-lookup"><span data-stu-id="4917d-120">Name</span></span>       | <span data-ttu-id="4917d-121">类型</span><span class="sxs-lookup"><span data-stu-id="4917d-121">Type</span></span> | <span data-ttu-id="4917d-122">说明</span><span class="sxs-lookup"><span data-stu-id="4917d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4917d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4917d-123">Authorization</span></span>  | <span data-ttu-id="4917d-124">string</span><span class="sxs-lookup"><span data-stu-id="4917d-124">string</span></span>  | <span data-ttu-id="4917d-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4917d-125">Bearer {token}.</span></span> <span data-ttu-id="4917d-126">Required.</span><span class="sxs-lookup"><span data-stu-id="4917d-126">Required.</span></span> |
| <span data-ttu-id="4917d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4917d-127">Content-Type</span></span> | <span data-ttu-id="4917d-128">string</span><span class="sxs-lookup"><span data-stu-id="4917d-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4917d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4917d-129">Request body</span></span>
<span data-ttu-id="4917d-130">在请求正文中，提供一个 JSON 对象，其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="4917d-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="4917d-131">参数</span><span class="sxs-lookup"><span data-stu-id="4917d-131">Parameter</span></span>    | <span data-ttu-id="4917d-132">类型</span><span class="sxs-lookup"><span data-stu-id="4917d-132">Type</span></span>   |<span data-ttu-id="4917d-133">说明</span><span class="sxs-lookup"><span data-stu-id="4917d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4917d-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="4917d-134">siteCollectionId</span></span>|<span data-ttu-id="4917d-135">String</span><span class="sxs-lookup"><span data-stu-id="4917d-135">String</span></span>|<span data-ttu-id="4917d-136">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="4917d-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="4917d-137">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="4917d-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="4917d-138">siteId</span><span class="sxs-lookup"><span data-stu-id="4917d-138">siteId</span></span>|<span data-ttu-id="4917d-139">String</span><span class="sxs-lookup"><span data-stu-id="4917d-139">String</span></span>|<span data-ttu-id="4917d-140">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="4917d-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="4917d-141">仅在复制到 SharePoint 网站时使用。</span><span class="sxs-lookup"><span data-stu-id="4917d-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="4917d-142">groupId</span><span class="sxs-lookup"><span data-stu-id="4917d-142">groupId</span></span>|<span data-ttu-id="4917d-143">String</span><span class="sxs-lookup"><span data-stu-id="4917d-143">String</span></span>|<span data-ttu-id="4917d-144">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="4917d-144">The id of the group to copy to.</span></span> <span data-ttu-id="4917d-145">仅在复制到 Microsoft 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="4917d-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="4917d-146">id</span><span class="sxs-lookup"><span data-stu-id="4917d-146">id</span></span>|<span data-ttu-id="4917d-147">String</span><span class="sxs-lookup"><span data-stu-id="4917d-147">String</span></span>|<span data-ttu-id="4917d-148">必填。</span><span class="sxs-lookup"><span data-stu-id="4917d-148">Required.</span></span> <span data-ttu-id="4917d-149">目标分区组的 id。</span><span class="sxs-lookup"><span data-stu-id="4917d-149">The id of the destination section group.</span></span> |
|<span data-ttu-id="4917d-150">renameAs</span><span class="sxs-lookup"><span data-stu-id="4917d-150">renameAs</span></span>|<span data-ttu-id="4917d-151">String</span><span class="sxs-lookup"><span data-stu-id="4917d-151">String</span></span>|<span data-ttu-id="4917d-152">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="4917d-152">The name of the copy.</span></span> <span data-ttu-id="4917d-153">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="4917d-153">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="4917d-154">响应</span><span class="sxs-lookup"><span data-stu-id="4917d-154">Response</span></span>

<span data-ttu-id="4917d-155">如果成功，此方法将返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="4917d-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="4917d-156">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="4917d-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4917d-157">示例</span><span class="sxs-lookup"><span data-stu-id="4917d-157">Example</span></span>
<span data-ttu-id="4917d-158">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4917d-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4917d-159">请求</span><span class="sxs-lookup"><span data-stu-id="4917d-159">Request</span></span>
<span data-ttu-id="4917d-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4917d-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4917d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="4917d-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4917d-162">C#</span><span class="sxs-lookup"><span data-stu-id="4917d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4917d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4917d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4917d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4917d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4917d-165">响应</span><span class="sxs-lookup"><span data-stu-id="4917d-165">Response</span></span>
<span data-ttu-id="4917d-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4917d-166">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
