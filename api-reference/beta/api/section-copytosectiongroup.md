---
title: '部分: copyToSectionGroup'
description: 将分区复制到特定分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: c96f332611cdc9d1f3e19772f33c09ee5648dc18
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457441"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="d070f-103">部分: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="d070f-103">section: copyToSectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d070f-104">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="d070f-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="d070f-105">对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="d070f-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="d070f-106">权限</span><span class="sxs-lookup"><span data-stu-id="d070f-106">Permissions</span></span>
<span data-ttu-id="d070f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d070f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d070f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d070f-109">Permission type</span></span>      | <span data-ttu-id="d070f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d070f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d070f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d070f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d070f-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d070f-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d070f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d070f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d070f-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d070f-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d070f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d070f-115">Application</span></span> | <span data-ttu-id="d070f-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d070f-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d070f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d070f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="d070f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d070f-118">Request headers</span></span>
| <span data-ttu-id="d070f-119">名称</span><span class="sxs-lookup"><span data-stu-id="d070f-119">Name</span></span>       | <span data-ttu-id="d070f-120">类型</span><span class="sxs-lookup"><span data-stu-id="d070f-120">Type</span></span> | <span data-ttu-id="d070f-121">说明</span><span class="sxs-lookup"><span data-stu-id="d070f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d070f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d070f-122">Authorization</span></span>  | <span data-ttu-id="d070f-123">string</span><span class="sxs-lookup"><span data-stu-id="d070f-123">string</span></span>  | <span data-ttu-id="d070f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d070f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d070f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d070f-126">Content-Type</span></span> | <span data-ttu-id="d070f-127">string</span><span class="sxs-lookup"><span data-stu-id="d070f-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d070f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d070f-128">Request body</span></span>
<span data-ttu-id="d070f-129">在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="d070f-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="d070f-130">参数</span><span class="sxs-lookup"><span data-stu-id="d070f-130">Parameter</span></span>    | <span data-ttu-id="d070f-131">类型</span><span class="sxs-lookup"><span data-stu-id="d070f-131">Type</span></span>   |<span data-ttu-id="d070f-132">说明</span><span class="sxs-lookup"><span data-stu-id="d070f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d070f-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="d070f-133">siteCollectionId</span></span>|<span data-ttu-id="d070f-134">String</span><span class="sxs-lookup"><span data-stu-id="d070f-134">String</span></span>|<span data-ttu-id="d070f-135">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="d070f-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="d070f-136">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="d070f-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="d070f-137">siteId</span><span class="sxs-lookup"><span data-stu-id="d070f-137">siteId</span></span>|<span data-ttu-id="d070f-138">String</span><span class="sxs-lookup"><span data-stu-id="d070f-138">String</span></span>|<span data-ttu-id="d070f-139">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="d070f-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="d070f-140">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="d070f-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="d070f-141">groupId</span><span class="sxs-lookup"><span data-stu-id="d070f-141">groupId</span></span>|<span data-ttu-id="d070f-142">String</span><span class="sxs-lookup"><span data-stu-id="d070f-142">String</span></span>|<span data-ttu-id="d070f-143">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="d070f-143">The id of the group to copy to.</span></span> <span data-ttu-id="d070f-144">仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="d070f-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="d070f-145">id</span><span class="sxs-lookup"><span data-stu-id="d070f-145">id</span></span>|<span data-ttu-id="d070f-146">String</span><span class="sxs-lookup"><span data-stu-id="d070f-146">String</span></span>|<span data-ttu-id="d070f-147">必需。</span><span class="sxs-lookup"><span data-stu-id="d070f-147">Required.</span></span> <span data-ttu-id="d070f-148">目标分区组的 id。</span><span class="sxs-lookup"><span data-stu-id="d070f-148">The id of the destination section group.</span></span> |
|<span data-ttu-id="d070f-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="d070f-149">renameAs</span></span>|<span data-ttu-id="d070f-150">String</span><span class="sxs-lookup"><span data-stu-id="d070f-150">String</span></span>|<span data-ttu-id="d070f-151">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="d070f-151">The name of the copy.</span></span> <span data-ttu-id="d070f-152">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="d070f-152">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="d070f-153">响应</span><span class="sxs-lookup"><span data-stu-id="d070f-153">Response</span></span>

<span data-ttu-id="d070f-154">如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。</span><span class="sxs-lookup"><span data-stu-id="d070f-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="d070f-155">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="d070f-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="d070f-156">示例</span><span class="sxs-lookup"><span data-stu-id="d070f-156">Example</span></span>
<span data-ttu-id="d070f-157">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d070f-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d070f-158">请求</span><span class="sxs-lookup"><span data-stu-id="d070f-158">Request</span></span>
<span data-ttu-id="d070f-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d070f-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d070f-160">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d070f-160">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d070f-161">C#</span><span class="sxs-lookup"><span data-stu-id="d070f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d070f-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="d070f-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d070f-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="d070f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d070f-164">响应</span><span class="sxs-lookup"><span data-stu-id="d070f-164">Response</span></span>
<span data-ttu-id="d070f-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d070f-165">Here is an example of the response.</span></span>
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
