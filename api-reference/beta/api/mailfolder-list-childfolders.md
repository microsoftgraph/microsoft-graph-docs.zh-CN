---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 803a04c858b6ce003ee92b0b0cec32536e9fdb53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984055"
---
# <a name="list-childfolders"></a><span data-ttu-id="8e879-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="8e879-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e879-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="8e879-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e879-107">权限</span><span class="sxs-lookup"><span data-stu-id="8e879-107">Permissions</span></span>

<span data-ttu-id="8e879-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e879-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e879-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e879-110">Permission type</span></span>                        | <span data-ttu-id="8e879-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e879-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="8e879-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e879-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e879-113">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="8e879-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="8e879-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e879-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e879-115">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="8e879-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="8e879-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e879-116">Application</span></span>                            | <span data-ttu-id="8e879-117">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="8e879-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="8e879-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e879-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e879-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8e879-119">Optional query parameters</span></span>

<span data-ttu-id="8e879-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8e879-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e879-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e879-121">Request headers</span></span>

| <span data-ttu-id="8e879-122">名称</span><span class="sxs-lookup"><span data-stu-id="8e879-122">Name</span></span>          | <span data-ttu-id="8e879-123">类型</span><span class="sxs-lookup"><span data-stu-id="8e879-123">Type</span></span>   | <span data-ttu-id="8e879-124">说明</span><span class="sxs-lookup"><span data-stu-id="8e879-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="8e879-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e879-125">Authorization</span></span> | <span data-ttu-id="8e879-126">string</span><span class="sxs-lookup"><span data-stu-id="8e879-126">string</span></span> | <span data-ttu-id="8e879-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e879-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e879-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e879-129">Request body</span></span>

<span data-ttu-id="8e879-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e879-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e879-131">响应</span><span class="sxs-lookup"><span data-stu-id="8e879-131">Response</span></span>

<span data-ttu-id="8e879-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="8e879-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e879-133">示例</span><span class="sxs-lookup"><span data-stu-id="8e879-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="8e879-134">示例 1: 列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="8e879-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="8e879-135">请求</span><span class="sxs-lookup"><span data-stu-id="8e879-135">Request</span></span>

<span data-ttu-id="8e879-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e879-136">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e879-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8e879-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e879-138">C#</span><span class="sxs-lookup"><span data-stu-id="8e879-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e879-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="8e879-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e879-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="8e879-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e879-141">Java</span><span class="sxs-lookup"><span data-stu-id="8e879-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="8e879-142">响应</span><span class="sxs-lookup"><span data-stu-id="8e879-142">Response</span></span>

<span data-ttu-id="8e879-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e879-143">The following is an example of the response.</span></span>

> <span data-ttu-id="8e879-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e879-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e879-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e879-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders"
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="8e879-146">示例 2: 列出邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="8e879-146">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="8e879-147">请求</span><span class="sxs-lookup"><span data-stu-id="8e879-147">Request</span></span>

<span data-ttu-id="8e879-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e879-148">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e879-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8e879-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e879-150">C#</span><span class="sxs-lookup"><span data-stu-id="8e879-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e879-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="8e879-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e879-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="8e879-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e879-153">Java</span><span class="sxs-lookup"><span data-stu-id="8e879-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-childfolders-of-searchfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e879-154">响应</span><span class="sxs-lookup"><span data-stu-id="8e879-154">Response</span></span>

<span data-ttu-id="8e879-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e879-155">The following is an example of the response.</span></span>

> <span data-ttu-id="8e879-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e879-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e879-157">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e879-157">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMz",
      "displayName": "Get MyAnalytics",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 6,
      "totalItemCount": 6,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'MyAnalytics')"
    },
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMy",
      "displayName": "Action Required",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 4,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
