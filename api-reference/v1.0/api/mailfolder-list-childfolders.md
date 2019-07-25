---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 51ce2a020d794a3aeb141ce0bc6196d24d12f2b8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881375"
---
# <a name="list-childfolders"></a><span data-ttu-id="b8ef3-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="b8ef3-104">List childFolders</span></span>

<span data-ttu-id="b8ef3-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8ef3-107">权限</span><span class="sxs-lookup"><span data-stu-id="b8ef3-107">Permissions</span></span>
<span data-ttu-id="b8ef3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8ef3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8ef3-110">Permission type</span></span>      | <span data-ttu-id="b8ef3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8ef3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8ef3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ef3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8ef3-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8ef3-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8ef3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ef3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8ef3-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8ef3-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8ef3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8ef3-116">Application</span></span> | <span data-ttu-id="b8ef3-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8ef3-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8ef3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8ef3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8ef3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b8ef3-119">Optional query parameters</span></span>
<span data-ttu-id="b8ef3-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b8ef3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8ef3-121">Request headers</span></span>
| <span data-ttu-id="b8ef3-122">名称</span><span class="sxs-lookup"><span data-stu-id="b8ef3-122">Name</span></span>       | <span data-ttu-id="b8ef3-123">类型</span><span class="sxs-lookup"><span data-stu-id="b8ef3-123">Type</span></span> | <span data-ttu-id="b8ef3-124">说明</span><span class="sxs-lookup"><span data-stu-id="b8ef3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8ef3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8ef3-125">Authorization</span></span>  | <span data-ttu-id="b8ef3-126">string</span><span class="sxs-lookup"><span data-stu-id="b8ef3-126">string</span></span>  | <span data-ttu-id="b8ef3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8ef3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8ef3-129">Request body</span></span>
<span data-ttu-id="b8ef3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8ef3-131">响应</span><span class="sxs-lookup"><span data-stu-id="b8ef3-131">Response</span></span>

<span data-ttu-id="b8ef3-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8ef3-133">示例</span><span class="sxs-lookup"><span data-stu-id="b8ef3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8ef3-134">请求</span><span class="sxs-lookup"><span data-stu-id="b8ef3-134">Request</span></span>
<span data-ttu-id="b8ef3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8ef3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8ef3-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8ef3-137">C#</span><span class="sxs-lookup"><span data-stu-id="b8ef3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8ef3-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b8ef3-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8ef3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8ef3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8ef3-140">Java</span><span class="sxs-lookup"><span data-stu-id="b8ef3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b8ef3-141">响应</span><span class="sxs-lookup"><span data-stu-id="b8ef3-141">Response</span></span>
<span data-ttu-id="b8ef3-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8ef3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
