---
title: 列出 mailFolder
description: '在已登录用户的根文件夹下获取邮件文件夹集合。 '
author: svpsiva
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: c653f79888edc964cee2151aaa32d7d913053cb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091962"
---
# <a name="list-mailfolders"></a><span data-ttu-id="646c8-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="646c8-103">List mailFolders</span></span>

<span data-ttu-id="646c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="646c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="646c8-105">直接在已登录用户的根文件夹下获取邮件文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="646c8-105">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="646c8-106">返回的集合包括直接在根目录下的所有[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="646c8-106">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="646c8-107">权限</span><span class="sxs-lookup"><span data-stu-id="646c8-107">Permissions</span></span>
<span data-ttu-id="646c8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="646c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="646c8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="646c8-110">Permission type</span></span>      | <span data-ttu-id="646c8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="646c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="646c8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="646c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="646c8-113">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="646c8-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="646c8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="646c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="646c8-115">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="646c8-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="646c8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="646c8-116">Application</span></span> | <span data-ttu-id="646c8-117">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="646c8-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="646c8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="646c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="646c8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="646c8-119">Optional query parameters</span></span>
<span data-ttu-id="646c8-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="646c8-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="646c8-121">请求头</span><span class="sxs-lookup"><span data-stu-id="646c8-121">Request headers</span></span>
| <span data-ttu-id="646c8-122">标头</span><span class="sxs-lookup"><span data-stu-id="646c8-122">Header</span></span>       | <span data-ttu-id="646c8-123">值</span><span class="sxs-lookup"><span data-stu-id="646c8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="646c8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="646c8-124">Authorization</span></span>  | <span data-ttu-id="646c8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="646c8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="646c8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="646c8-127">Content-Type</span></span>   | <span data-ttu-id="646c8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="646c8-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="646c8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="646c8-129">Request body</span></span>
<span data-ttu-id="646c8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="646c8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="646c8-131">响应</span><span class="sxs-lookup"><span data-stu-id="646c8-131">Response</span></span>

<span data-ttu-id="646c8-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="646c8-132">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="646c8-133">示例</span><span class="sxs-lookup"><span data-stu-id="646c8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="646c8-134">请求</span><span class="sxs-lookup"><span data-stu-id="646c8-134">Request</span></span>
<span data-ttu-id="646c8-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="646c8-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="646c8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="646c8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="646c8-137">C#</span><span class="sxs-lookup"><span data-stu-id="646c8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="646c8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="646c8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="646c8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="646c8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="646c8-140">Java</span><span class="sxs-lookup"><span data-stu-id="646c8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="646c8-141">响应</span><span class="sxs-lookup"><span data-stu-id="646c8-141">Response</span></span>
<span data-ttu-id="646c8-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="646c8-142">Here is an example of the response.</span></span>

><span data-ttu-id="646c8-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="646c8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

