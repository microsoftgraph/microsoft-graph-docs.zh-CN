---
title: 创建 MailFolder
description: 使用此 API 新建子 MailFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 92c57b5336eb60377915a4abc64b070b28bb98ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516488"
---
# <a name="create-mailfolder"></a><span data-ttu-id="e9520-103">Create mailFolder</span><span class="sxs-lookup"><span data-stu-id="e9520-103">Create mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9520-104">使用此 API 新建子 MailFolder。</span><span class="sxs-lookup"><span data-stu-id="e9520-104">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9520-105">权限</span><span class="sxs-lookup"><span data-stu-id="e9520-105">Permissions</span></span>

<span data-ttu-id="e9520-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9520-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9520-108">Permission type</span></span> | <span data-ttu-id="e9520-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9520-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="e9520-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9520-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9520-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9520-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e9520-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9520-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9520-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9520-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e9520-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9520-114">Application</span></span> | <span data-ttu-id="e9520-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9520-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9520-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9520-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="e9520-117">查询 URL 为文件夹 ID 或已知文件夹名称中指定的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="e9520-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="e9520-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="e9520-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9520-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9520-119">Request headers</span></span>

| <span data-ttu-id="e9520-120">标头</span><span class="sxs-lookup"><span data-stu-id="e9520-120">Header</span></span> | <span data-ttu-id="e9520-121">值</span><span class="sxs-lookup"><span data-stu-id="e9520-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="e9520-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9520-122">Authorization</span></span> | <span data-ttu-id="e9520-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="e9520-123"></span></span> <span data-ttu-id="e9520-124">必需。</span><span class="sxs-lookup"><span data-stu-id="e9520-124">Required.</span></span> |
| <span data-ttu-id="e9520-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9520-125">Content-Type</span></span> | <span data-ttu-id="e9520-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="e9520-126"></span></span> <span data-ttu-id="e9520-127">必需。</span><span class="sxs-lookup"><span data-stu-id="e9520-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9520-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9520-128">Request body</span></span>

<span data-ttu-id="e9520-p105">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="e9520-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="e9520-131">参数</span><span class="sxs-lookup"><span data-stu-id="e9520-131">Parameter</span></span> | <span data-ttu-id="e9520-132">类型</span><span class="sxs-lookup"><span data-stu-id="e9520-132">Type</span></span> | <span data-ttu-id="e9520-133">说明</span><span class="sxs-lookup"><span data-stu-id="e9520-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="e9520-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e9520-134">displayName</span></span>|<span data-ttu-id="e9520-135">String</span><span class="sxs-lookup"><span data-stu-id="e9520-135">String</span></span>|<span data-ttu-id="e9520-136">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e9520-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e9520-137">响应</span><span class="sxs-lookup"><span data-stu-id="e9520-137">Response</span></span>

<span data-ttu-id="e9520-138">如果成功，此方法返回`201 Created`响应代码和响应正文中的[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e9520-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9520-139">示例</span><span class="sxs-lookup"><span data-stu-id="e9520-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e9520-140">请求</span><span class="sxs-lookup"><span data-stu-id="e9520-140">Request</span></span>

<span data-ttu-id="e9520-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e9520-141">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="e9520-142">响应</span><span class="sxs-lookup"><span data-stu-id="e9520-142">Response</span></span>

<span data-ttu-id="e9520-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e9520-143">The following is an example of the response.</span></span>

> <span data-ttu-id="e9520-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9520-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e9520-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e9520-145">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/mailfolder-post-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
