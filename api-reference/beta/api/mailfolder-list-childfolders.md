---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 275f7bcd771db43f5d091848d9be8c50c6ddb124
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417728"
---
# <a name="list-childfolders"></a><span data-ttu-id="b846e-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="b846e-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b846e-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="b846e-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b846e-107">权限</span><span class="sxs-lookup"><span data-stu-id="b846e-107">Permissions</span></span>

<span data-ttu-id="b846e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b846e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b846e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b846e-110">Permission type</span></span>                        | <span data-ttu-id="b846e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b846e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="b846e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b846e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b846e-113">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="b846e-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b846e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b846e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b846e-115">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="b846e-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b846e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b846e-116">Application</span></span>                            | <span data-ttu-id="b846e-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b846e-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="b846e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b846e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b846e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b846e-119">Optional query parameters</span></span>

<span data-ttu-id="b846e-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b846e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b846e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b846e-121">Request headers</span></span>

| <span data-ttu-id="b846e-122">名称</span><span class="sxs-lookup"><span data-stu-id="b846e-122">Name</span></span>          | <span data-ttu-id="b846e-123">类型</span><span class="sxs-lookup"><span data-stu-id="b846e-123">Type</span></span>   | <span data-ttu-id="b846e-124">说明</span><span class="sxs-lookup"><span data-stu-id="b846e-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="b846e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b846e-125">Authorization</span></span> | <span data-ttu-id="b846e-126">string</span><span class="sxs-lookup"><span data-stu-id="b846e-126">string</span></span> | <span data-ttu-id="b846e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b846e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b846e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b846e-129">Request body</span></span>

<span data-ttu-id="b846e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b846e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b846e-131">响应</span><span class="sxs-lookup"><span data-stu-id="b846e-131">Response</span></span>

<span data-ttu-id="b846e-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b846e-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b846e-133">示例</span><span class="sxs-lookup"><span data-stu-id="b846e-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="b846e-134">示例 1: 列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="b846e-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="b846e-135">请求</span><span class="sxs-lookup"><span data-stu-id="b846e-135">Request</span></span>

<span data-ttu-id="b846e-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b846e-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="b846e-137">响应</span><span class="sxs-lookup"><span data-stu-id="b846e-137">Response</span></span>

<span data-ttu-id="b846e-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b846e-138">The following is an example of the response.</span></span>

> <span data-ttu-id="b846e-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b846e-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b846e-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b846e-140">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b846e-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b846e-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b846e-142">C#</span><span class="sxs-lookup"><span data-stu-id="b846e-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b846e-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="b846e-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b846e-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="b846e-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="b846e-145">示例 2: 列出邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="b846e-145">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="b846e-146">请求</span><span class="sxs-lookup"><span data-stu-id="b846e-146">Request</span></span>

<span data-ttu-id="b846e-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b846e-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="b846e-148">响应</span><span class="sxs-lookup"><span data-stu-id="b846e-148">Response</span></span>

<span data-ttu-id="b846e-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b846e-149">The following is an example of the response.</span></span>

> <span data-ttu-id="b846e-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b846e-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b846e-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b846e-151">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b846e-152">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b846e-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b846e-153">C#</span><span class="sxs-lookup"><span data-stu-id="b846e-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b846e-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="b846e-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b846e-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="b846e-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
