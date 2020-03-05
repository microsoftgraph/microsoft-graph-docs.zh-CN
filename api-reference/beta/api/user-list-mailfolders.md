---
title: 列出 mailFolder
description: 获取已登录用户的邮箱中的所有邮件文件夹。
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 34146d3fab0e4f13e2d9c41e738c57a7e8bdd1cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451824"
---
# <a name="list-mailfolders"></a><span data-ttu-id="dadcf-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="dadcf-103">List mailFolders</span></span>

<span data-ttu-id="dadcf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dadcf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dadcf-105">获取登录用户的邮箱中的所有邮件文件夹，包括任何[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="dadcf-105">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dadcf-106">权限</span><span class="sxs-lookup"><span data-stu-id="dadcf-106">Permissions</span></span>
<span data-ttu-id="dadcf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dadcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dadcf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dadcf-109">Permission type</span></span>      | <span data-ttu-id="dadcf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dadcf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dadcf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dadcf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dadcf-112">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dadcf-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dadcf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dadcf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dadcf-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dadcf-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dadcf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dadcf-115">Application</span></span> | <span data-ttu-id="dadcf-116">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dadcf-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dadcf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dadcf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dadcf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dadcf-118">Optional query parameters</span></span>
<span data-ttu-id="dadcf-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dadcf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dadcf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dadcf-120">Request headers</span></span>
| <span data-ttu-id="dadcf-121">标头</span><span class="sxs-lookup"><span data-stu-id="dadcf-121">Header</span></span>       | <span data-ttu-id="dadcf-122">值</span><span class="sxs-lookup"><span data-stu-id="dadcf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dadcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dadcf-123">Authorization</span></span>  | <span data-ttu-id="dadcf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dadcf-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dadcf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dadcf-126">Content-Type</span></span>   | <span data-ttu-id="dadcf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dadcf-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dadcf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="dadcf-128">Request body</span></span>
<span data-ttu-id="dadcf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dadcf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dadcf-130">响应</span><span class="sxs-lookup"><span data-stu-id="dadcf-130">Response</span></span>

<span data-ttu-id="dadcf-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dadcf-131">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dadcf-132">示例</span><span class="sxs-lookup"><span data-stu-id="dadcf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dadcf-133">请求</span><span class="sxs-lookup"><span data-stu-id="dadcf-133">Request</span></span>
<span data-ttu-id="dadcf-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dadcf-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dadcf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dadcf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="dadcf-136">C#</span><span class="sxs-lookup"><span data-stu-id="dadcf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dadcf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dadcf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dadcf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dadcf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dadcf-139">响应</span><span class="sxs-lookup"><span data-stu-id="dadcf-139">Response</span></span>
<span data-ttu-id="dadcf-140">下面是一个响应示例，其中包含一个作为 "收件箱" 下的子文件夹的**mailSearchFolder** 。</span><span class="sxs-lookup"><span data-stu-id="dadcf-140">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="dadcf-141">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dadcf-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dadcf-142">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dadcf-142">All of the properties will be returned from an actual call.</span></span>
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
            "@odata.type": "#microsoft.graph.mailSearchFolder",
            "id": "AAMkADYRAAAZg1yTAAA=",
            "displayName": "Weekly digests",
            "parentFolderId": "AQMkADYAAAIBDAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 4,
            "totalItemCount": 5,
            "wellKnownName": null,
            "isSupported": true,
            "filterQuery": "contains(subject, 'weekly digest')"
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
<!--
{
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
