---
title: 获取 contactFolder
description: 通过使用联系人文件夹 ID 获取联系人文件夹。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 73f9e8359640efa733371b9dd04ba4be6491937a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047096"
---
# <a name="get-contactfolder"></a><span data-ttu-id="d81b5-103">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="d81b5-103">Get contactFolder</span></span>

<span data-ttu-id="d81b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d81b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d81b5-105">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="d81b5-105">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="d81b5-106">在两种方案中，应用可以获取其他用户的联系人文件夹：</span><span class="sxs-lookup"><span data-stu-id="d81b5-106">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="d81b5-107">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="d81b5-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d81b5-108">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d81b5-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d81b5-109">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="d81b5-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="d81b5-110">权限</span><span class="sxs-lookup"><span data-stu-id="d81b5-110">Permissions</span></span>
<span data-ttu-id="d81b5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d81b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d81b5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d81b5-113">Permission type</span></span>      | <span data-ttu-id="d81b5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d81b5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d81b5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d81b5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d81b5-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d81b5-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d81b5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d81b5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81b5-118">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d81b5-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d81b5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d81b5-119">Application</span></span> | <span data-ttu-id="d81b5-120">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d81b5-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d81b5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d81b5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d81b5-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d81b5-122">Optional query parameters</span></span>
<span data-ttu-id="d81b5-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d81b5-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d81b5-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d81b5-124">Request headers</span></span>
| <span data-ttu-id="d81b5-125">名称</span><span class="sxs-lookup"><span data-stu-id="d81b5-125">Name</span></span>       | <span data-ttu-id="d81b5-126">类型</span><span class="sxs-lookup"><span data-stu-id="d81b5-126">Type</span></span> | <span data-ttu-id="d81b5-127">说明</span><span class="sxs-lookup"><span data-stu-id="d81b5-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d81b5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d81b5-128">Authorization</span></span>  | <span data-ttu-id="d81b5-129">string</span><span class="sxs-lookup"><span data-stu-id="d81b5-129">string</span></span>  | <span data-ttu-id="d81b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d81b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d81b5-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d81b5-132">Request body</span></span>
<span data-ttu-id="d81b5-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d81b5-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d81b5-134">响应</span><span class="sxs-lookup"><span data-stu-id="d81b5-134">Response</span></span>

<span data-ttu-id="d81b5-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d81b5-135">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d81b5-136">示例</span><span class="sxs-lookup"><span data-stu-id="d81b5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d81b5-137">请求</span><span class="sxs-lookup"><span data-stu-id="d81b5-137">Request</span></span>
<span data-ttu-id="d81b5-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d81b5-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d81b5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81b5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="d81b5-140">C#</span><span class="sxs-lookup"><span data-stu-id="d81b5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d81b5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81b5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d81b5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81b5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d81b5-143">Java</span><span class="sxs-lookup"><span data-stu-id="d81b5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d81b5-144">响应</span><span class="sxs-lookup"><span data-stu-id="d81b5-144">Response</span></span>
<span data-ttu-id="d81b5-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d81b5-145">Here is an example of the response.</span></span> <span data-ttu-id="d81b5-146">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d81b5-146">Note: The response object shown here might be shortened for readability.</span></span>
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
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
