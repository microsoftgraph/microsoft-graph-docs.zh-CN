---
title: 创建 mailFolder
description: 使用此 API 创建新的子 mailFolder。
ms.openlocfilehash: 44d9e9ebfd721a68734376342500ad1e2a182cda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045863"
---
# <a name="create-mailfolder"></a><span data-ttu-id="eec23-103">创建 mailFolder</span><span class="sxs-lookup"><span data-stu-id="eec23-103">Create mailFolder</span></span>

> <span data-ttu-id="eec23-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eec23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eec23-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eec23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eec23-106">使用此 API 创建新的子[mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="eec23-106">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eec23-107">权限</span><span class="sxs-lookup"><span data-stu-id="eec23-107">Permissions</span></span>

<span data-ttu-id="eec23-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eec23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eec23-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eec23-110">Permission type</span></span> | <span data-ttu-id="eec23-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eec23-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="eec23-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eec23-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eec23-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eec23-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eec23-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eec23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eec23-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eec23-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eec23-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eec23-116">Application</span></span> | <span data-ttu-id="eec23-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eec23-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eec23-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eec23-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="eec23-119">查询 URL 为文件夹 ID 或已知文件夹名称中指定的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="eec23-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="eec23-120">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="eec23-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eec23-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="eec23-121">Request headers</span></span>

| <span data-ttu-id="eec23-122">标头</span><span class="sxs-lookup"><span data-stu-id="eec23-122">Header</span></span> | <span data-ttu-id="eec23-123">值</span><span class="sxs-lookup"><span data-stu-id="eec23-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="eec23-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eec23-124">Authorization</span></span> | <span data-ttu-id="eec23-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="eec23-125"></span></span> <span data-ttu-id="eec23-126">必需。</span><span class="sxs-lookup"><span data-stu-id="eec23-126">Required.</span></span> |
| <span data-ttu-id="eec23-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eec23-127">Content-Type</span></span> | <span data-ttu-id="eec23-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="eec23-128"></span></span> <span data-ttu-id="eec23-129">必需。</span><span class="sxs-lookup"><span data-stu-id="eec23-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eec23-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="eec23-130">Request body</span></span>

<span data-ttu-id="eec23-p106">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="eec23-p106">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="eec23-133">参数</span><span class="sxs-lookup"><span data-stu-id="eec23-133">Parameter</span></span> | <span data-ttu-id="eec23-134">类型</span><span class="sxs-lookup"><span data-stu-id="eec23-134">Type</span></span> | <span data-ttu-id="eec23-135">说明</span><span class="sxs-lookup"><span data-stu-id="eec23-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="eec23-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eec23-136">displayName</span></span>|<span data-ttu-id="eec23-137">String</span><span class="sxs-lookup"><span data-stu-id="eec23-137">String</span></span>|<span data-ttu-id="eec23-138">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="eec23-138">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="eec23-139">响应</span><span class="sxs-lookup"><span data-stu-id="eec23-139">Response</span></span>

<span data-ttu-id="eec23-140">如果成功，此方法返回`201 Created`响应代码和响应正文中的[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eec23-140">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eec23-141">示例</span><span class="sxs-lookup"><span data-stu-id="eec23-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eec23-142">请求</span><span class="sxs-lookup"><span data-stu-id="eec23-142">Request</span></span>

<span data-ttu-id="eec23-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eec23-143">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="eec23-144">响应</span><span class="sxs-lookup"><span data-stu-id="eec23-144">Response</span></span>

<span data-ttu-id="eec23-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eec23-145">The following is an example of the response.</span></span>

> <span data-ttu-id="eec23-146">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eec23-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eec23-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eec23-147">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
