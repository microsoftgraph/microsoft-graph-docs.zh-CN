---
title: 获取 contactFolder
description: 通过使用联系人文件夹 ID 获取联系人文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 78f70919b00b275572efef6287f3fdf3da7995c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436984"
---
# <a name="get-contactfolder"></a><span data-ttu-id="8669c-103">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="8669c-103">Get contactFolder</span></span>

<span data-ttu-id="8669c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8669c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8669c-105">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="8669c-105">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="8669c-106">在以下两种情况下，应用可以获取其他用户的联系人文件夹：</span><span class="sxs-lookup"><span data-stu-id="8669c-106">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="8669c-107">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="8669c-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8669c-108">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="8669c-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8669c-109">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="8669c-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="8669c-110">权限</span><span class="sxs-lookup"><span data-stu-id="8669c-110">Permissions</span></span>
<span data-ttu-id="8669c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8669c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8669c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="8669c-113">Permission type</span></span>      | <span data-ttu-id="8669c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8669c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8669c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8669c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8669c-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8669c-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8669c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8669c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8669c-118">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8669c-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8669c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8669c-119">Application</span></span> | <span data-ttu-id="8669c-120">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8669c-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8669c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8669c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8669c-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8669c-122">Optional query parameters</span></span>
<span data-ttu-id="8669c-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8669c-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8669c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="8669c-124">Request headers</span></span>
| <span data-ttu-id="8669c-125">名称</span><span class="sxs-lookup"><span data-stu-id="8669c-125">Name</span></span>       | <span data-ttu-id="8669c-126">类型</span><span class="sxs-lookup"><span data-stu-id="8669c-126">Type</span></span> | <span data-ttu-id="8669c-127">说明</span><span class="sxs-lookup"><span data-stu-id="8669c-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8669c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8669c-128">Authorization</span></span>  | <span data-ttu-id="8669c-129">string</span><span class="sxs-lookup"><span data-stu-id="8669c-129">string</span></span>  | <span data-ttu-id="8669c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8669c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8669c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="8669c-132">Request body</span></span>
<span data-ttu-id="8669c-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8669c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8669c-134">响应</span><span class="sxs-lookup"><span data-stu-id="8669c-134">Response</span></span>

<span data-ttu-id="8669c-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8669c-135">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8669c-136">示例</span><span class="sxs-lookup"><span data-stu-id="8669c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8669c-137">请求</span><span class="sxs-lookup"><span data-stu-id="8669c-137">Request</span></span>
<span data-ttu-id="8669c-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8669c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8669c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8669c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="8669c-140">C#</span><span class="sxs-lookup"><span data-stu-id="8669c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8669c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8669c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8669c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8669c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8669c-143">响应</span><span class="sxs-lookup"><span data-stu-id="8669c-143">Response</span></span>
<span data-ttu-id="8669c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8669c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
