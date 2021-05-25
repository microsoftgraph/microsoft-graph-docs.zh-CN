---
title: 创建 MailFolder
description: 使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a60f7166337933a3ee8897f9817c6adb148bd05c
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629397"
---
# <a name="create-mailfolder"></a><span data-ttu-id="93377-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="93377-103">Create MailFolder</span></span>

<span data-ttu-id="93377-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93377-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93377-105">使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="93377-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>

<span data-ttu-id="93377-106">如果要隐藏新文件夹，必须在创建时将 **isHidden** `true` 属性设置为 。</span><span class="sxs-lookup"><span data-stu-id="93377-106">If you intend a new folder to be hidden, you must set the **isHidden** property to `true` on creation.</span></span>

## <a name="permissions"></a><span data-ttu-id="93377-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="93377-107">Permissions</span></span>
<span data-ttu-id="93377-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93377-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="93377-110">Permission type</span></span>      | <span data-ttu-id="93377-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93377-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93377-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93377-112">Delegated (work or school account)</span></span> | <span data-ttu-id="93377-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93377-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="93377-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93377-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93377-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93377-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="93377-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="93377-116">Application</span></span> | <span data-ttu-id="93377-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93377-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="93377-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93377-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="93377-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="93377-119">Request headers</span></span>
| <span data-ttu-id="93377-120">标头</span><span class="sxs-lookup"><span data-stu-id="93377-120">Header</span></span>       | <span data-ttu-id="93377-121">值</span><span class="sxs-lookup"><span data-stu-id="93377-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93377-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93377-122">Authorization</span></span>  | <span data-ttu-id="93377-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93377-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="93377-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93377-125">Content-Type</span></span>  | <span data-ttu-id="93377-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93377-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93377-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93377-127">Request body</span></span>
<span data-ttu-id="93377-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="93377-128">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="93377-129">**displayName** 和 **isHidden** 是 [mailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="93377-129">**displayName** and **isHidden** are the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="93377-130">参数</span><span class="sxs-lookup"><span data-stu-id="93377-130">Parameter</span></span>    | <span data-ttu-id="93377-131">类型</span><span class="sxs-lookup"><span data-stu-id="93377-131">Type</span></span>   |<span data-ttu-id="93377-132">说明</span><span class="sxs-lookup"><span data-stu-id="93377-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93377-133">displayName</span><span class="sxs-lookup"><span data-stu-id="93377-133">displayName</span></span>|<span data-ttu-id="93377-134">String</span><span class="sxs-lookup"><span data-stu-id="93377-134">String</span></span>|<span data-ttu-id="93377-135">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="93377-135">The display name of the new folder.</span></span>|
|<span data-ttu-id="93377-136">isHidden</span><span class="sxs-lookup"><span data-stu-id="93377-136">isHidden</span></span>|<span data-ttu-id="93377-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="93377-137">Boolean</span></span>|<span data-ttu-id="93377-138">指示是否隐藏新文件夹。</span><span class="sxs-lookup"><span data-stu-id="93377-138">Indicates whether the new folder is hidden.</span></span> <span data-ttu-id="93377-139">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="93377-139">The default value is `false`.</span></span> <span data-ttu-id="93377-140">设置属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="93377-140">Setting the property is optional.</span></span> <span data-ttu-id="93377-141">设置后，将不能更新此属性。</span><span class="sxs-lookup"><span data-stu-id="93377-141">Once set, you cannot update this property.</span></span> <span data-ttu-id="93377-142">在"隐藏邮件 [文件夹"中查看详细信息](../resources/mailfolder.md#hidden-mail-folders)</span><span class="sxs-lookup"><span data-stu-id="93377-142">See more information in [Hidden mail folders](../resources/mailfolder.md#hidden-mail-folders)</span></span>|

## <a name="response"></a><span data-ttu-id="93377-143">响应</span><span class="sxs-lookup"><span data-stu-id="93377-143">Response</span></span>

<span data-ttu-id="93377-144">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [mailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93377-144">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93377-145">示例</span><span class="sxs-lookup"><span data-stu-id="93377-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="93377-146">请求</span><span class="sxs-lookup"><span data-stu-id="93377-146">Request</span></span>
<span data-ttu-id="93377-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93377-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93377-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="93377-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "Clutter",
  "isHidden": true
}
```
# <a name="c"></a>[<span data-ttu-id="93377-149">C#</span><span class="sxs-lookup"><span data-stu-id="93377-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93377-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93377-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93377-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93377-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93377-152">Java</span><span class="sxs-lookup"><span data-stu-id="93377-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93377-153">响应</span><span class="sxs-lookup"><span data-stu-id="93377-153">Response</span></span>
<span data-ttu-id="93377-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="93377-154">Here is an example of the response.</span></span> 

><span data-ttu-id="93377-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="93377-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "Clutter",
  "parentFolderId": "AQMkADlmOGQwZmU3LWVjOWMtNDhiYgAtODcxNy1",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "hN2Y5OGRhNGYwODEALgAAA0DAKbvJvFhJgcT3lZpkhNQBAA1",
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

