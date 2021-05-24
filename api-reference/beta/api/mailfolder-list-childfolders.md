---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 59d5fe5bfc52f20e38188f597616947a75b7c000
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629530"
---
# <a name="list-childfolders"></a><span data-ttu-id="c1a23-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="c1a23-104">List childFolders</span></span>

<span data-ttu-id="c1a23-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a23-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a23-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="c1a23-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

<span data-ttu-id="c1a23-108">默认情况下，此操作不会返回隐藏文件夹。</span><span class="sxs-lookup"><span data-stu-id="c1a23-108">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="c1a23-109">使用查询参数 _includeHiddenFolders_ 将其包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="c1a23-109">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a23-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="c1a23-110">Permissions</span></span>

<span data-ttu-id="c1a23-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1a23-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1a23-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1a23-113">Permission type</span></span>                        | <span data-ttu-id="c1a23-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1a23-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="c1a23-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a23-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1a23-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1a23-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="c1a23-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a23-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1a23-118">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1a23-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="c1a23-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1a23-119">Application</span></span>                            | <span data-ttu-id="c1a23-120">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1a23-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="c1a23-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1a23-121">HTTP request</span></span>

<span data-ttu-id="c1a23-122">若要获取指定文件夹下的所有子文件夹（隐藏文件夹除外）：</span><span class="sxs-lookup"><span data-stu-id="c1a23-122">To get all the child folders under the specified folder, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c1a23-123">若要在 _响应_ 中包括隐藏的子文件夹：</span><span class="sxs-lookup"><span data-stu-id="c1a23-123">To include _hidden_ child folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1a23-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1a23-124">Optional query parameters</span></span>
<span data-ttu-id="c1a23-125">若要返回所有 childFolders 的列表，包括隐藏的子文件夹 (其 **isHidden** 属性为 true) ，在请求 URL 中，将查询参数指定为 ，如 HTTP 请求部分 `includeHiddenFolders` `true` 所示 [](#http-request)。</span><span class="sxs-lookup"><span data-stu-id="c1a23-125">To return a list of all childFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="c1a23-126">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1a23-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1a23-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1a23-127">Request headers</span></span>

| <span data-ttu-id="c1a23-128">名称</span><span class="sxs-lookup"><span data-stu-id="c1a23-128">Name</span></span>          | <span data-ttu-id="c1a23-129">类型</span><span class="sxs-lookup"><span data-stu-id="c1a23-129">Type</span></span>   | <span data-ttu-id="c1a23-130">说明</span><span class="sxs-lookup"><span data-stu-id="c1a23-130">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="c1a23-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1a23-131">Authorization</span></span> | <span data-ttu-id="c1a23-132">string</span><span class="sxs-lookup"><span data-stu-id="c1a23-132">string</span></span> | <span data-ttu-id="c1a23-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1a23-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1a23-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1a23-135">Request body</span></span>

<span data-ttu-id="c1a23-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1a23-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1a23-137">响应</span><span class="sxs-lookup"><span data-stu-id="c1a23-137">Response</span></span>

<span data-ttu-id="c1a23-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1a23-138">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1a23-139">示例</span><span class="sxs-lookup"><span data-stu-id="c1a23-139">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="c1a23-140">示例 1：列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="c1a23-140">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="c1a23-141">请求</span><span class="sxs-lookup"><span data-stu-id="c1a23-141">Request</span></span>

<span data-ttu-id="c1a23-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1a23-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1a23-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a23-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="c"></a>[<span data-ttu-id="c1a23-144">C#</span><span class="sxs-lookup"><span data-stu-id="c1a23-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1a23-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a23-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1a23-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1a23-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1a23-147">Java</span><span class="sxs-lookup"><span data-stu-id="c1a23-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c1a23-148">响应</span><span class="sxs-lookup"><span data-stu-id="c1a23-148">Response</span></span>

<span data-ttu-id="c1a23-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1a23-149">The following is an example of the response.</span></span>

> <span data-ttu-id="c1a23-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1a23-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders",
      "isHidden": false
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="c1a23-151">示例 2：列出邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="c1a23-151">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="c1a23-152">请求</span><span class="sxs-lookup"><span data-stu-id="c1a23-152">Request</span></span>

<span data-ttu-id="c1a23-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1a23-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1a23-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a23-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="c"></a>[<span data-ttu-id="c1a23-155">C#</span><span class="sxs-lookup"><span data-stu-id="c1a23-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1a23-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a23-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1a23-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1a23-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1a23-158">Java</span><span class="sxs-lookup"><span data-stu-id="c1a23-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-childfolders-of-searchfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1a23-159">响应</span><span class="sxs-lookup"><span data-stu-id="c1a23-159">Response</span></span>

<span data-ttu-id="c1a23-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1a23-160">The following is an example of the response.</span></span>

> <span data-ttu-id="c1a23-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1a23-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "isHidden": false,
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
      "isHidden": false,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

### <a name="example-3-include-hidden-child-folders-under-a-specified-mail-folder"></a><span data-ttu-id="c1a23-162">示例 3：在指定的邮件文件夹下包含隐藏的子文件夹</span><span class="sxs-lookup"><span data-stu-id="c1a23-162">Example 3: Include hidden child folders under a specified mail folder</span></span>

<span data-ttu-id="c1a23-163">下一个示例使用 query 参数获取指定邮件文件夹下的子文件夹列表，包括 `includeHiddenFolders` 隐藏邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="c1a23-163">The next example uses the `includeHiddenFolders` query parameter to get a list of child folders under a specified mail folder including hidden mail folders.</span></span> <span data-ttu-id="c1a23-164">该响应包括将 **isHidden** 设置为 true 的"待筛选邮件"文件夹。</span><span class="sxs-lookup"><span data-stu-id="c1a23-164">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="c1a23-165">请求</span><span class="sxs-lookup"><span data-stu-id="c1a23-165">Request</span></span>

<span data-ttu-id="c1a23-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1a23-166">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "mailfolder_get_hiddenchildfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders?includeHiddenFolders=true
```

#### <a name="response"></a><span data-ttu-id="c1a23-167">响应</span><span class="sxs-lookup"><span data-stu-id="c1a23-167">Response</span></span>

<span data-ttu-id="c1a23-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1a23-168">The following is an example of the response.</span></span>

> <span data-ttu-id="c1a23-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1a23-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Clutters",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null,
      "isHidden": true
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders",
      "isHidden": false
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


