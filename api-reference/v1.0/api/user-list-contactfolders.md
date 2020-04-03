---
title: List contactFolders
description: 获取已登录用户的默认联系人文件夹中的联系人文件夹集合。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5d1033f9e7034a98631403759b29cc9339f6bfb0
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108849"
---
# <a name="list-contactfolders"></a><span data-ttu-id="e9608-103">List contactFolders</span><span class="sxs-lookup"><span data-stu-id="e9608-103">List contactFolders</span></span>

<span data-ttu-id="e9608-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9608-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9608-105">获取已登录用户的默认联系人文件夹中的联系人文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="e9608-105">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9608-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9608-106">Permissions</span></span>
<span data-ttu-id="e9608-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9608-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9608-109">Permission type</span></span>      | <span data-ttu-id="e9608-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9608-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9608-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9608-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9608-112">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9608-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e9608-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9608-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9608-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9608-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e9608-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9608-115">Application</span></span> | <span data-ttu-id="e9608-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9608-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9608-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9608-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9608-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e9608-118">Optional query parameters</span></span>
<span data-ttu-id="e9608-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e9608-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e9608-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9608-120">Request headers</span></span>
| <span data-ttu-id="e9608-121">标头</span><span class="sxs-lookup"><span data-stu-id="e9608-121">Header</span></span>       | <span data-ttu-id="e9608-122">值</span><span class="sxs-lookup"><span data-stu-id="e9608-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9608-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9608-123">Authorization</span></span>  | <span data-ttu-id="e9608-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9608-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e9608-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9608-126">Content-Type</span></span>   | <span data-ttu-id="e9608-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e9608-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9608-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9608-128">Request body</span></span>
<span data-ttu-id="e9608-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9608-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9608-130">响应</span><span class="sxs-lookup"><span data-stu-id="e9608-130">Response</span></span>

<span data-ttu-id="e9608-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e9608-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9608-132">示例</span><span class="sxs-lookup"><span data-stu-id="e9608-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9608-133">请求</span><span class="sxs-lookup"><span data-stu-id="e9608-133">Request</span></span>
<span data-ttu-id="e9608-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9608-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9608-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9608-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="e9608-136">C#</span><span class="sxs-lookup"><span data-stu-id="e9608-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9608-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9608-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9608-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9608-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9608-139">Java</span><span class="sxs-lookup"><span data-stu-id="e9608-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e9608-140">响应</span><span class="sxs-lookup"><span data-stu-id="e9608-140">Response</span></span>
<span data-ttu-id="e9608-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9608-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
