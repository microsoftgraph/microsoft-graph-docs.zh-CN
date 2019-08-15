---
title: 获取 contactFolder
description: 通过使用联系人文件夹 ID 获取联系人文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5de49776c57789e04dd40723c4eb4f20ac03661
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417968"
---
# <a name="get-contactfolder"></a><span data-ttu-id="5cbe7-103">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="5cbe7-103">Get contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cbe7-104">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-104">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="5cbe7-105">在以下两种情况下, 应用可以获取其他用户的联系人文件夹:</span><span class="sxs-lookup"><span data-stu-id="5cbe7-105">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="5cbe7-106">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="5cbe7-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5cbe7-107">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5cbe7-108">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="5cbe7-109">权限</span><span class="sxs-lookup"><span data-stu-id="5cbe7-109">Permissions</span></span>
<span data-ttu-id="5cbe7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cbe7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cbe7-112">Permission type</span></span>      | <span data-ttu-id="5cbe7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cbe7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cbe7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cbe7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5cbe7-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cbe7-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5cbe7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cbe7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cbe7-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cbe7-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5cbe7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cbe7-118">Application</span></span> | <span data-ttu-id="5cbe7-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cbe7-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cbe7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cbe7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5cbe7-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5cbe7-121">Optional query parameters</span></span>
<span data-ttu-id="5cbe7-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5cbe7-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cbe7-123">Request headers</span></span>
| <span data-ttu-id="5cbe7-124">名称</span><span class="sxs-lookup"><span data-stu-id="5cbe7-124">Name</span></span>       | <span data-ttu-id="5cbe7-125">类型</span><span class="sxs-lookup"><span data-stu-id="5cbe7-125">Type</span></span> | <span data-ttu-id="5cbe7-126">说明</span><span class="sxs-lookup"><span data-stu-id="5cbe7-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5cbe7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cbe7-127">Authorization</span></span>  | <span data-ttu-id="5cbe7-128">string</span><span class="sxs-lookup"><span data-stu-id="5cbe7-128">string</span></span>  | <span data-ttu-id="5cbe7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5cbe7-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cbe7-131">Request body</span></span>
<span data-ttu-id="5cbe7-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cbe7-133">响应</span><span class="sxs-lookup"><span data-stu-id="5cbe7-133">Response</span></span>

<span data-ttu-id="5cbe7-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-134">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5cbe7-135">示例</span><span class="sxs-lookup"><span data-stu-id="5cbe7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cbe7-136">请求</span><span class="sxs-lookup"><span data-stu-id="5cbe7-136">Request</span></span>
<span data-ttu-id="5cbe7-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5cbe7-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5cbe7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5cbe7-139">C#</span><span class="sxs-lookup"><span data-stu-id="5cbe7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5cbe7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cbe7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5cbe7-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="5cbe7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5cbe7-142">响应</span><span class="sxs-lookup"><span data-stu-id="5cbe7-142">Response</span></span>
<span data-ttu-id="5cbe7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cbe7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
