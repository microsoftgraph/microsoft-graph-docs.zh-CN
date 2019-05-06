---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 783a2f4d11c814cc0d0c6f903476a3fa2043cce1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598592"
---
# <a name="list-childfolders"></a><span data-ttu-id="07c4b-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="07c4b-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c4b-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="07c4b-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c4b-107">权限</span><span class="sxs-lookup"><span data-stu-id="07c4b-107">Permissions</span></span>

<span data-ttu-id="07c4b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07c4b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07c4b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="07c4b-110">Permission type</span></span>                        | <span data-ttu-id="07c4b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07c4b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="07c4b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07c4b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="07c4b-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07c4b-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="07c4b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07c4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c4b-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07c4b-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="07c4b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="07c4b-116">Application</span></span>                            | <span data-ttu-id="07c4b-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07c4b-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="07c4b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07c4b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07c4b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="07c4b-119">Optional query parameters</span></span>

<span data-ttu-id="07c4b-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="07c4b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07c4b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="07c4b-121">Request headers</span></span>

| <span data-ttu-id="07c4b-122">名称</span><span class="sxs-lookup"><span data-stu-id="07c4b-122">Name</span></span>          | <span data-ttu-id="07c4b-123">类型</span><span class="sxs-lookup"><span data-stu-id="07c4b-123">Type</span></span>   | <span data-ttu-id="07c4b-124">说明</span><span class="sxs-lookup"><span data-stu-id="07c4b-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="07c4b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07c4b-125">Authorization</span></span> | <span data-ttu-id="07c4b-126">string</span><span class="sxs-lookup"><span data-stu-id="07c4b-126">string</span></span> | <span data-ttu-id="07c4b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07c4b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07c4b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="07c4b-129">Request body</span></span>

<span data-ttu-id="07c4b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="07c4b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07c4b-131">响应</span><span class="sxs-lookup"><span data-stu-id="07c4b-131">Response</span></span>

<span data-ttu-id="07c4b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="07c4b-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07c4b-133">示例</span><span class="sxs-lookup"><span data-stu-id="07c4b-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="07c4b-134">示例 1: 列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="07c4b-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="07c4b-135">请求</span><span class="sxs-lookup"><span data-stu-id="07c4b-135">Request</span></span>

<span data-ttu-id="07c4b-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07c4b-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="07c4b-137">响应</span><span class="sxs-lookup"><span data-stu-id="07c4b-137">Response</span></span>

<span data-ttu-id="07c4b-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="07c4b-138">The following is an example of the response.</span></span>

> <span data-ttu-id="07c4b-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="07c4b-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07c4b-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="07c4b-140">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="07c4b-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="07c4b-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07c4b-142">语言</span><span class="sxs-lookup"><span data-stu-id="07c4b-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07c4b-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="07c4b-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="07c4b-144">示例 2: 列出邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="07c4b-144">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="07c4b-145">请求</span><span class="sxs-lookup"><span data-stu-id="07c4b-145">Request</span></span>

<span data-ttu-id="07c4b-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07c4b-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="07c4b-147">响应</span><span class="sxs-lookup"><span data-stu-id="07c4b-147">Response</span></span>

<span data-ttu-id="07c4b-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="07c4b-148">The following is an example of the response.</span></span>

> <span data-ttu-id="07c4b-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="07c4b-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07c4b-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="07c4b-150">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="07c4b-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="07c4b-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07c4b-152">语言</span><span class="sxs-lookup"><span data-stu-id="07c4b-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07c4b-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="07c4b-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
