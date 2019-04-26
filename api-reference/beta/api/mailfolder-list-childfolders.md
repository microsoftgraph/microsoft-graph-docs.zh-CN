---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 您可以使用`.../me/MailFolders`快捷方式获取顶级 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f551e78cd7c713554b8283542f50c1ee6da05556
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338720"
---
# <a name="list-childfolders"></a><span data-ttu-id="1c01b-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="1c01b-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c01b-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="1c01b-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c01b-107">权限</span><span class="sxs-lookup"><span data-stu-id="1c01b-107">Permissions</span></span>

<span data-ttu-id="1c01b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c01b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c01b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c01b-110">Permission type</span></span>                        | <span data-ttu-id="1c01b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c01b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="1c01b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c01b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c01b-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c01b-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="1c01b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c01b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c01b-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c01b-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="1c01b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c01b-116">Application</span></span>                            | <span data-ttu-id="1c01b-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c01b-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="1c01b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c01b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c01b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1c01b-119">Optional query parameters</span></span>

<span data-ttu-id="1c01b-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1c01b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c01b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c01b-121">Request headers</span></span>

| <span data-ttu-id="1c01b-122">名称</span><span class="sxs-lookup"><span data-stu-id="1c01b-122">Name</span></span>          | <span data-ttu-id="1c01b-123">类型</span><span class="sxs-lookup"><span data-stu-id="1c01b-123">Type</span></span>   | <span data-ttu-id="1c01b-124">说明</span><span class="sxs-lookup"><span data-stu-id="1c01b-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="1c01b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c01b-125">Authorization</span></span> | <span data-ttu-id="1c01b-126">string</span><span class="sxs-lookup"><span data-stu-id="1c01b-126">string</span></span> | <span data-ttu-id="1c01b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c01b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c01b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c01b-129">Request body</span></span>

<span data-ttu-id="1c01b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c01b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c01b-131">响应</span><span class="sxs-lookup"><span data-stu-id="1c01b-131">Response</span></span>

<span data-ttu-id="1c01b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1c01b-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c01b-133">示例</span><span class="sxs-lookup"><span data-stu-id="1c01b-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="1c01b-134">示例 1: 列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="1c01b-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="1c01b-135">请求</span><span class="sxs-lookup"><span data-stu-id="1c01b-135">Request</span></span>

<span data-ttu-id="1c01b-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c01b-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="1c01b-137">响应</span><span class="sxs-lookup"><span data-stu-id="1c01b-137">Response</span></span>

<span data-ttu-id="1c01b-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1c01b-138">The following is an example of the response.</span></span>

> <span data-ttu-id="1c01b-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1c01b-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c01b-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c01b-140">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="1c01b-141">示例 2: 列出邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="1c01b-141">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="1c01b-142">请求</span><span class="sxs-lookup"><span data-stu-id="1c01b-142">Request</span></span>

<span data-ttu-id="1c01b-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c01b-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="1c01b-144">响应</span><span class="sxs-lookup"><span data-stu-id="1c01b-144">Response</span></span>

<span data-ttu-id="1c01b-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1c01b-145">The following is an example of the response.</span></span>

> <span data-ttu-id="1c01b-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1c01b-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c01b-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c01b-147">All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
