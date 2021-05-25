---
title: 创建子文件夹
description: 使用此 API 新建子 MailFolder。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4d8d43e4bb3840fa248ab6b1f1109dc2061ff695
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629138"
---
# <a name="create-child-folder"></a><span data-ttu-id="2e5c3-103">创建子文件夹</span><span class="sxs-lookup"><span data-stu-id="2e5c3-103">Create child folder</span></span>

<span data-ttu-id="2e5c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e5c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e5c3-105">使用此 API 创建新的子 [mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-105">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="2e5c3-106">如果要隐藏新文件夹，必须在创建时将 **isHidden** `true` 属性设置为 。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-106">If you intend a new folder to be hidden, you must set the **isHidden** property to `true` on creation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e5c3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2e5c3-107">Permissions</span></span>

<span data-ttu-id="2e5c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e5c3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e5c3-110">Permission type</span></span> | <span data-ttu-id="2e5c3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e5c3-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="2e5c3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e5c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2e5c3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e5c3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2e5c3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e5c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e5c3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e5c3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2e5c3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e5c3-116">Application</span></span> | <span data-ttu-id="2e5c3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e5c3-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e5c3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e5c3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="2e5c3-119">在查询 URL 中将父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="2e5c3-120">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e5c3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e5c3-121">Request headers</span></span>

| <span data-ttu-id="2e5c3-122">标头</span><span class="sxs-lookup"><span data-stu-id="2e5c3-122">Header</span></span> | <span data-ttu-id="2e5c3-123">值</span><span class="sxs-lookup"><span data-stu-id="2e5c3-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="2e5c3-124">授权</span><span class="sxs-lookup"><span data-stu-id="2e5c3-124">Authorization</span></span> | <span data-ttu-id="2e5c3-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="2e5c3-125">`Bearer {token}`.</span></span> <span data-ttu-id="2e5c3-126">必需。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-126">Required.</span></span> |
| <span data-ttu-id="2e5c3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e5c3-127">Content-Type</span></span> | <span data-ttu-id="2e5c3-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="2e5c3-128">`application/json`.</span></span> <span data-ttu-id="2e5c3-129">必需。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e5c3-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e5c3-130">Request body</span></span>

<span data-ttu-id="2e5c3-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-131">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="2e5c3-132">**displayName** 和 **isHidden** 是 [mailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-132">**displayName** and **isHidden** are the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="2e5c3-133">参数</span><span class="sxs-lookup"><span data-stu-id="2e5c3-133">Parameter</span></span> | <span data-ttu-id="2e5c3-134">类型</span><span class="sxs-lookup"><span data-stu-id="2e5c3-134">Type</span></span> | <span data-ttu-id="2e5c3-135">说明</span><span class="sxs-lookup"><span data-stu-id="2e5c3-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="2e5c3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2e5c3-136">displayName</span></span>|<span data-ttu-id="2e5c3-137">String</span><span class="sxs-lookup"><span data-stu-id="2e5c3-137">String</span></span>|<span data-ttu-id="2e5c3-138">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-138">The display name of the new folder.</span></span>|
|<span data-ttu-id="2e5c3-139">isHidden</span><span class="sxs-lookup"><span data-stu-id="2e5c3-139">isHidden</span></span>|<span data-ttu-id="2e5c3-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="2e5c3-140">Boolean</span></span>|<span data-ttu-id="2e5c3-141">指示是否隐藏新文件夹。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-141">Indicates whether the new folder is hidden.</span></span> <span data-ttu-id="2e5c3-142">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-142">The default value is `false`.</span></span> <span data-ttu-id="2e5c3-143">设置属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-143">Setting the property is optional.</span></span> <span data-ttu-id="2e5c3-144">设置后，将不能更新此属性。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-144">Once set, you cannot update this property.</span></span> <span data-ttu-id="2e5c3-145">在"隐藏邮件 [文件夹"中查看详细信息](../resources/mailfolder.md#hidden-mail-folders)</span><span class="sxs-lookup"><span data-stu-id="2e5c3-145">See more information in [Hidden mail folders](../resources/mailfolder.md#hidden-mail-folders)</span></span>|

## <a name="response"></a><span data-ttu-id="2e5c3-146">响应</span><span class="sxs-lookup"><span data-stu-id="2e5c3-146">Response</span></span>

<span data-ttu-id="2e5c3-147">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [mailFolder](../resources/mailfolder.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-147">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e5c3-148">示例</span><span class="sxs-lookup"><span data-stu-id="2e5c3-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e5c3-149">请求</span><span class="sxs-lookup"><span data-stu-id="2e5c3-149">Request</span></span>

<span data-ttu-id="2e5c3-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e5c3-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e5c3-151">HTTP</span></span>](#tab/http)
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
  "isHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="2e5c3-152">C#</span><span class="sxs-lookup"><span data-stu-id="2e5c3-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e5c3-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e5c3-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e5c3-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e5c3-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e5c3-155">Java</span><span class="sxs-lookup"><span data-stu-id="2e5c3-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2e5c3-156">响应</span><span class="sxs-lookup"><span data-stu-id="2e5c3-156">Response</span></span>
<span data-ttu-id="2e5c3-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-157">Here is an example of the response.</span></span>

> <span data-ttu-id="2e5c3-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "id-value",
  "isHidden": true
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

