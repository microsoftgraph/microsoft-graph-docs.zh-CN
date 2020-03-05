---
title: 创建 ContactFolder
description: '创建新的 contactFolder 作为指定文件夹的子文件夹。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7f782f32bd08532cad2efb10a101e3f96230bdbe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436872"
---
# <a name="create-contactfolder"></a><span data-ttu-id="2b7fc-103">创建 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="2b7fc-103">Create ContactFolder</span></span>

<span data-ttu-id="2b7fc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2b7fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b7fc-105">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-105">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="2b7fc-106">还可以[在用户的默认联系人文件夹下创建新的 contactFolder](user-post-contactfolders.md)。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-106">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2b7fc-107">权限</span><span class="sxs-lookup"><span data-stu-id="2b7fc-107">Permissions</span></span>
<span data-ttu-id="2b7fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7fc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b7fc-110">Permission type</span></span>      | <span data-ttu-id="2b7fc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b7fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b7fc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b7fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b7fc-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b7fc-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2b7fc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b7fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b7fc-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b7fc-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2b7fc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b7fc-116">Application</span></span> | <span data-ttu-id="2b7fc-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b7fc-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b7fc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b7fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="2b7fc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b7fc-119">Request headers</span></span>
| <span data-ttu-id="2b7fc-120">标头</span><span class="sxs-lookup"><span data-stu-id="2b7fc-120">Header</span></span>       | <span data-ttu-id="2b7fc-121">值</span><span class="sxs-lookup"><span data-stu-id="2b7fc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b7fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b7fc-122">Authorization</span></span>  | <span data-ttu-id="2b7fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b7fc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b7fc-125">Content-Type</span></span>  | <span data-ttu-id="2b7fc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b7fc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b7fc-128">Request body</span></span>
<span data-ttu-id="2b7fc-129">在请求正文中，提供 [ContactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2b7fc-130">响应</span><span class="sxs-lookup"><span data-stu-id="2b7fc-130">Response</span></span>

<span data-ttu-id="2b7fc-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b7fc-132">示例</span><span class="sxs-lookup"><span data-stu-id="2b7fc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b7fc-133">请求</span><span class="sxs-lookup"><span data-stu-id="2b7fc-133">Request</span></span>
<span data-ttu-id="2b7fc-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b7fc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7fc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="2b7fc-136">C#</span><span class="sxs-lookup"><span data-stu-id="2b7fc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b7fc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b7fc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b7fc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b7fc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2b7fc-139">在请求正文中，提供 [contactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-139">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2b7fc-140">响应</span><span class="sxs-lookup"><span data-stu-id="2b7fc-140">Response</span></span>
<span data-ttu-id="2b7fc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
