---
title: 创建 mailSearchFolder
description: 使用此 API 在指定用户的邮箱中创建新的 mailSearchFolder。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ffa9f15cfabc5811a42bb17aea818b101e0a9f71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027706"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="713fd-103">创建 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="713fd-103">Create mailSearchFolder</span></span>

<span data-ttu-id="713fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="713fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="713fd-105">在指定用户的邮箱中创建新的 [mailSearchFolder](../resources/mailsearchfolder.md) 。</span><span class="sxs-lookup"><span data-stu-id="713fd-105">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="713fd-106">权限</span><span class="sxs-lookup"><span data-stu-id="713fd-106">Permissions</span></span>

<span data-ttu-id="713fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="713fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="713fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="713fd-109">Permission type</span></span> | <span data-ttu-id="713fd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="713fd-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="713fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="713fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="713fd-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="713fd-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="713fd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="713fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="713fd-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="713fd-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="713fd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="713fd-115">Application</span></span> | <span data-ttu-id="713fd-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="713fd-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="713fd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="713fd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="713fd-118">将查询 URL 中的父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="713fd-118">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="713fd-119">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="713fd-119">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="713fd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="713fd-120">Request headers</span></span>

| <span data-ttu-id="713fd-121">标头</span><span class="sxs-lookup"><span data-stu-id="713fd-121">Header</span></span> | <span data-ttu-id="713fd-122">值</span><span class="sxs-lookup"><span data-stu-id="713fd-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="713fd-123">授权</span><span class="sxs-lookup"><span data-stu-id="713fd-123">Authorization</span></span> | <span data-ttu-id="713fd-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="713fd-124">`Bearer {token}`.</span></span> <span data-ttu-id="713fd-125">必需。</span><span class="sxs-lookup"><span data-stu-id="713fd-125">Required.</span></span> |
| <span data-ttu-id="713fd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="713fd-126">Content-Type</span></span> | <span data-ttu-id="713fd-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="713fd-127">`application/json`.</span></span> <span data-ttu-id="713fd-128">必需。</span><span class="sxs-lookup"><span data-stu-id="713fd-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="713fd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="713fd-129">Request body</span></span>

<span data-ttu-id="713fd-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="713fd-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="713fd-131">参数</span><span class="sxs-lookup"><span data-stu-id="713fd-131">Parameter</span></span> | <span data-ttu-id="713fd-132">类型</span><span class="sxs-lookup"><span data-stu-id="713fd-132">Type</span></span> | <span data-ttu-id="713fd-133">说明</span><span class="sxs-lookup"><span data-stu-id="713fd-133">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="713fd-134">@odata.type</span><span class="sxs-lookup"><span data-stu-id="713fd-134">@odata.type</span></span> | <span data-ttu-id="713fd-135">String</span><span class="sxs-lookup"><span data-stu-id="713fd-135">String</span></span> | <span data-ttu-id="713fd-136">要创建的文件夹的类型。</span><span class="sxs-lookup"><span data-stu-id="713fd-136">The type of folder to be created.</span></span> <span data-ttu-id="713fd-137">设置为 "mailSearchFolder"。</span><span class="sxs-lookup"><span data-stu-id="713fd-137">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="713fd-138">displayName</span><span class="sxs-lookup"><span data-stu-id="713fd-138">displayName</span></span> | <span data-ttu-id="713fd-139">String</span><span class="sxs-lookup"><span data-stu-id="713fd-139">String</span></span> | <span data-ttu-id="713fd-140">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="713fd-140">The display name of the new folder.</span></span>|
| <span data-ttu-id="713fd-141">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="713fd-141">includeNestedFolders</span></span> | <span data-ttu-id="713fd-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="713fd-142">Boolean</span></span> | <span data-ttu-id="713fd-143">指示应如何在搜索中遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="713fd-143">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="713fd-144">`true` 表示应执行深入搜索以在 **sourceFolderIds**中显式指定的每个文件夹的层次结构中包含子文件夹。</span><span class="sxs-lookup"><span data-stu-id="713fd-144">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="713fd-145">`false` 表示仅对 **sourceFolderIds**中显式指定的每个文件夹进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="713fd-145">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="713fd-146">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="713fd-146">sourceFolderIds</span></span> | <span data-ttu-id="713fd-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="713fd-147">String collection</span></span> | <span data-ttu-id="713fd-148">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="713fd-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="713fd-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="713fd-149">filterQuery</span></span> | <span data-ttu-id="713fd-150">String</span><span class="sxs-lookup"><span data-stu-id="713fd-150">String</span></span> | <span data-ttu-id="713fd-151">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="713fd-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="713fd-152">响应</span><span class="sxs-lookup"><span data-stu-id="713fd-152">Response</span></span>

<span data-ttu-id="713fd-153">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [mailSearchFolder](../resources/mailsearchfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="713fd-153">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="713fd-154">示例</span><span class="sxs-lookup"><span data-stu-id="713fd-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="713fd-155">请求</span><span class="sxs-lookup"><span data-stu-id="713fd-155">Request</span></span>

<span data-ttu-id="713fd-156">以下是请求的示例-它将创建包含主题中的字符串 "每周摘要" 的邮件的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="713fd-156">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="713fd-157">搜索文件夹在应用指定的筛选器查询的同一文件夹下。</span><span class="sxs-lookup"><span data-stu-id="713fd-157">The search folder is under the same folder on which the specified filter query applies.</span></span>

# <a name="http"></a>[<span data-ttu-id="713fd-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="713fd-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="713fd-159">C#</span><span class="sxs-lookup"><span data-stu-id="713fd-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="713fd-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="713fd-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="713fd-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="713fd-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="713fd-162">响应</span><span class="sxs-lookup"><span data-stu-id="713fd-162">Response</span></span>

<span data-ttu-id="713fd-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="713fd-163">The following is an example of the response.</span></span>

><span data-ttu-id="713fd-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="713fd-164">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="713fd-165">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="713fd-165">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->


