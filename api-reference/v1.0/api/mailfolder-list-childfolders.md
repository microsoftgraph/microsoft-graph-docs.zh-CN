---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9080d3ac5cc8cc027386c1bcb740f7f084689abe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055951"
---
# <a name="list-childfolders"></a><span data-ttu-id="c0e44-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="c0e44-104">List childFolders</span></span>

<span data-ttu-id="c0e44-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e44-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0e44-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="c0e44-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0e44-108">权限</span><span class="sxs-lookup"><span data-stu-id="c0e44-108">Permissions</span></span>
<span data-ttu-id="c0e44-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0e44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e44-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0e44-111">Permission type</span></span>      | <span data-ttu-id="c0e44-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0e44-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0e44-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0e44-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c0e44-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0e44-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c0e44-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0e44-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0e44-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0e44-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c0e44-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0e44-117">Application</span></span> | <span data-ttu-id="c0e44-118">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0e44-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0e44-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0e44-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0e44-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0e44-120">Optional query parameters</span></span>
<span data-ttu-id="c0e44-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c0e44-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0e44-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0e44-122">Request headers</span></span>
| <span data-ttu-id="c0e44-123">名称</span><span class="sxs-lookup"><span data-stu-id="c0e44-123">Name</span></span>       | <span data-ttu-id="c0e44-124">类型</span><span class="sxs-lookup"><span data-stu-id="c0e44-124">Type</span></span> | <span data-ttu-id="c0e44-125">说明</span><span class="sxs-lookup"><span data-stu-id="c0e44-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0e44-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0e44-126">Authorization</span></span>  | <span data-ttu-id="c0e44-127">string</span><span class="sxs-lookup"><span data-stu-id="c0e44-127">string</span></span>  | <span data-ttu-id="c0e44-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0e44-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0e44-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0e44-130">Request body</span></span>
<span data-ttu-id="c0e44-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0e44-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e44-132">响应</span><span class="sxs-lookup"><span data-stu-id="c0e44-132">Response</span></span>

<span data-ttu-id="c0e44-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0e44-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0e44-134">示例</span><span class="sxs-lookup"><span data-stu-id="c0e44-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0e44-135">请求</span><span class="sxs-lookup"><span data-stu-id="c0e44-135">Request</span></span>
<span data-ttu-id="c0e44-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0e44-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0e44-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0e44-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="c0e44-138">C#</span><span class="sxs-lookup"><span data-stu-id="c0e44-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0e44-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0e44-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0e44-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0e44-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0e44-141">Java</span><span class="sxs-lookup"><span data-stu-id="c0e44-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0e44-142">响应</span><span class="sxs-lookup"><span data-stu-id="c0e44-142">Response</span></span>
<span data-ttu-id="c0e44-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0e44-143">Here is an example of the response.</span></span> <span data-ttu-id="c0e44-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c0e44-144">Note: The response object shown here might be shortened for readability.</span></span>
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
