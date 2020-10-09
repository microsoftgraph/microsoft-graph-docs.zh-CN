---
title: 获取 mailFolder
description: 检索邮件文件夹对象的属性和关系。
author: svpsiva
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a32f8b0d4ab0d6a8a2de0938350d87cb82a84e55
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401248"
---
# <a name="get-mailfolder"></a><span data-ttu-id="43992-103">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="43992-103">Get mailFolder</span></span>

<span data-ttu-id="43992-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43992-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43992-105">检索邮件文件夹对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43992-105">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="43992-106">在下列两种情况下，应用可获取其他用户的邮件文件夹：</span><span class="sxs-lookup"><span data-stu-id="43992-106">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="43992-107">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="43992-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="43992-108">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="43992-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="43992-109">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="43992-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="43992-110">权限</span><span class="sxs-lookup"><span data-stu-id="43992-110">Permissions</span></span>
<span data-ttu-id="43992-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43992-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43992-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="43992-113">Permission type</span></span>      | <span data-ttu-id="43992-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43992-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43992-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43992-115">Delegated (work or school account)</span></span> | <span data-ttu-id="43992-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43992-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="43992-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43992-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43992-118">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43992-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="43992-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="43992-119">Application</span></span> | <span data-ttu-id="43992-120">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43992-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="43992-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43992-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="43992-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="43992-122">Optional query parameters</span></span>
<span data-ttu-id="43992-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="43992-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="43992-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="43992-124">Request headers</span></span>
| <span data-ttu-id="43992-125">名称</span><span class="sxs-lookup"><span data-stu-id="43992-125">Name</span></span>       | <span data-ttu-id="43992-126">类型</span><span class="sxs-lookup"><span data-stu-id="43992-126">Type</span></span> | <span data-ttu-id="43992-127">说明</span><span class="sxs-lookup"><span data-stu-id="43992-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="43992-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="43992-128">Authorization</span></span>  | <span data-ttu-id="43992-129">string</span><span class="sxs-lookup"><span data-stu-id="43992-129">string</span></span>  | <span data-ttu-id="43992-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43992-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43992-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="43992-132">Request body</span></span>
<span data-ttu-id="43992-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43992-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43992-134">响应</span><span class="sxs-lookup"><span data-stu-id="43992-134">Response</span></span>

<span data-ttu-id="43992-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43992-135">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="43992-136">示例</span><span class="sxs-lookup"><span data-stu-id="43992-136">Examples</span></span>
### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="43992-137">示例 1：获取邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="43992-137">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="43992-138">请求</span><span class="sxs-lookup"><span data-stu-id="43992-138">Request</span></span>

<span data-ttu-id="43992-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="43992-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="43992-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="43992-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="c"></a>[<span data-ttu-id="43992-141">C#</span><span class="sxs-lookup"><span data-stu-id="43992-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43992-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43992-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43992-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43992-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43992-144">Java</span><span class="sxs-lookup"><span data-stu-id="43992-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="43992-145">响应</span><span class="sxs-lookup"><span data-stu-id="43992-145">Response</span></span>

<span data-ttu-id="43992-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="43992-146">The following is an example of the response.</span></span>

> <span data-ttu-id="43992-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="43992-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="43992-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="43992-148">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGVmMDEzM",
  "displayName": "Inbox",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 2,
  "unreadItemCount": 59,
  "totalItemCount": 60
}
```

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="43992-149">示例 2：获取邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="43992-149">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="43992-150">请求</span><span class="sxs-lookup"><span data-stu-id="43992-150">Request</span></span>

<span data-ttu-id="43992-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="43992-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="43992-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="43992-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="c"></a>[<span data-ttu-id="43992-153">C#</span><span class="sxs-lookup"><span data-stu-id="43992-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43992-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43992-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43992-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43992-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43992-156">Java</span><span class="sxs-lookup"><span data-stu-id="43992-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="43992-157">响应</span><span class="sxs-lookup"><span data-stu-id="43992-157">Response</span></span>

<span data-ttu-id="43992-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="43992-158">The following is an example of the response.</span></span>

> <span data-ttu-id="43992-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="43992-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="43992-160">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="43992-160">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->