---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 412f38352dadbd42810d4b153a788912c95e04d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053627"
---
# <a name="list-childfolders"></a><span data-ttu-id="b4548-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="b4548-104">List childFolders</span></span>

<span data-ttu-id="b4548-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4548-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4548-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="b4548-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4548-108">权限</span><span class="sxs-lookup"><span data-stu-id="b4548-108">Permissions</span></span>

<span data-ttu-id="b4548-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4548-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4548-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4548-111">Permission type</span></span>                        | <span data-ttu-id="b4548-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4548-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="b4548-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4548-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4548-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4548-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b4548-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4548-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4548-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4548-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b4548-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4548-117">Application</span></span>                            | <span data-ttu-id="b4548-118">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4548-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="b4548-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4548-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4548-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b4548-120">Optional query parameters</span></span>

<span data-ttu-id="b4548-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4548-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4548-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4548-122">Request headers</span></span>

| <span data-ttu-id="b4548-123">名称</span><span class="sxs-lookup"><span data-stu-id="b4548-123">Name</span></span>          | <span data-ttu-id="b4548-124">类型</span><span class="sxs-lookup"><span data-stu-id="b4548-124">Type</span></span>   | <span data-ttu-id="b4548-125">说明</span><span class="sxs-lookup"><span data-stu-id="b4548-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="b4548-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4548-126">Authorization</span></span> | <span data-ttu-id="b4548-127">string</span><span class="sxs-lookup"><span data-stu-id="b4548-127">string</span></span> | <span data-ttu-id="b4548-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4548-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4548-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4548-130">Request body</span></span>

<span data-ttu-id="b4548-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4548-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4548-132">响应</span><span class="sxs-lookup"><span data-stu-id="b4548-132">Response</span></span>

<span data-ttu-id="b4548-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b4548-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4548-134">示例</span><span class="sxs-lookup"><span data-stu-id="b4548-134">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="b4548-135">示例1：列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="b4548-135">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="b4548-136">请求</span><span class="sxs-lookup"><span data-stu-id="b4548-136">Request</span></span>

<span data-ttu-id="b4548-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4548-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4548-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4548-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="c"></a>[<span data-ttu-id="b4548-139">C#</span><span class="sxs-lookup"><span data-stu-id="b4548-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4548-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4548-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4548-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4548-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="b4548-142">响应</span><span class="sxs-lookup"><span data-stu-id="b4548-142">Response</span></span>

<span data-ttu-id="b4548-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4548-143">The following is an example of the response.</span></span>

> <span data-ttu-id="b4548-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4548-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4548-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4548-145">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="b4548-146">示例2：列出邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="b4548-146">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="b4548-147">请求</span><span class="sxs-lookup"><span data-stu-id="b4548-147">Request</span></span>

<span data-ttu-id="b4548-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4548-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4548-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4548-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="c"></a>[<span data-ttu-id="b4548-150">C#</span><span class="sxs-lookup"><span data-stu-id="b4548-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4548-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4548-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4548-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4548-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4548-153">响应</span><span class="sxs-lookup"><span data-stu-id="b4548-153">Response</span></span>

<span data-ttu-id="b4548-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4548-154">The following is an example of the response.</span></span>

> <span data-ttu-id="b4548-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4548-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4548-156">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4548-156">All the properties will be returned from an actual call.</span></span>

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


