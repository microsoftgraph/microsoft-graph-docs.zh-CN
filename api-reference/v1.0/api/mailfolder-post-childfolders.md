---
title: 创建 MailFolder
description: 使用此 API 新建子 MailFolder。
author: angelgolfer-ms
ms.openlocfilehash: 717baa63f3bb15355eaf59387b8fc701ab1288b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331519"
---
# <a name="create-mailfolder"></a><span data-ttu-id="78e21-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="78e21-103">Create MailFolder</span></span>

<span data-ttu-id="78e21-104">使用此 API 新建子 MailFolder。</span><span class="sxs-lookup"><span data-stu-id="78e21-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="78e21-105">权限</span><span class="sxs-lookup"><span data-stu-id="78e21-105">Permissions</span></span>

<span data-ttu-id="78e21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78e21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78e21-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78e21-108">Permission type</span></span> | <span data-ttu-id="78e21-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78e21-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="78e21-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78e21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78e21-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78e21-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="78e21-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78e21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78e21-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78e21-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="78e21-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78e21-114">Application</span></span> | <span data-ttu-id="78e21-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78e21-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="78e21-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78e21-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="78e21-117">查询 URL 为文件夹 ID 或已知文件夹名称中指定的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="78e21-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="78e21-118">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="78e21-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="78e21-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="78e21-119">Request headers</span></span>

| <span data-ttu-id="78e21-120">标头</span><span class="sxs-lookup"><span data-stu-id="78e21-120">Header</span></span> | <span data-ttu-id="78e21-121">值</span><span class="sxs-lookup"><span data-stu-id="78e21-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="78e21-122">授权</span><span class="sxs-lookup"><span data-stu-id="78e21-122">Authorization</span></span> | <span data-ttu-id="78e21-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="78e21-123"></span></span> <span data-ttu-id="78e21-124">必需。</span><span class="sxs-lookup"><span data-stu-id="78e21-124">Required.</span></span> |
| <span data-ttu-id="78e21-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78e21-125">Content-Type</span></span> | <span data-ttu-id="78e21-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="78e21-126"></span></span> <span data-ttu-id="78e21-127">必需。</span><span class="sxs-lookup"><span data-stu-id="78e21-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78e21-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="78e21-128">Request body</span></span>

<span data-ttu-id="78e21-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="78e21-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="78e21-130">**displayName**是[mailFolder](../resources/mailfolder.md)对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="78e21-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="78e21-131">参数</span><span class="sxs-lookup"><span data-stu-id="78e21-131">Parameter</span></span> | <span data-ttu-id="78e21-132">Type</span><span class="sxs-lookup"><span data-stu-id="78e21-132">Type</span></span> | <span data-ttu-id="78e21-133">说明</span><span class="sxs-lookup"><span data-stu-id="78e21-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="78e21-134">displayName</span><span class="sxs-lookup"><span data-stu-id="78e21-134">displayName</span></span>|<span data-ttu-id="78e21-135">String</span><span class="sxs-lookup"><span data-stu-id="78e21-135">String</span></span>|<span data-ttu-id="78e21-136">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="78e21-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="78e21-137">响应</span><span class="sxs-lookup"><span data-stu-id="78e21-137">Response</span></span>

<span data-ttu-id="78e21-138">如果成功，此方法返回`201 Created`响应代码和响应正文的[mailFolder](../resources/mailfolder.md)资源。</span><span class="sxs-lookup"><span data-stu-id="78e21-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e21-139">示例</span><span class="sxs-lookup"><span data-stu-id="78e21-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="78e21-140">请求</span><span class="sxs-lookup"><span data-stu-id="78e21-140">Request</span></span>

<span data-ttu-id="78e21-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78e21-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="78e21-142">响应</span><span class="sxs-lookup"><span data-stu-id="78e21-142">Response</span></span>
<span data-ttu-id="78e21-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78e21-143">Here is an example of the response.</span></span>

> <span data-ttu-id="78e21-144">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="78e21-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="78e21-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78e21-145">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
