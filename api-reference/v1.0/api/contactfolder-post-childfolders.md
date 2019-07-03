---
title: 创建 ContactFolder
description: '创建新的 contactFolder 作为指定文件夹的子文件夹。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 61bf132688fbe0b7b8580c4fdb1f637b26ef7cb9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443019"
---
# <a name="create-contactfolder"></a><span data-ttu-id="bac8a-103">创建 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="bac8a-103">Create ContactFolder</span></span>

<span data-ttu-id="bac8a-104">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="bac8a-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="bac8a-105">还可以[在用户的默认联系人文件夹下创建新的 contactFolder](user-post-contactfolders.md)。</span><span class="sxs-lookup"><span data-stu-id="bac8a-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bac8a-106">权限</span><span class="sxs-lookup"><span data-stu-id="bac8a-106">Permissions</span></span>
<span data-ttu-id="bac8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bac8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bac8a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bac8a-109">Permission type</span></span>      | <span data-ttu-id="bac8a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bac8a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bac8a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bac8a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bac8a-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bac8a-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bac8a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bac8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bac8a-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bac8a-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bac8a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bac8a-115">Application</span></span> | <span data-ttu-id="bac8a-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bac8a-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bac8a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bac8a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="bac8a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bac8a-118">Request headers</span></span>
| <span data-ttu-id="bac8a-119">标头</span><span class="sxs-lookup"><span data-stu-id="bac8a-119">Header</span></span>       | <span data-ttu-id="bac8a-120">值</span><span class="sxs-lookup"><span data-stu-id="bac8a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bac8a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bac8a-121">Authorization</span></span>  | <span data-ttu-id="bac8a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bac8a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bac8a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bac8a-124">Content-Type</span></span>  | <span data-ttu-id="bac8a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bac8a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bac8a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bac8a-127">Request body</span></span>
<span data-ttu-id="bac8a-128">在请求正文中，提供 [ContactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bac8a-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bac8a-129">响应</span><span class="sxs-lookup"><span data-stu-id="bac8a-129">Response</span></span>

<span data-ttu-id="bac8a-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bac8a-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bac8a-131">示例</span><span class="sxs-lookup"><span data-stu-id="bac8a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bac8a-132">请求</span><span class="sxs-lookup"><span data-stu-id="bac8a-132">Request</span></span>
<span data-ttu-id="bac8a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bac8a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bac8a-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bac8a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bac8a-135">C#</span><span class="sxs-lookup"><span data-stu-id="bac8a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bac8a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="bac8a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bac8a-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="bac8a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bac8a-138">在请求正文中，提供 [contactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bac8a-138">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bac8a-139">响应</span><span class="sxs-lookup"><span data-stu-id="bac8a-139">Response</span></span>
<span data-ttu-id="bac8a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bac8a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
