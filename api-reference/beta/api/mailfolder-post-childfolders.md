---
title: Create mailFolder
description: 使用此 API 创建新的子 mailFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6534b49212f68b5bdb871e9298e5583f0a3afa79
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415237"
---
# <a name="create-mailfolder"></a><span data-ttu-id="0d89a-103">Create mailFolder</span><span class="sxs-lookup"><span data-stu-id="0d89a-103">Create mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d89a-104">使用此 API 创建新的子[mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="0d89a-104">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d89a-105">权限</span><span class="sxs-lookup"><span data-stu-id="0d89a-105">Permissions</span></span>

<span data-ttu-id="0d89a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d89a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d89a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d89a-108">Permission type</span></span> | <span data-ttu-id="0d89a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d89a-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="0d89a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d89a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d89a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d89a-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0d89a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d89a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d89a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d89a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0d89a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d89a-114">Application</span></span> | <span data-ttu-id="0d89a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d89a-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d89a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d89a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="0d89a-117">将查询 URL 中的父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="0d89a-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="0d89a-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="0d89a-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d89a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d89a-119">Request headers</span></span>

| <span data-ttu-id="0d89a-120">标头</span><span class="sxs-lookup"><span data-stu-id="0d89a-120">Header</span></span> | <span data-ttu-id="0d89a-121">值</span><span class="sxs-lookup"><span data-stu-id="0d89a-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="0d89a-122">授权</span><span class="sxs-lookup"><span data-stu-id="0d89a-122">Authorization</span></span> | <span data-ttu-id="0d89a-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="0d89a-123"></span></span> <span data-ttu-id="0d89a-124">必需。</span><span class="sxs-lookup"><span data-stu-id="0d89a-124">Required.</span></span> |
| <span data-ttu-id="0d89a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d89a-125">Content-Type</span></span> | <span data-ttu-id="0d89a-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="0d89a-126"></span></span> <span data-ttu-id="0d89a-127">必需。</span><span class="sxs-lookup"><span data-stu-id="0d89a-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d89a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d89a-128">Request body</span></span>

<span data-ttu-id="0d89a-p105">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="0d89a-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="0d89a-131">参数</span><span class="sxs-lookup"><span data-stu-id="0d89a-131">Parameter</span></span> | <span data-ttu-id="0d89a-132">类型</span><span class="sxs-lookup"><span data-stu-id="0d89a-132">Type</span></span> | <span data-ttu-id="0d89a-133">说明</span><span class="sxs-lookup"><span data-stu-id="0d89a-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="0d89a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0d89a-134">displayName</span></span>|<span data-ttu-id="0d89a-135">String</span><span class="sxs-lookup"><span data-stu-id="0d89a-135">String</span></span>|<span data-ttu-id="0d89a-136">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0d89a-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="0d89a-137">响应</span><span class="sxs-lookup"><span data-stu-id="0d89a-137">Response</span></span>

<span data-ttu-id="0d89a-138">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0d89a-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d89a-139">示例</span><span class="sxs-lookup"><span data-stu-id="0d89a-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0d89a-140">请求</span><span class="sxs-lookup"><span data-stu-id="0d89a-140">Request</span></span>

<span data-ttu-id="0d89a-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d89a-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0d89a-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0d89a-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0d89a-143">C#</span><span class="sxs-lookup"><span data-stu-id="0d89a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d89a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d89a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0d89a-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="0d89a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d89a-146">响应</span><span class="sxs-lookup"><span data-stu-id="0d89a-146">Response</span></span>

<span data-ttu-id="0d89a-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0d89a-147">The following is an example of the response.</span></span>

> <span data-ttu-id="0d89a-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0d89a-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0d89a-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d89a-149">All the properties will be returned from an actual call.</span></span>
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
