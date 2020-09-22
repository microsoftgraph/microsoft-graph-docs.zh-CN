---
title: 创建 MailFolder
description: 使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5b8e6c41de41f23b5a8b3d6e1a31394773c666b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064540"
---
# <a name="create-mailfolder"></a><span data-ttu-id="b5e28-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="b5e28-103">Create MailFolder</span></span>

<span data-ttu-id="b5e28-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e28-105">使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="b5e28-105">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5e28-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5e28-106">Permissions</span></span>
<span data-ttu-id="b5e28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5e28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5e28-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5e28-109">Permission type</span></span>      | <span data-ttu-id="b5e28-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5e28-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5e28-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5e28-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5e28-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e28-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b5e28-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5e28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e28-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e28-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b5e28-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5e28-115">Application</span></span> | <span data-ttu-id="b5e28-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e28-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e28-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5e28-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="b5e28-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5e28-118">Request headers</span></span>
| <span data-ttu-id="b5e28-119">标头</span><span class="sxs-lookup"><span data-stu-id="b5e28-119">Header</span></span>       | <span data-ttu-id="b5e28-120">值</span><span class="sxs-lookup"><span data-stu-id="b5e28-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5e28-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e28-121">Authorization</span></span>  | <span data-ttu-id="b5e28-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5e28-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b5e28-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5e28-124">Content-Type</span></span>  | <span data-ttu-id="b5e28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5e28-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5e28-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5e28-126">Request body</span></span>
<span data-ttu-id="b5e28-p103">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="b5e28-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="b5e28-129">参数</span><span class="sxs-lookup"><span data-stu-id="b5e28-129">Parameter</span></span>    | <span data-ttu-id="b5e28-130">类型</span><span class="sxs-lookup"><span data-stu-id="b5e28-130">Type</span></span>   |<span data-ttu-id="b5e28-131">说明</span><span class="sxs-lookup"><span data-stu-id="b5e28-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5e28-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b5e28-132">displayName</span></span>|<span data-ttu-id="b5e28-133">String</span><span class="sxs-lookup"><span data-stu-id="b5e28-133">String</span></span>|<span data-ttu-id="b5e28-134">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b5e28-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="b5e28-135">响应</span><span class="sxs-lookup"><span data-stu-id="b5e28-135">Response</span></span>

<span data-ttu-id="b5e28-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5e28-136">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5e28-137">示例</span><span class="sxs-lookup"><span data-stu-id="b5e28-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5e28-138">请求</span><span class="sxs-lookup"><span data-stu-id="b5e28-138">Request</span></span>
<span data-ttu-id="b5e28-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5e28-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5e28-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e28-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b5e28-141">C#</span><span class="sxs-lookup"><span data-stu-id="b5e28-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e28-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e28-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e28-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e28-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5e28-144">响应</span><span class="sxs-lookup"><span data-stu-id="b5e28-144">Response</span></span>
<span data-ttu-id="b5e28-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5e28-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


