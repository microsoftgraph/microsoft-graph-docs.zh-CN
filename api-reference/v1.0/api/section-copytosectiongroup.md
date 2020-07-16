---
title: 部分： copyToSectionGroup
description: 将分区复制到特定分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 68a15f81fc61868d2f1b835c3a593a39be2546e3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897496"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="b44e0-103">部分： copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b44e0-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="b44e0-104">命名空间： microsoft. graph 将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="b44e0-104">Namespace: microsoft.graph Copies a section to a specific section group.</span></span>

<span data-ttu-id="b44e0-105">对于复制操作，请遵循异步调用模式：首先调用复制操作，然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="b44e0-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b44e0-106">权限</span><span class="sxs-lookup"><span data-stu-id="b44e0-106">Permissions</span></span>
<span data-ttu-id="b44e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b44e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b44e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b44e0-109">Permission type</span></span>      | <span data-ttu-id="b44e0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b44e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b44e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b44e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b44e0-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44e0-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b44e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b44e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b44e0-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b44e0-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b44e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b44e0-115">Application</span></span> | <span data-ttu-id="b44e0-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44e0-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b44e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b44e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="b44e0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b44e0-118">Request headers</span></span>
| <span data-ttu-id="b44e0-119">名称</span><span class="sxs-lookup"><span data-stu-id="b44e0-119">Name</span></span>       | <span data-ttu-id="b44e0-120">类型</span><span class="sxs-lookup"><span data-stu-id="b44e0-120">Type</span></span> | <span data-ttu-id="b44e0-121">说明</span><span class="sxs-lookup"><span data-stu-id="b44e0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b44e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b44e0-122">Authorization</span></span>  | <span data-ttu-id="b44e0-123">string</span><span class="sxs-lookup"><span data-stu-id="b44e0-123">string</span></span>  | <span data-ttu-id="b44e0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b44e0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b44e0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b44e0-126">Content-Type</span></span> | <span data-ttu-id="b44e0-127">string</span><span class="sxs-lookup"><span data-stu-id="b44e0-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b44e0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b44e0-128">Request body</span></span>
<span data-ttu-id="b44e0-129">在请求正文中，提供一个 JSON 对象，其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="b44e0-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="b44e0-130">参数</span><span class="sxs-lookup"><span data-stu-id="b44e0-130">Parameter</span></span>    | <span data-ttu-id="b44e0-131">类型</span><span class="sxs-lookup"><span data-stu-id="b44e0-131">Type</span></span>   |<span data-ttu-id="b44e0-132">说明</span><span class="sxs-lookup"><span data-stu-id="b44e0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b44e0-133">groupId</span><span class="sxs-lookup"><span data-stu-id="b44e0-133">groupId</span></span>|<span data-ttu-id="b44e0-134">String</span><span class="sxs-lookup"><span data-stu-id="b44e0-134">String</span></span>|<span data-ttu-id="b44e0-135">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="b44e0-135">The id of the group to copy to.</span></span> <span data-ttu-id="b44e0-136">仅在复制到 Microsoft 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="b44e0-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="b44e0-137">id</span><span class="sxs-lookup"><span data-stu-id="b44e0-137">id</span></span>|<span data-ttu-id="b44e0-138">String</span><span class="sxs-lookup"><span data-stu-id="b44e0-138">String</span></span>|<span data-ttu-id="b44e0-139">必填。</span><span class="sxs-lookup"><span data-stu-id="b44e0-139">Required.</span></span> <span data-ttu-id="b44e0-140">目标分区组的 id。</span><span class="sxs-lookup"><span data-stu-id="b44e0-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="b44e0-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="b44e0-141">renameAs</span></span>|<span data-ttu-id="b44e0-142">String</span><span class="sxs-lookup"><span data-stu-id="b44e0-142">String</span></span>|<span data-ttu-id="b44e0-143">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="b44e0-143">The name of the copy.</span></span> <span data-ttu-id="b44e0-144">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="b44e0-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="b44e0-145">响应</span><span class="sxs-lookup"><span data-stu-id="b44e0-145">Response</span></span>

<span data-ttu-id="b44e0-146">如果成功，此方法将返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。</span><span class="sxs-lookup"><span data-stu-id="b44e0-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="b44e0-147">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="b44e0-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b44e0-148">示例</span><span class="sxs-lookup"><span data-stu-id="b44e0-148">Example</span></span>
<span data-ttu-id="b44e0-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b44e0-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b44e0-150">请求</span><span class="sxs-lookup"><span data-stu-id="b44e0-150">Request</span></span>
<span data-ttu-id="b44e0-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b44e0-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b44e0-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="b44e0-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b44e0-153">C#</span><span class="sxs-lookup"><span data-stu-id="b44e0-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b44e0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b44e0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b44e0-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b44e0-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b44e0-156">Java</span><span class="sxs-lookup"><span data-stu-id="b44e0-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b44e0-157">响应</span><span class="sxs-lookup"><span data-stu-id="b44e0-157">Response</span></span>
<span data-ttu-id="b44e0-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b44e0-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
