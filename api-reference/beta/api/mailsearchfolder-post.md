---
title: 创建 mailSearchFolder
description: 使用此 API 在指定用户的邮箱中创建新的 mailSearchFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 05959fe291116b1e16d0108c257ab73f38805d95
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812906"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="4f058-103">创建 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="4f058-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f058-104">在指定用户的邮箱中创建新的[mailSearchFolder](../resources/mailsearchfolder.md) 。</span><span class="sxs-lookup"><span data-stu-id="4f058-104">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f058-105">权限</span><span class="sxs-lookup"><span data-stu-id="4f058-105">Permissions</span></span>

<span data-ttu-id="4f058-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f058-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f058-108">Permission type</span></span> | <span data-ttu-id="4f058-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f058-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="4f058-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f058-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f058-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f058-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4f058-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f058-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f058-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f058-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4f058-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f058-114">Application</span></span> | <span data-ttu-id="4f058-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f058-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f058-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f058-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="4f058-117">将查询 URL 中的父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="4f058-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="4f058-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="4f058-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f058-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f058-119">Request headers</span></span>

| <span data-ttu-id="4f058-120">标头</span><span class="sxs-lookup"><span data-stu-id="4f058-120">Header</span></span> | <span data-ttu-id="4f058-121">值</span><span class="sxs-lookup"><span data-stu-id="4f058-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="4f058-122">授权</span><span class="sxs-lookup"><span data-stu-id="4f058-122">Authorization</span></span> | <span data-ttu-id="4f058-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="4f058-123"></span></span> <span data-ttu-id="4f058-124">必需。</span><span class="sxs-lookup"><span data-stu-id="4f058-124">Required.</span></span> |
| <span data-ttu-id="4f058-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f058-125">Content-Type</span></span> | <span data-ttu-id="4f058-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="4f058-126"></span></span> <span data-ttu-id="4f058-127">必需。</span><span class="sxs-lookup"><span data-stu-id="4f058-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f058-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f058-128">Request body</span></span>

<span data-ttu-id="4f058-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4f058-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f058-130">参数</span><span class="sxs-lookup"><span data-stu-id="4f058-130">Parameter</span></span> | <span data-ttu-id="4f058-131">类型</span><span class="sxs-lookup"><span data-stu-id="4f058-131">Type</span></span> | <span data-ttu-id="4f058-132">说明</span><span class="sxs-lookup"><span data-stu-id="4f058-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="4f058-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="4f058-133">@odata.type</span></span> | <span data-ttu-id="4f058-134">String</span><span class="sxs-lookup"><span data-stu-id="4f058-134">String</span></span> | <span data-ttu-id="4f058-135">要创建的文件夹的类型。</span><span class="sxs-lookup"><span data-stu-id="4f058-135">The type of folder to be created.</span></span> <span data-ttu-id="4f058-136">设置为 "mailSearchFolder"。</span><span class="sxs-lookup"><span data-stu-id="4f058-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="4f058-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4f058-137">displayName</span></span> | <span data-ttu-id="4f058-138">String</span><span class="sxs-lookup"><span data-stu-id="4f058-138">String</span></span> | <span data-ttu-id="4f058-139">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f058-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="4f058-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="4f058-140">includeNestedFolders</span></span> | <span data-ttu-id="4f058-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f058-141">Boolean</span></span> | <span data-ttu-id="4f058-142">指示应如何在搜索中遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="4f058-142">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="4f058-143">`true`表示应执行深入搜索以在**sourceFolderIds**中显式指定的每个文件夹的层次结构中包含子文件夹。</span><span class="sxs-lookup"><span data-stu-id="4f058-143">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="4f058-144">`false`表示仅对**sourceFolderIds**中显式指定的每个文件夹进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="4f058-144">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="4f058-145">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="4f058-145">sourceFolderIds</span></span> | <span data-ttu-id="4f058-146">String collection</span><span class="sxs-lookup"><span data-stu-id="4f058-146">String collection</span></span> | <span data-ttu-id="4f058-147">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="4f058-147">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="4f058-148">filterQuery</span><span class="sxs-lookup"><span data-stu-id="4f058-148">filterQuery</span></span> | <span data-ttu-id="4f058-149">String</span><span class="sxs-lookup"><span data-stu-id="4f058-149">String</span></span> | <span data-ttu-id="4f058-150">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="4f058-150">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="4f058-151">响应</span><span class="sxs-lookup"><span data-stu-id="4f058-151">Response</span></span>

<span data-ttu-id="4f058-152">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[mailSearchFolder](../resources/mailsearchfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4f058-152">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f058-153">示例</span><span class="sxs-lookup"><span data-stu-id="4f058-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4f058-154">请求</span><span class="sxs-lookup"><span data-stu-id="4f058-154">Request</span></span>

<span data-ttu-id="4f058-155">以下是请求的示例-它将创建包含主题中的字符串 "每周摘要" 的邮件的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="4f058-155">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="4f058-156">搜索文件夹在应用指定的筛选器查询的同一文件夹下。</span><span class="sxs-lookup"><span data-stu-id="4f058-156">The search folder is under the same folder on which the specified filter query applies.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADYAAAIBDAAAAA=="],
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Weekly digests",
  "includeNestedFolders": true,
  "sourceFolderIds": ["AQMkADYAAAIBDAAAAA=="],
  "filterQuery": "contains(subject, 'weekly digest')"
}
```

#### <a name="response"></a><span data-ttu-id="4f058-157">响应</span><span class="sxs-lookup"><span data-stu-id="4f058-157">Response</span></span>

<span data-ttu-id="4f058-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4f058-158">The following is an example of the response.</span></span>

><span data-ttu-id="4f058-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4f058-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f058-160">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f058-160">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders('AQMkADYAAAIBDAAAAA%3D%3D')/childFolders/$entity",
    "@odata.type": "#microsoft.graph.mailSearchFolder",
    "id": "AAMkADYfRAAAZg1yTAAA=",
    "displayName": "Weekly digests",
    "parentFolderId": "AQMkADYAAAIBDAAAAA==",
    "childFolderCount": 0,
    "unreadItemCount": 0,
    "totalItemCount": 0,
    "wellKnownName": null,
    "isSupported": true,
    "includeNestedFolders": true,
    "sourceFolderIds": [
        "AQMkADYAAAIBDAAAAA=="
    ],
    "filterQuery": "contains(subject, 'weekly digest')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4f058-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4f058-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4f058-162">C#</span><span class="sxs-lookup"><span data-stu-id="4f058-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_mailsearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f058-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f058-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_mailsearchfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
