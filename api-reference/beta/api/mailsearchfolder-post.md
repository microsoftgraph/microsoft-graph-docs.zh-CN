---
title: 创建 mailSearchFolder
description: 此 API 用于指定的用户的邮箱中创建新 mailSearchFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ef9992e1b0eaee83c39831424215cb9756f895d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517727"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="61b45-103">创建 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="61b45-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61b45-104">此 API 用于指定的用户的邮箱中创建新[mailSearchFolder](../resources/mailsearchfolder.md) 。</span><span class="sxs-lookup"><span data-stu-id="61b45-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="61b45-105">权限</span><span class="sxs-lookup"><span data-stu-id="61b45-105">Permissions</span></span>

<span data-ttu-id="61b45-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61b45-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="61b45-108">Permission type</span></span> | <span data-ttu-id="61b45-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61b45-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="61b45-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61b45-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61b45-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b45-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61b45-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61b45-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61b45-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b45-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61b45-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="61b45-114">Application</span></span> | <span data-ttu-id="61b45-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b45-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="61b45-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61b45-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="61b45-117">查询 URL 为文件夹 ID 或已知文件夹名称中指定的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="61b45-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="61b45-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="61b45-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="61b45-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="61b45-119">Request headers</span></span>

| <span data-ttu-id="61b45-120">标头</span><span class="sxs-lookup"><span data-stu-id="61b45-120">Header</span></span> | <span data-ttu-id="61b45-121">值</span><span class="sxs-lookup"><span data-stu-id="61b45-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="61b45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61b45-122">Authorization</span></span> | <span data-ttu-id="61b45-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="61b45-123"></span></span> <span data-ttu-id="61b45-124">必需。</span><span class="sxs-lookup"><span data-stu-id="61b45-124">Required.</span></span> |
| <span data-ttu-id="61b45-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61b45-125">Content-Type</span></span> | <span data-ttu-id="61b45-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="61b45-126"></span></span> <span data-ttu-id="61b45-127">必需。</span><span class="sxs-lookup"><span data-stu-id="61b45-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61b45-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="61b45-128">Request body</span></span>

<span data-ttu-id="61b45-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="61b45-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="61b45-130">参数</span><span class="sxs-lookup"><span data-stu-id="61b45-130">Parameter</span></span> | <span data-ttu-id="61b45-131">类型</span><span class="sxs-lookup"><span data-stu-id="61b45-131">Type</span></span> | <span data-ttu-id="61b45-132">说明</span><span class="sxs-lookup"><span data-stu-id="61b45-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="61b45-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="61b45-133">@odata.type</span></span> | <span data-ttu-id="61b45-134">String</span><span class="sxs-lookup"><span data-stu-id="61b45-134">String</span></span> | <span data-ttu-id="61b45-135">要创建的文件夹的类型。</span><span class="sxs-lookup"><span data-stu-id="61b45-135">The type of folder to be created.</span></span> <span data-ttu-id="61b45-136">设置为"microsoft.graph.mailSearchFolder"。</span><span class="sxs-lookup"><span data-stu-id="61b45-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="61b45-137">displayName</span><span class="sxs-lookup"><span data-stu-id="61b45-137">displayName</span></span> | <span data-ttu-id="61b45-138">String</span><span class="sxs-lookup"><span data-stu-id="61b45-138">String</span></span> | <span data-ttu-id="61b45-139">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="61b45-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="61b45-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="61b45-140">includeNestedFolders</span></span> | <span data-ttu-id="61b45-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="61b45-141">Boolean</span></span> | <span data-ttu-id="61b45-142">如何应遍历的邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="61b45-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="61b45-143">`true`意味着应为深入搜索完成时`false`意味着浅表搜索应改为完成。</span><span class="sxs-lookup"><span data-stu-id="61b45-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="61b45-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="61b45-144">sourceFolderIDs</span></span> | <span data-ttu-id="61b45-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="61b45-145">String collection</span></span> | <span data-ttu-id="61b45-146">应 mined 邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="61b45-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="61b45-147">filterQuery</span><span class="sxs-lookup"><span data-stu-id="61b45-147">filterQuery</span></span> | <span data-ttu-id="61b45-148">String</span><span class="sxs-lookup"><span data-stu-id="61b45-148">String</span></span> | <span data-ttu-id="61b45-149">要筛选的邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="61b45-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="61b45-150">响应</span><span class="sxs-lookup"><span data-stu-id="61b45-150">Response</span></span>

<span data-ttu-id="61b45-151">如果成功，此方法返回`201 Created`响应代码和响应正文中的[mailSearchFolder](../resources/mailsearchfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="61b45-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61b45-152">示例</span><span class="sxs-lookup"><span data-stu-id="61b45-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="61b45-153">请求</span><span class="sxs-lookup"><span data-stu-id="61b45-153">Request</span></span>

<span data-ttu-id="61b45-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61b45-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a><span data-ttu-id="61b45-155">响应</span><span class="sxs-lookup"><span data-stu-id="61b45-155">Response</span></span>

<span data-ttu-id="61b45-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="61b45-156">The following is an example of the response.</span></span>

><span data-ttu-id="61b45-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="61b45-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="61b45-158">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="61b45-158">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
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
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
