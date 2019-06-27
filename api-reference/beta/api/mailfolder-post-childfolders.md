---
title: Create mailFolder
description: 使用此 API 创建新的子 mailFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f181f2716aa56dc9d27f0dbc2259157a0d04b28f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266644"
---
# <a name="create-mailfolder"></a><span data-ttu-id="c6069-103">Create mailFolder</span><span class="sxs-lookup"><span data-stu-id="c6069-103">Create mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6069-104">使用此 API 创建新的子[mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="c6069-104">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6069-105">权限</span><span class="sxs-lookup"><span data-stu-id="c6069-105">Permissions</span></span>

<span data-ttu-id="c6069-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6069-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6069-108">Permission type</span></span> | <span data-ttu-id="c6069-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6069-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c6069-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6069-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6069-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6069-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6069-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6069-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6069-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6069-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6069-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6069-114">Application</span></span> | <span data-ttu-id="c6069-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6069-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6069-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6069-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c6069-117">将查询 URL 中的父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="c6069-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c6069-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="c6069-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6069-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6069-119">Request headers</span></span>

| <span data-ttu-id="c6069-120">标头</span><span class="sxs-lookup"><span data-stu-id="c6069-120">Header</span></span> | <span data-ttu-id="c6069-121">值</span><span class="sxs-lookup"><span data-stu-id="c6069-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c6069-122">授权</span><span class="sxs-lookup"><span data-stu-id="c6069-122">Authorization</span></span> | <span data-ttu-id="c6069-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c6069-123"></span></span> <span data-ttu-id="c6069-124">必需。</span><span class="sxs-lookup"><span data-stu-id="c6069-124">Required.</span></span> |
| <span data-ttu-id="c6069-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6069-125">Content-Type</span></span> | <span data-ttu-id="c6069-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c6069-126"></span></span> <span data-ttu-id="c6069-127">必需。</span><span class="sxs-lookup"><span data-stu-id="c6069-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6069-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6069-128">Request body</span></span>

<span data-ttu-id="c6069-p105">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="c6069-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="c6069-131">参数</span><span class="sxs-lookup"><span data-stu-id="c6069-131">Parameter</span></span> | <span data-ttu-id="c6069-132">类型</span><span class="sxs-lookup"><span data-stu-id="c6069-132">Type</span></span> | <span data-ttu-id="c6069-133">说明</span><span class="sxs-lookup"><span data-stu-id="c6069-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="c6069-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c6069-134">displayName</span></span>|<span data-ttu-id="c6069-135">String</span><span class="sxs-lookup"><span data-stu-id="c6069-135">String</span></span>|<span data-ttu-id="c6069-136">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c6069-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="c6069-137">响应</span><span class="sxs-lookup"><span data-stu-id="c6069-137">Response</span></span>

<span data-ttu-id="c6069-138">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6069-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6069-139">示例</span><span class="sxs-lookup"><span data-stu-id="c6069-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6069-140">请求</span><span class="sxs-lookup"><span data-stu-id="c6069-140">Request</span></span>

<span data-ttu-id="c6069-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6069-141">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="c6069-142">响应</span><span class="sxs-lookup"><span data-stu-id="c6069-142">Response</span></span>

<span data-ttu-id="c6069-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c6069-143">The following is an example of the response.</span></span>

> <span data-ttu-id="c6069-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c6069-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c6069-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c6069-145">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6069-146">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c6069-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6069-147">C#</span><span class="sxs-lookup"><span data-stu-id="c6069-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6069-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6069-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6069-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="c6069-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_mailfolder_from_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
