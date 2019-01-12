---
title: 创建 mailSearchFolder
description: 此 API 用于指定的用户的邮箱中创建新 mailSearchFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 626bf3a2e8bc77ba929895eed74ac0bb803aa5d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912874"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="0ac0d-103">创建 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="0ac0d-103">Create mailSearchFolder</span></span>

> <span data-ttu-id="0ac0d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ac0d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ac0d-106">此 API 用于指定的用户的邮箱中创建新[mailSearchFolder](../resources/mailsearchfolder.md) 。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-106">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ac0d-107">权限</span><span class="sxs-lookup"><span data-stu-id="0ac0d-107">Permissions</span></span>

<span data-ttu-id="0ac0d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ac0d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ac0d-110">Permission type</span></span> | <span data-ttu-id="0ac0d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ac0d-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="0ac0d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac0d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ac0d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac0d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ac0d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac0d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ac0d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac0d-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ac0d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ac0d-116">Application</span></span> | <span data-ttu-id="0ac0d-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac0d-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ac0d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ac0d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="0ac0d-119">查询 URL 为文件夹 ID 或已知文件夹名称中指定的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="0ac0d-120">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ac0d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ac0d-121">Request headers</span></span>

| <span data-ttu-id="0ac0d-122">标头</span><span class="sxs-lookup"><span data-stu-id="0ac0d-122">Header</span></span> | <span data-ttu-id="0ac0d-123">值</span><span class="sxs-lookup"><span data-stu-id="0ac0d-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="0ac0d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac0d-124">Authorization</span></span> | <span data-ttu-id="0ac0d-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="0ac0d-125"></span></span> <span data-ttu-id="0ac0d-126">必填。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-126">Required.</span></span> |
| <span data-ttu-id="0ac0d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ac0d-127">Content-Type</span></span> | <span data-ttu-id="0ac0d-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="0ac0d-128"></span></span> <span data-ttu-id="0ac0d-129">必填。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ac0d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ac0d-130">Request body</span></span>

<span data-ttu-id="0ac0d-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ac0d-132">参数</span><span class="sxs-lookup"><span data-stu-id="0ac0d-132">Parameter</span></span> | <span data-ttu-id="0ac0d-133">类型</span><span class="sxs-lookup"><span data-stu-id="0ac0d-133">Type</span></span> | <span data-ttu-id="0ac0d-134">说明</span><span class="sxs-lookup"><span data-stu-id="0ac0d-134">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="0ac0d-135">@odata.type</span><span class="sxs-lookup"><span data-stu-id="0ac0d-135">@odata.type</span></span> | <span data-ttu-id="0ac0d-136">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac0d-136">String</span></span> | <span data-ttu-id="0ac0d-137">要创建的文件夹的类型。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-137">The type of folder to be created.</span></span> <span data-ttu-id="0ac0d-138">设置为"microsoft.graph.mailSearchFolder"。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-138">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="0ac0d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac0d-139">displayName</span></span> | <span data-ttu-id="0ac0d-140">String</span><span class="sxs-lookup"><span data-stu-id="0ac0d-140">String</span></span> | <span data-ttu-id="0ac0d-141">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-141">The display name of the new folder.</span></span>|
| <span data-ttu-id="0ac0d-142">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="0ac0d-142">includeNestedFolders</span></span> | <span data-ttu-id="0ac0d-143">布尔</span><span class="sxs-lookup"><span data-stu-id="0ac0d-143">Boolean</span></span> | <span data-ttu-id="0ac0d-144">如何应遍历的邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-144">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="0ac0d-145">`true`意味着应为深入搜索完成时`false`意味着浅表搜索应改为完成。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-145">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="0ac0d-146">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="0ac0d-146">sourceFolderIDs</span></span> | <span data-ttu-id="0ac0d-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ac0d-147">String collection</span></span> | <span data-ttu-id="0ac0d-148">应 mined 邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="0ac0d-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="0ac0d-149">filterQuery</span></span> | <span data-ttu-id="0ac0d-150">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac0d-150">String</span></span> | <span data-ttu-id="0ac0d-151">要筛选的邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="0ac0d-152">响应</span><span class="sxs-lookup"><span data-stu-id="0ac0d-152">Response</span></span>

<span data-ttu-id="0ac0d-153">如果成功，此方法返回`201 Created`响应代码和响应正文中的[mailSearchFolder](../resources/mailsearchfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-153">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac0d-154">示例</span><span class="sxs-lookup"><span data-stu-id="0ac0d-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0ac0d-155">请求</span><span class="sxs-lookup"><span data-stu-id="0ac0d-155">Request</span></span>

<span data-ttu-id="0ac0d-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-156">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="0ac0d-157">响应</span><span class="sxs-lookup"><span data-stu-id="0ac0d-157">Response</span></span>

<span data-ttu-id="0ac0d-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-158">The following is an example of the response.</span></span>

><span data-ttu-id="0ac0d-159">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ac0d-160">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0ac0d-160">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
