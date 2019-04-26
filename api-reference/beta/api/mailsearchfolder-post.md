---
title: 创建 mailSearchFolder
description: 使用此 API 在指定用户的邮箱中创建新的 mailSearchFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bdebbcb9c842d57d4c6ee8d8eb72f45df74a22d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333307"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="aa2a3-103">创建 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="aa2a3-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa2a3-104">使用此 API 在指定用户的邮箱中创建新的[mailSearchFolder](../resources/mailsearchfolder.md) 。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa2a3-105">权限</span><span class="sxs-lookup"><span data-stu-id="aa2a3-105">Permissions</span></span>

<span data-ttu-id="aa2a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa2a3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa2a3-108">Permission type</span></span> | <span data-ttu-id="aa2a3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa2a3-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="aa2a3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa2a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa2a3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa2a3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aa2a3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa2a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa2a3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa2a3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aa2a3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa2a3-114">Application</span></span> | <span data-ttu-id="aa2a3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa2a3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa2a3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa2a3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="aa2a3-117">将查询 URL 中的父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="aa2a3-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa2a3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa2a3-119">Request headers</span></span>

| <span data-ttu-id="aa2a3-120">标头</span><span class="sxs-lookup"><span data-stu-id="aa2a3-120">Header</span></span> | <span data-ttu-id="aa2a3-121">值</span><span class="sxs-lookup"><span data-stu-id="aa2a3-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="aa2a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa2a3-122">Authorization</span></span> | <span data-ttu-id="aa2a3-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="aa2a3-123"></span></span> <span data-ttu-id="aa2a3-124">必需。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-124">Required.</span></span> |
| <span data-ttu-id="aa2a3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa2a3-125">Content-Type</span></span> | <span data-ttu-id="aa2a3-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="aa2a3-126"></span></span> <span data-ttu-id="aa2a3-127">必填。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa2a3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa2a3-128">Request body</span></span>

<span data-ttu-id="aa2a3-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aa2a3-130">参数</span><span class="sxs-lookup"><span data-stu-id="aa2a3-130">Parameter</span></span> | <span data-ttu-id="aa2a3-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa2a3-131">Type</span></span> | <span data-ttu-id="aa2a3-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa2a3-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="aa2a3-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="aa2a3-133">@odata.type</span></span> | <span data-ttu-id="aa2a3-134">String</span><span class="sxs-lookup"><span data-stu-id="aa2a3-134">String</span></span> | <span data-ttu-id="aa2a3-135">要创建的文件夹的类型。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-135">The type of folder to be created.</span></span> <span data-ttu-id="aa2a3-136">设置为 "mailSearchFolder"。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="aa2a3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="aa2a3-137">displayName</span></span> | <span data-ttu-id="aa2a3-138">String</span><span class="sxs-lookup"><span data-stu-id="aa2a3-138">String</span></span> | <span data-ttu-id="aa2a3-139">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="aa2a3-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="aa2a3-140">includeNestedFolders</span></span> | <span data-ttu-id="aa2a3-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa2a3-141">Boolean</span></span> | <span data-ttu-id="aa2a3-142">应如何遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="aa2a3-143">`true`表示应执行深入搜索, 而不是`false`指应改为进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="aa2a3-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="aa2a3-144">sourceFolderIDs</span></span> | <span data-ttu-id="aa2a3-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="aa2a3-145">String collection</span></span> | <span data-ttu-id="aa2a3-146">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="aa2a3-147">filterQuery</span><span class="sxs-lookup"><span data-stu-id="aa2a3-147">filterQuery</span></span> | <span data-ttu-id="aa2a3-148">String</span><span class="sxs-lookup"><span data-stu-id="aa2a3-148">String</span></span> | <span data-ttu-id="aa2a3-149">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="aa2a3-150">响应</span><span class="sxs-lookup"><span data-stu-id="aa2a3-150">Response</span></span>

<span data-ttu-id="aa2a3-151">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[mailSearchFolder](../resources/mailsearchfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa2a3-152">示例</span><span class="sxs-lookup"><span data-stu-id="aa2a3-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aa2a3-153">请求</span><span class="sxs-lookup"><span data-stu-id="aa2a3-153">Request</span></span>

<span data-ttu-id="aa2a3-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-154">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="aa2a3-155">响应</span><span class="sxs-lookup"><span data-stu-id="aa2a3-155">Response</span></span>

<span data-ttu-id="aa2a3-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-156">The following is an example of the response.</span></span>

><span data-ttu-id="aa2a3-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aa2a3-158">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aa2a3-158">All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
