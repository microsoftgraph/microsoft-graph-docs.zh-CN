---
title: 'mailFolder: copy'
description: 将 mailfolder 及其内容复制到其他 mailfolder。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8414eaf1c572b61c320e8c5db6f77656ca99c497
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049294"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="a053b-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="a053b-103">mailFolder: copy</span></span>

<span data-ttu-id="a053b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a053b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a053b-105">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="a053b-105">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a053b-106">权限</span><span class="sxs-lookup"><span data-stu-id="a053b-106">Permissions</span></span>

<span data-ttu-id="a053b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a053b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a053b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a053b-109">Permission type</span></span> | <span data-ttu-id="a053b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a053b-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="a053b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a053b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a053b-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a053b-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a053b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a053b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a053b-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a053b-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a053b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a053b-115">Application</span></span> | <span data-ttu-id="a053b-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a053b-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a053b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a053b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="a053b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a053b-118">Request headers</span></span>

| <span data-ttu-id="a053b-119">标头</span><span class="sxs-lookup"><span data-stu-id="a053b-119">Header</span></span> | <span data-ttu-id="a053b-120">值</span><span class="sxs-lookup"><span data-stu-id="a053b-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="a053b-121">授权</span><span class="sxs-lookup"><span data-stu-id="a053b-121">Authorization</span></span> | <span data-ttu-id="a053b-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="a053b-122">`Bearer {token}`.</span></span> <span data-ttu-id="a053b-123">必需。</span><span class="sxs-lookup"><span data-stu-id="a053b-123">Required.</span></span> |
| <span data-ttu-id="a053b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a053b-124">Content-Type</span></span> | <span data-ttu-id="a053b-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="a053b-125">`application/json`.</span></span> <span data-ttu-id="a053b-126">必需。</span><span class="sxs-lookup"><span data-stu-id="a053b-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a053b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a053b-127">Request body</span></span>

<span data-ttu-id="a053b-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a053b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a053b-129">参数</span><span class="sxs-lookup"><span data-stu-id="a053b-129">Parameter</span></span> | <span data-ttu-id="a053b-130">类型</span><span class="sxs-lookup"><span data-stu-id="a053b-130">Type</span></span> | <span data-ttu-id="a053b-131">说明</span><span class="sxs-lookup"><span data-stu-id="a053b-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="a053b-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="a053b-132">destinationId</span></span>|<span data-ttu-id="a053b-133">String</span><span class="sxs-lookup"><span data-stu-id="a053b-133">String</span></span>|<span data-ttu-id="a053b-134">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="a053b-134">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="a053b-135">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="a053b-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a053b-136">响应</span><span class="sxs-lookup"><span data-stu-id="a053b-136">Response</span></span>

<span data-ttu-id="a053b-137">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [mailFolder](../resources/mailfolder.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="a053b-137">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a053b-138">示例</span><span class="sxs-lookup"><span data-stu-id="a053b-138">Example</span></span>

<span data-ttu-id="a053b-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a053b-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a053b-140">请求</span><span class="sxs-lookup"><span data-stu-id="a053b-140">Request</span></span>

<span data-ttu-id="a053b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a053b-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a053b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a053b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="a053b-143">C#</span><span class="sxs-lookup"><span data-stu-id="a053b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a053b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a053b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a053b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a053b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a053b-146">Java</span><span class="sxs-lookup"><span data-stu-id="a053b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a053b-147">响应</span><span class="sxs-lookup"><span data-stu-id="a053b-147">Response</span></span>

<span data-ttu-id="a053b-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a053b-148">Here is an example of the response.</span></span>

> <span data-ttu-id="a053b-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a053b-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


