---
title: 获取 mailFolder
description: 检索邮件文件夹对象的属性和关系。
author: angelgolfer-ms
ms.openlocfilehash: e1394c6bf97a3c5d65bda0ee7b8f29d8a29643bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357811"
---
# <a name="get-mailfolder"></a><span data-ttu-id="09262-103">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="09262-103">Get mailFolder</span></span>

> <span data-ttu-id="09262-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="09262-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09262-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09262-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09262-106">检索邮件文件夹对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09262-106">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="09262-107">有两种方案相关应用程序可以在哪里找到另一个用户的邮件文件夹：</span><span class="sxs-lookup"><span data-stu-id="09262-107">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="09262-108">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="09262-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="09262-109">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享邮件文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="09262-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="09262-110">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="09262-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="09262-111">权限</span><span class="sxs-lookup"><span data-stu-id="09262-111">Permissions</span></span>
<span data-ttu-id="09262-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09262-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09262-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="09262-114">Permission type</span></span>      | <span data-ttu-id="09262-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09262-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09262-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09262-116">Delegated (work or school account)</span></span> | <span data-ttu-id="09262-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09262-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="09262-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09262-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09262-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09262-119">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="09262-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="09262-120">Application</span></span> | <span data-ttu-id="09262-121">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09262-121">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="09262-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09262-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09262-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="09262-123">Optional query parameters</span></span>
<span data-ttu-id="09262-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="09262-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09262-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="09262-125">Request headers</span></span>
| <span data-ttu-id="09262-126">Name</span><span class="sxs-lookup"><span data-stu-id="09262-126">Name</span></span>       | <span data-ttu-id="09262-127">类型</span><span class="sxs-lookup"><span data-stu-id="09262-127">Type</span></span> | <span data-ttu-id="09262-128">说明</span><span class="sxs-lookup"><span data-stu-id="09262-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="09262-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="09262-129">Authorization</span></span>  | <span data-ttu-id="09262-130">string</span><span class="sxs-lookup"><span data-stu-id="09262-130">string</span></span>  | <span data-ttu-id="09262-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09262-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09262-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="09262-133">Request body</span></span>
<span data-ttu-id="09262-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09262-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09262-135">响应</span><span class="sxs-lookup"><span data-stu-id="09262-135">Response</span></span>
<span data-ttu-id="09262-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09262-136">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="09262-137">示例 1</span><span class="sxs-lookup"><span data-stu-id="09262-137">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="09262-138">请求 1</span><span class="sxs-lookup"><span data-stu-id="09262-138">Request 1</span></span>
<span data-ttu-id="09262-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09262-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="09262-140">响应 1</span><span class="sxs-lookup"><span data-stu-id="09262-140">Response 1</span></span>
<span data-ttu-id="09262-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09262-141">The following is an example of the response.</span></span>
 ><span data-ttu-id="09262-142">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="09262-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09262-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09262-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

## <a name="example-2"></a><span data-ttu-id="09262-144">示例 2</span><span class="sxs-lookup"><span data-stu-id="09262-144">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="09262-145">请求 2</span><span class="sxs-lookup"><span data-stu-id="09262-145">Request 2</span></span>
<span data-ttu-id="09262-146">下面是一个搜索文件夹的示例，该请求。</span><span class="sxs-lookup"><span data-stu-id="09262-146">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="09262-147">响应 2</span><span class="sxs-lookup"><span data-stu-id="09262-147">Response 2</span></span>
<span data-ttu-id="09262-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09262-148">The following is an example of the response.</span></span>
 ><span data-ttu-id="09262-149">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="09262-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09262-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09262-150">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
