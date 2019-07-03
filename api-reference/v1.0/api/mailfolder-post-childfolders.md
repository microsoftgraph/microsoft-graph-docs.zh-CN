---
title: 创建 MailFolder
description: 使用此 API 新建子 MailFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5e5c2c9b0aa1355475fcb810bbc27b10593b0c25
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454354"
---
# <a name="create-mailfolder"></a><span data-ttu-id="dcaa8-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="dcaa8-103">Create MailFolder</span></span>

<span data-ttu-id="dcaa8-104">使用此 API 新建子 MailFolder。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcaa8-105">权限</span><span class="sxs-lookup"><span data-stu-id="dcaa8-105">Permissions</span></span>

<span data-ttu-id="dcaa8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcaa8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcaa8-108">Permission type</span></span> | <span data-ttu-id="dcaa8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcaa8-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="dcaa8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcaa8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcaa8-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcaa8-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dcaa8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcaa8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcaa8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcaa8-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dcaa8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcaa8-114">Application</span></span> | <span data-ttu-id="dcaa8-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcaa8-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcaa8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcaa8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="dcaa8-117">将查询 URL 中的父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="dcaa8-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcaa8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcaa8-119">Request headers</span></span>

| <span data-ttu-id="dcaa8-120">标头</span><span class="sxs-lookup"><span data-stu-id="dcaa8-120">Header</span></span> | <span data-ttu-id="dcaa8-121">值</span><span class="sxs-lookup"><span data-stu-id="dcaa8-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="dcaa8-122">授权</span><span class="sxs-lookup"><span data-stu-id="dcaa8-122">Authorization</span></span> | <span data-ttu-id="dcaa8-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="dcaa8-123"></span></span> <span data-ttu-id="dcaa8-124">必需。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-124">Required.</span></span> |
| <span data-ttu-id="dcaa8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dcaa8-125">Content-Type</span></span> | <span data-ttu-id="dcaa8-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="dcaa8-126"></span></span> <span data-ttu-id="dcaa8-127">必需。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcaa8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcaa8-128">Request body</span></span>

<span data-ttu-id="dcaa8-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="dcaa8-130">**displayName**是[mailFolder](../resources/mailfolder.md)对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="dcaa8-131">参数</span><span class="sxs-lookup"><span data-stu-id="dcaa8-131">Parameter</span></span> | <span data-ttu-id="dcaa8-132">类型</span><span class="sxs-lookup"><span data-stu-id="dcaa8-132">Type</span></span> | <span data-ttu-id="dcaa8-133">说明</span><span class="sxs-lookup"><span data-stu-id="dcaa8-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="dcaa8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="dcaa8-134">displayName</span></span>|<span data-ttu-id="dcaa8-135">String</span><span class="sxs-lookup"><span data-stu-id="dcaa8-135">String</span></span>|<span data-ttu-id="dcaa8-136">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="dcaa8-137">响应</span><span class="sxs-lookup"><span data-stu-id="dcaa8-137">Response</span></span>

<span data-ttu-id="dcaa8-138">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[mailFolder](../resources/mailfolder.md)资源。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcaa8-139">示例</span><span class="sxs-lookup"><span data-stu-id="dcaa8-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dcaa8-140">请求</span><span class="sxs-lookup"><span data-stu-id="dcaa8-140">Request</span></span>

<span data-ttu-id="dcaa8-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dcaa8-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dcaa8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcaa8-143">C#</span><span class="sxs-lookup"><span data-stu-id="dcaa8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcaa8-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="dcaa8-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcaa8-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="dcaa8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dcaa8-146">响应</span><span class="sxs-lookup"><span data-stu-id="dcaa8-146">Response</span></span>
<span data-ttu-id="dcaa8-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-147">Here is an example of the response.</span></span>

> <span data-ttu-id="dcaa8-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dcaa8-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dcaa8-149">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
