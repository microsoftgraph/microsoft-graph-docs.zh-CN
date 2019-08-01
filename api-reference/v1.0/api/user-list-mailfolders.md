---
title: 列出 mailFolder
description: '在已登录用户的根文件夹下获取邮件文件夹集合。 '
author: angelgolfer-ms
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 753123c2cee6ddf670c983f2c56f5e8f53877716
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026871"
---
# <a name="list-mailfolders"></a><span data-ttu-id="96001-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="96001-103">List mailFolders</span></span>

<span data-ttu-id="96001-104">直接在已登录用户的根文件夹下获取邮件文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="96001-104">Get the mail folder collection under the root folder of the signed-in user.</span></span> <span data-ttu-id="96001-105">返回的集合包括直接在根目录下的所有[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="96001-105">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="96001-106">权限</span><span class="sxs-lookup"><span data-stu-id="96001-106">Permissions</span></span>
<span data-ttu-id="96001-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96001-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96001-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96001-109">Permission type</span></span>      | <span data-ttu-id="96001-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96001-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96001-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96001-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96001-112">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96001-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="96001-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96001-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96001-114">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96001-114">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="96001-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="96001-115">Application</span></span> | <span data-ttu-id="96001-116">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96001-116">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="96001-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96001-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96001-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96001-118">Optional query parameters</span></span>
<span data-ttu-id="96001-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96001-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96001-120">请求头</span><span class="sxs-lookup"><span data-stu-id="96001-120">Request headers</span></span>
| <span data-ttu-id="96001-121">标头</span><span class="sxs-lookup"><span data-stu-id="96001-121">Header</span></span>       | <span data-ttu-id="96001-122">值</span><span class="sxs-lookup"><span data-stu-id="96001-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96001-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96001-123">Authorization</span></span>  | <span data-ttu-id="96001-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96001-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="96001-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96001-126">Content-Type</span></span>   | <span data-ttu-id="96001-127">application/json</span><span class="sxs-lookup"><span data-stu-id="96001-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96001-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="96001-128">Request body</span></span>
<span data-ttu-id="96001-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96001-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96001-130">响应</span><span class="sxs-lookup"><span data-stu-id="96001-130">Response</span></span>

<span data-ttu-id="96001-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="96001-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96001-132">示例</span><span class="sxs-lookup"><span data-stu-id="96001-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96001-133">请求</span><span class="sxs-lookup"><span data-stu-id="96001-133">Request</span></span>
<span data-ttu-id="96001-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96001-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96001-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="96001-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96001-136">C#</span><span class="sxs-lookup"><span data-stu-id="96001-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96001-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="96001-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96001-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96001-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96001-139">Java</span><span class="sxs-lookup"><span data-stu-id="96001-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96001-140">响应</span><span class="sxs-lookup"><span data-stu-id="96001-140">Response</span></span>
<span data-ttu-id="96001-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="96001-141">Here is an example of the response.</span></span> 

><span data-ttu-id="96001-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96001-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AQMkADYAAAIBXQAAAA==",
            "displayName": "Archive",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "archive"
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory"
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "deleteditems"
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "drafts"
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "wellKnownName": "inbox"
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "junkemail"
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "outbox"
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "sentitems"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
