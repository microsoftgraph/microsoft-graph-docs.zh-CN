---
title: Create mailFolder
description: 使用此 API 创建新的子 mailFolder。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d79b9817332c7aea773ad9062efd3a4718dd197
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049252"
---
# <a name="create-mailfolder"></a><span data-ttu-id="f6331-103">Create mailFolder</span><span class="sxs-lookup"><span data-stu-id="f6331-103">Create mailFolder</span></span>

<span data-ttu-id="f6331-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6331-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6331-105">使用此 API 创建新的子 [mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="f6331-105">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6331-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6331-106">Permissions</span></span>

<span data-ttu-id="f6331-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6331-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6331-109">Permission type</span></span> | <span data-ttu-id="f6331-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6331-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f6331-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6331-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6331-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6331-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6331-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6331-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6331-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6331-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6331-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6331-115">Application</span></span> | <span data-ttu-id="f6331-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6331-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6331-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6331-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="f6331-118">在查询 URL 中将父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="f6331-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f6331-119">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="f6331-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6331-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6331-120">Request headers</span></span>

| <span data-ttu-id="f6331-121">标头</span><span class="sxs-lookup"><span data-stu-id="f6331-121">Header</span></span> | <span data-ttu-id="f6331-122">值</span><span class="sxs-lookup"><span data-stu-id="f6331-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f6331-123">授权</span><span class="sxs-lookup"><span data-stu-id="f6331-123">Authorization</span></span> | <span data-ttu-id="f6331-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f6331-124">`Bearer {token}`.</span></span> <span data-ttu-id="f6331-125">必需。</span><span class="sxs-lookup"><span data-stu-id="f6331-125">Required.</span></span> |
| <span data-ttu-id="f6331-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6331-126">Content-Type</span></span> | <span data-ttu-id="f6331-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f6331-127">`application/json`.</span></span> <span data-ttu-id="f6331-128">必需。</span><span class="sxs-lookup"><span data-stu-id="f6331-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6331-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6331-129">Request body</span></span>

<span data-ttu-id="f6331-p105">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="f6331-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="f6331-132">参数</span><span class="sxs-lookup"><span data-stu-id="f6331-132">Parameter</span></span> | <span data-ttu-id="f6331-133">类型</span><span class="sxs-lookup"><span data-stu-id="f6331-133">Type</span></span> | <span data-ttu-id="f6331-134">说明</span><span class="sxs-lookup"><span data-stu-id="f6331-134">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="f6331-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f6331-135">displayName</span></span>|<span data-ttu-id="f6331-136">String</span><span class="sxs-lookup"><span data-stu-id="f6331-136">String</span></span>|<span data-ttu-id="f6331-137">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f6331-137">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="f6331-138">响应</span><span class="sxs-lookup"><span data-stu-id="f6331-138">Response</span></span>

<span data-ttu-id="f6331-139">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [mailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6331-139">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6331-140">示例</span><span class="sxs-lookup"><span data-stu-id="f6331-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f6331-141">请求</span><span class="sxs-lookup"><span data-stu-id="f6331-141">Request</span></span>

<span data-ttu-id="f6331-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6331-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6331-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6331-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="f6331-144">C#</span><span class="sxs-lookup"><span data-stu-id="f6331-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6331-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6331-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6331-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6331-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6331-147">Java</span><span class="sxs-lookup"><span data-stu-id="f6331-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6331-148">响应</span><span class="sxs-lookup"><span data-stu-id="f6331-148">Response</span></span>

<span data-ttu-id="f6331-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f6331-149">The following is an example of the response.</span></span>

> <span data-ttu-id="f6331-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f6331-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


