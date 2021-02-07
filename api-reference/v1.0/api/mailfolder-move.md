---
title: 'mailFolder: move'
description: 将 Mailfolder 及其内容移动到其他 mailfolder。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ea5e38ab2196c5ba7dba8a1776bd989b0ba97086
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135327"
---
# <a name="mailfolder-move"></a><span data-ttu-id="e0547-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="e0547-103">mailFolder: move</span></span>

<span data-ttu-id="e0547-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0547-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0547-105">将 Mailfolder 及其内容移动到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="e0547-105">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0547-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e0547-106">Permissions</span></span>

<span data-ttu-id="e0547-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0547-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0547-109">Permission type</span></span> | <span data-ttu-id="e0547-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0547-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="e0547-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0547-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0547-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0547-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e0547-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0547-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0547-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0547-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e0547-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0547-115">Application</span></span> | <span data-ttu-id="e0547-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0547-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0547-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0547-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="e0547-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0547-118">Request headers</span></span>

| <span data-ttu-id="e0547-119">标头</span><span class="sxs-lookup"><span data-stu-id="e0547-119">Header</span></span> | <span data-ttu-id="e0547-120">值</span><span class="sxs-lookup"><span data-stu-id="e0547-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="e0547-121">授权</span><span class="sxs-lookup"><span data-stu-id="e0547-121">Authorization</span></span> | <span data-ttu-id="e0547-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="e0547-122">`Bearer {token}`.</span></span> <span data-ttu-id="e0547-123">必需。</span><span class="sxs-lookup"><span data-stu-id="e0547-123">Required.</span></span> |
| <span data-ttu-id="e0547-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0547-124">Content-Type</span></span> | <span data-ttu-id="e0547-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="e0547-125">`application/json`.</span></span> <span data-ttu-id="e0547-126">必需。</span><span class="sxs-lookup"><span data-stu-id="e0547-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0547-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0547-127">Request body</span></span>

<span data-ttu-id="e0547-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e0547-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0547-129">参数</span><span class="sxs-lookup"><span data-stu-id="e0547-129">Parameter</span></span> | <span data-ttu-id="e0547-130">类型</span><span class="sxs-lookup"><span data-stu-id="e0547-130">Type</span></span> | <span data-ttu-id="e0547-131">说明</span><span class="sxs-lookup"><span data-stu-id="e0547-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="e0547-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="e0547-132">destinationId</span></span>|<span data-ttu-id="e0547-133">String</span><span class="sxs-lookup"><span data-stu-id="e0547-133">String</span></span>|<span data-ttu-id="e0547-134">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="e0547-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="e0547-135">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="e0547-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="e0547-136">响应</span><span class="sxs-lookup"><span data-stu-id="e0547-136">Response</span></span>

<span data-ttu-id="e0547-137">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [mailFolder](../resources/mailfolder.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="e0547-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0547-138">示例</span><span class="sxs-lookup"><span data-stu-id="e0547-138">Example</span></span>

<span data-ttu-id="e0547-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e0547-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e0547-140">请求</span><span class="sxs-lookup"><span data-stu-id="e0547-140">Request</span></span>

<span data-ttu-id="e0547-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0547-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0547-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0547-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e0547-143">C#</span><span class="sxs-lookup"><span data-stu-id="e0547-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0547-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0547-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0547-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0547-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0547-146">Java</span><span class="sxs-lookup"><span data-stu-id="e0547-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e0547-147">响应</span><span class="sxs-lookup"><span data-stu-id="e0547-147">Response</span></span>

<span data-ttu-id="e0547-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0547-148">Here is an example of the response.</span></span>

> <span data-ttu-id="e0547-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0547-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

