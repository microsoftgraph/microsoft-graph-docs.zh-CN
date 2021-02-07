---
title: 创建 MailFolder
description: 使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 434e3ae114f0514ad002939aa1a39f82b0c31455
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137219"
---
# <a name="create-mailfolder"></a><span data-ttu-id="4e02d-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="4e02d-103">Create MailFolder</span></span>

<span data-ttu-id="4e02d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e02d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e02d-105">使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="4e02d-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e02d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4e02d-106">Permissions</span></span>
<span data-ttu-id="4e02d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e02d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e02d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e02d-109">Permission type</span></span>      | <span data-ttu-id="4e02d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e02d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e02d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e02d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4e02d-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e02d-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4e02d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e02d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e02d-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e02d-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4e02d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e02d-115">Application</span></span> | <span data-ttu-id="4e02d-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e02d-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e02d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e02d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="4e02d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e02d-118">Request headers</span></span>
| <span data-ttu-id="4e02d-119">标头</span><span class="sxs-lookup"><span data-stu-id="4e02d-119">Header</span></span>       | <span data-ttu-id="4e02d-120">值</span><span class="sxs-lookup"><span data-stu-id="4e02d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e02d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e02d-121">Authorization</span></span>  | <span data-ttu-id="4e02d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e02d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e02d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e02d-124">Content-Type</span></span>  | <span data-ttu-id="4e02d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e02d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e02d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e02d-126">Request body</span></span>
<span data-ttu-id="4e02d-p103">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="4e02d-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="4e02d-129">参数</span><span class="sxs-lookup"><span data-stu-id="4e02d-129">Parameter</span></span>    | <span data-ttu-id="4e02d-130">类型</span><span class="sxs-lookup"><span data-stu-id="4e02d-130">Type</span></span>   |<span data-ttu-id="4e02d-131">说明</span><span class="sxs-lookup"><span data-stu-id="4e02d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e02d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4e02d-132">displayName</span></span>|<span data-ttu-id="4e02d-133">String</span><span class="sxs-lookup"><span data-stu-id="4e02d-133">String</span></span>|<span data-ttu-id="4e02d-134">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4e02d-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="4e02d-135">响应</span><span class="sxs-lookup"><span data-stu-id="4e02d-135">Response</span></span>

<span data-ttu-id="4e02d-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e02d-136">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e02d-137">示例</span><span class="sxs-lookup"><span data-stu-id="4e02d-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e02d-138">请求</span><span class="sxs-lookup"><span data-stu-id="4e02d-138">Request</span></span>
<span data-ttu-id="4e02d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e02d-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e02d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e02d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "Clutter"
}
```
# <a name="c"></a>[<span data-ttu-id="4e02d-141">C#</span><span class="sxs-lookup"><span data-stu-id="4e02d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e02d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e02d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e02d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e02d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e02d-144">Java</span><span class="sxs-lookup"><span data-stu-id="4e02d-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e02d-145">响应</span><span class="sxs-lookup"><span data-stu-id="4e02d-145">Response</span></span>
<span data-ttu-id="4e02d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e02d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "hN2Y5OGRhNGYwODEALgAAA0DAKbvJvFhJgcT3lZpkhNQBAA1"
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

