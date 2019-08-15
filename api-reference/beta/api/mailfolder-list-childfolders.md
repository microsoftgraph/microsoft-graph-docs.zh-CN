---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1c3151174276ad4bcb9fdfb89550609aebaba1e5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415293"
---
# <a name="list-childfolders"></a><span data-ttu-id="82627-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="82627-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82627-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="82627-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="82627-107">权限</span><span class="sxs-lookup"><span data-stu-id="82627-107">Permissions</span></span>

<span data-ttu-id="82627-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82627-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82627-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82627-110">Permission type</span></span>                        | <span data-ttu-id="82627-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82627-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="82627-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82627-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="82627-113">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="82627-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="82627-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82627-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82627-115">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="82627-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="82627-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82627-116">Application</span></span>                            | <span data-ttu-id="82627-117">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="82627-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="82627-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82627-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82627-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82627-119">Optional query parameters</span></span>

<span data-ttu-id="82627-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82627-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82627-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="82627-121">Request headers</span></span>

| <span data-ttu-id="82627-122">名称</span><span class="sxs-lookup"><span data-stu-id="82627-122">Name</span></span>          | <span data-ttu-id="82627-123">类型</span><span class="sxs-lookup"><span data-stu-id="82627-123">Type</span></span>   | <span data-ttu-id="82627-124">说明</span><span class="sxs-lookup"><span data-stu-id="82627-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="82627-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="82627-125">Authorization</span></span> | <span data-ttu-id="82627-126">string</span><span class="sxs-lookup"><span data-stu-id="82627-126">string</span></span> | <span data-ttu-id="82627-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82627-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82627-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="82627-129">Request body</span></span>

<span data-ttu-id="82627-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82627-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82627-131">响应</span><span class="sxs-lookup"><span data-stu-id="82627-131">Response</span></span>

<span data-ttu-id="82627-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="82627-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82627-133">示例</span><span class="sxs-lookup"><span data-stu-id="82627-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="82627-134">示例 1: 列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="82627-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="82627-135">请求</span><span class="sxs-lookup"><span data-stu-id="82627-135">Request</span></span>

<span data-ttu-id="82627-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="82627-136">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="82627-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="82627-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82627-138">C#</span><span class="sxs-lookup"><span data-stu-id="82627-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82627-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82627-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82627-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="82627-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="82627-141">响应</span><span class="sxs-lookup"><span data-stu-id="82627-141">Response</span></span>

<span data-ttu-id="82627-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="82627-142">The following is an example of the response.</span></span>

> <span data-ttu-id="82627-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82627-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="82627-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="82627-144">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="82627-145">示例 2: 列出邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="82627-145">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="82627-146">请求</span><span class="sxs-lookup"><span data-stu-id="82627-146">Request</span></span>

<span data-ttu-id="82627-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="82627-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="82627-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="82627-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82627-149">C#</span><span class="sxs-lookup"><span data-stu-id="82627-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82627-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82627-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82627-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="82627-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="82627-152">响应</span><span class="sxs-lookup"><span data-stu-id="82627-152">Response</span></span>

<span data-ttu-id="82627-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="82627-153">The following is an example of the response.</span></span>

> <span data-ttu-id="82627-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82627-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="82627-155">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="82627-155">All the properties will be returned from an actual call.</span></span>

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
