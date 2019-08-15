---
title: 创建 MailFolder
description: 使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9baaf507c8efb8d8a5cf56ed95abd62da5e056a3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421881"
---
# <a name="create-mailfolder"></a><span data-ttu-id="cf612-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="cf612-103">Create MailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf612-104">使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="cf612-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf612-105">权限</span><span class="sxs-lookup"><span data-stu-id="cf612-105">Permissions</span></span>
<span data-ttu-id="cf612-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf612-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf612-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf612-108">Permission type</span></span>      | <span data-ttu-id="cf612-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf612-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf612-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf612-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf612-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf612-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cf612-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf612-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf612-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf612-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cf612-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf612-114">Application</span></span> | <span data-ttu-id="cf612-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf612-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf612-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf612-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="cf612-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf612-117">Request headers</span></span>
| <span data-ttu-id="cf612-118">标头</span><span class="sxs-lookup"><span data-stu-id="cf612-118">Header</span></span>       | <span data-ttu-id="cf612-119">值</span><span class="sxs-lookup"><span data-stu-id="cf612-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf612-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf612-120">Authorization</span></span>  | <span data-ttu-id="cf612-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf612-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf612-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf612-123">Content-Type</span></span>  | <span data-ttu-id="cf612-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf612-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf612-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf612-125">Request body</span></span>
<span data-ttu-id="cf612-p103">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="cf612-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="cf612-128">参数</span><span class="sxs-lookup"><span data-stu-id="cf612-128">Parameter</span></span>    | <span data-ttu-id="cf612-129">类型</span><span class="sxs-lookup"><span data-stu-id="cf612-129">Type</span></span>   |<span data-ttu-id="cf612-130">说明</span><span class="sxs-lookup"><span data-stu-id="cf612-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf612-131">displayName</span><span class="sxs-lookup"><span data-stu-id="cf612-131">displayName</span></span>|<span data-ttu-id="cf612-132">String</span><span class="sxs-lookup"><span data-stu-id="cf612-132">String</span></span>|<span data-ttu-id="cf612-133">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cf612-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="cf612-134">响应</span><span class="sxs-lookup"><span data-stu-id="cf612-134">Response</span></span>

<span data-ttu-id="cf612-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf612-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf612-136">示例</span><span class="sxs-lookup"><span data-stu-id="cf612-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf612-137">请求</span><span class="sxs-lookup"><span data-stu-id="cf612-137">Request</span></span>
<span data-ttu-id="cf612-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf612-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cf612-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="cf612-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cf612-140">C#</span><span class="sxs-lookup"><span data-stu-id="cf612-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf612-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf612-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cf612-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="cf612-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cf612-143">响应</span><span class="sxs-lookup"><span data-stu-id="cf612-143">Response</span></span>
<span data-ttu-id="cf612-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf612-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
