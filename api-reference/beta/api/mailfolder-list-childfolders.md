---
title: 列出 childFolder
description: '在指定的文件夹下获取文件夹集合。 您可以使用`.../me/MailFolders`快捷方式来获取顶级 '
ms.openlocfilehash: 826ce59f0f808ee94107a41e76207e83632361ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046215"
---
# <a name="list-childfolders"></a><span data-ttu-id="b7a0d-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="b7a0d-104">List childFolders</span></span>

> <span data-ttu-id="b7a0d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7a0d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7a0d-p103">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-p103">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7a0d-109">权限</span><span class="sxs-lookup"><span data-stu-id="b7a0d-109">Permissions</span></span>
<span data-ttu-id="b7a0d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7a0d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7a0d-112">Permission type</span></span>      | <span data-ttu-id="b7a0d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7a0d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7a0d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7a0d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b7a0d-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a0d-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7a0d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7a0d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7a0d-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a0d-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7a0d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7a0d-118">Application</span></span> | <span data-ttu-id="b7a0d-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7a0d-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7a0d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7a0d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7a0d-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b7a0d-121">Optional query parameters</span></span>
<span data-ttu-id="b7a0d-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7a0d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7a0d-123">Request headers</span></span>
| <span data-ttu-id="b7a0d-124">名称</span><span class="sxs-lookup"><span data-stu-id="b7a0d-124">Name</span></span>       | <span data-ttu-id="b7a0d-125">类型</span><span class="sxs-lookup"><span data-stu-id="b7a0d-125">Type</span></span> | <span data-ttu-id="b7a0d-126">说明</span><span class="sxs-lookup"><span data-stu-id="b7a0d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7a0d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7a0d-127">Authorization</span></span>  | <span data-ttu-id="b7a0d-128">string</span><span class="sxs-lookup"><span data-stu-id="b7a0d-128">string</span></span>  | <span data-ttu-id="b7a0d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7a0d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7a0d-131">Request body</span></span>
<span data-ttu-id="b7a0d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7a0d-133">响应</span><span class="sxs-lookup"><span data-stu-id="b7a0d-133">Response</span></span>
<span data-ttu-id="b7a0d-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-134">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="b7a0d-135">示例 1</span><span class="sxs-lookup"><span data-stu-id="b7a0d-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="b7a0d-136">请求 1</span><span class="sxs-lookup"><span data-stu-id="b7a0d-136">Request 1</span></span>
<span data-ttu-id="b7a0d-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="b7a0d-138">响应 1</span><span class="sxs-lookup"><span data-stu-id="b7a0d-138">Response 1</span></span>
<span data-ttu-id="b7a0d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-139">The following is an example of the response.</span></span>
><span data-ttu-id="b7a0d-140">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b7a0d-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-141">All the properties will be returned from an actual call.</span></span>

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

## <a name="example-2"></a><span data-ttu-id="b7a0d-142">示例 2</span><span class="sxs-lookup"><span data-stu-id="b7a0d-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="b7a0d-143">请求 2</span><span class="sxs-lookup"><span data-stu-id="b7a0d-143">Request 2</span></span>
<span data-ttu-id="b7a0d-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="b7a0d-145">响应 2</span><span class="sxs-lookup"><span data-stu-id="b7a0d-145">Response 2</span></span>
<span data-ttu-id="b7a0d-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-146">The following is an example of the response.</span></span>
><span data-ttu-id="b7a0d-147">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b7a0d-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b7a0d-148">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
