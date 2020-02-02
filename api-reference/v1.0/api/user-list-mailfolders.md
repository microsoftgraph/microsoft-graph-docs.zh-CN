---
title: 列出 mailFolder
description: '在已登录用户的根文件夹下获取邮件文件夹集合。 '
author: angelgolfer-ms
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 1b802b636ce4a2a7e3b0b4b3c9c3c145842a9670
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652226"
---
# <a name="list-mailfolders"></a><span data-ttu-id="5f57f-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="5f57f-103">List mailFolders</span></span>

<span data-ttu-id="5f57f-104">直接在已登录用户的根文件夹下获取邮件文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="5f57f-104">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="5f57f-105">返回的集合包括直接在根目录下的所有[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="5f57f-105">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f57f-106">权限</span><span class="sxs-lookup"><span data-stu-id="5f57f-106">Permissions</span></span>
<span data-ttu-id="5f57f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f57f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f57f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f57f-109">Permission type</span></span>      | <span data-ttu-id="5f57f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f57f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f57f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f57f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5f57f-112">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f57f-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f57f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f57f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f57f-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f57f-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f57f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f57f-115">Application</span></span> | <span data-ttu-id="5f57f-116">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f57f-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f57f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f57f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5f57f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f57f-118">Optional query parameters</span></span>
<span data-ttu-id="5f57f-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5f57f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5f57f-120">请求头</span><span class="sxs-lookup"><span data-stu-id="5f57f-120">Request headers</span></span>
| <span data-ttu-id="5f57f-121">标头</span><span class="sxs-lookup"><span data-stu-id="5f57f-121">Header</span></span>       | <span data-ttu-id="5f57f-122">值</span><span class="sxs-lookup"><span data-stu-id="5f57f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f57f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f57f-123">Authorization</span></span>  | <span data-ttu-id="5f57f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f57f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5f57f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f57f-126">Content-Type</span></span>   | <span data-ttu-id="5f57f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5f57f-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f57f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f57f-128">Request body</span></span>
<span data-ttu-id="5f57f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f57f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f57f-130">响应</span><span class="sxs-lookup"><span data-stu-id="5f57f-130">Response</span></span>

<span data-ttu-id="5f57f-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f57f-131">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f57f-132">示例</span><span class="sxs-lookup"><span data-stu-id="5f57f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f57f-133">请求</span><span class="sxs-lookup"><span data-stu-id="5f57f-133">Request</span></span>
<span data-ttu-id="5f57f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f57f-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5f57f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f57f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5f57f-136">C#</span><span class="sxs-lookup"><span data-stu-id="5f57f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f57f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f57f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5f57f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f57f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5f57f-139">Java</span><span class="sxs-lookup"><span data-stu-id="5f57f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5f57f-140">响应</span><span class="sxs-lookup"><span data-stu-id="5f57f-140">Response</span></span>
<span data-ttu-id="5f57f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5f57f-141">Here is an example of the response.</span></span>

><span data-ttu-id="5f57f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5f57f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
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
