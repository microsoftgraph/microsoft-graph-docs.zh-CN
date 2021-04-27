---
title: 创建 ContactFolder
description: '创建新的 contactFolder 作为指定文件夹的子文件夹。 '
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 93406ad1b66c1ff5300510abba1aeb0829ba03e9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047075"
---
# <a name="create-contactfolder"></a><span data-ttu-id="e7fd9-103">创建 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="e7fd9-103">Create ContactFolder</span></span>

<span data-ttu-id="e7fd9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7fd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7fd9-105">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-105">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="e7fd9-106">还可以[在用户的默认联系人文件夹下创建新的 contactFolder](user-post-contactfolders.md)。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-106">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e7fd9-107">权限</span><span class="sxs-lookup"><span data-stu-id="e7fd9-107">Permissions</span></span>
<span data-ttu-id="e7fd9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7fd9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7fd9-110">Permission type</span></span>      | <span data-ttu-id="e7fd9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7fd9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7fd9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7fd9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e7fd9-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7fd9-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e7fd9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7fd9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7fd9-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7fd9-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e7fd9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7fd9-116">Application</span></span> | <span data-ttu-id="e7fd9-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7fd9-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7fd9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7fd9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="e7fd9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7fd9-119">Request headers</span></span>
| <span data-ttu-id="e7fd9-120">标头</span><span class="sxs-lookup"><span data-stu-id="e7fd9-120">Header</span></span>       | <span data-ttu-id="e7fd9-121">值</span><span class="sxs-lookup"><span data-stu-id="e7fd9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7fd9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7fd9-122">Authorization</span></span>  | <span data-ttu-id="e7fd9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e7fd9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7fd9-125">Content-Type</span></span>  | <span data-ttu-id="e7fd9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e7fd9-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7fd9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7fd9-128">Request body</span></span>
<span data-ttu-id="e7fd9-129">在请求正文中，提供 [ContactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e7fd9-130">响应</span><span class="sxs-lookup"><span data-stu-id="e7fd9-130">Response</span></span>

<span data-ttu-id="e7fd9-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7fd9-132">示例</span><span class="sxs-lookup"><span data-stu-id="e7fd9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7fd9-133">请求</span><span class="sxs-lookup"><span data-stu-id="e7fd9-133">Request</span></span>

<span data-ttu-id="e7fd9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7fd9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7fd9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json

{
  "displayName": "Family"
}
```
# <a name="c"></a>[<span data-ttu-id="e7fd9-136">C#</span><span class="sxs-lookup"><span data-stu-id="e7fd9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7fd9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7fd9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7fd9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7fd9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7fd9-139">Java</span><span class="sxs-lookup"><span data-stu-id="e7fd9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contactfolder-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e7fd9-140">在请求正文中，提供 [contactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-140">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="e7fd9-141">响应</span><span class="sxs-lookup"><span data-stu-id="e7fd9-141">Response</span></span>

<span data-ttu-id="e7fd9-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-142">Here is an example of the response.</span></span> <span data-ttu-id="e7fd9-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e7fd9-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Family",
  "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy04MDU0LTBkOTFkY2Y5NzE1NAAuAAAAAADESc12GiymT5Zp9IHtHnWZAQA2t6otiDF0TYOkcEEh3vhfAAAGgUC1AAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


