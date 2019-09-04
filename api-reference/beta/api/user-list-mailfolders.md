---
title: 列出 mailFolder
description: 获取已登录用户的邮箱中的所有邮件文件夹。
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1a58748afccb5a5b155a047c7cade259f05984c4
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721955"
---
# <a name="list-mailfolders"></a><span data-ttu-id="6fe11-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="6fe11-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fe11-104">获取登录用户的邮箱中的所有邮件文件夹, 包括任何[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="6fe11-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fe11-105">权限</span><span class="sxs-lookup"><span data-stu-id="6fe11-105">Permissions</span></span>
<span data-ttu-id="6fe11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fe11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe11-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fe11-108">Permission type</span></span>      | <span data-ttu-id="6fe11-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fe11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fe11-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fe11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6fe11-111">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="6fe11-111">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6fe11-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fe11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fe11-113">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="6fe11-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6fe11-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fe11-114">Application</span></span> | <span data-ttu-id="6fe11-115">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="6fe11-115">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fe11-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fe11-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fe11-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6fe11-117">Optional query parameters</span></span>
<span data-ttu-id="6fe11-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6fe11-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6fe11-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fe11-119">Request headers</span></span>
| <span data-ttu-id="6fe11-120">标头</span><span class="sxs-lookup"><span data-stu-id="6fe11-120">Header</span></span>       | <span data-ttu-id="6fe11-121">值</span><span class="sxs-lookup"><span data-stu-id="6fe11-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fe11-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fe11-122">Authorization</span></span>  | <span data-ttu-id="6fe11-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fe11-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6fe11-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6fe11-125">Content-Type</span></span>   | <span data-ttu-id="6fe11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fe11-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fe11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fe11-127">Request body</span></span>
<span data-ttu-id="6fe11-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fe11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fe11-129">响应</span><span class="sxs-lookup"><span data-stu-id="6fe11-129">Response</span></span>

<span data-ttu-id="6fe11-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6fe11-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fe11-131">示例</span><span class="sxs-lookup"><span data-stu-id="6fe11-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fe11-132">请求</span><span class="sxs-lookup"><span data-stu-id="6fe11-132">Request</span></span>
<span data-ttu-id="6fe11-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fe11-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fe11-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6fe11-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fe11-135">C#</span><span class="sxs-lookup"><span data-stu-id="6fe11-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fe11-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fe11-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fe11-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="6fe11-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6fe11-138">响应</span><span class="sxs-lookup"><span data-stu-id="6fe11-138">Response</span></span>
<span data-ttu-id="6fe11-139">下面是一个响应示例, 其中包含一个作为 "收件箱" 下的子文件夹的**mailSearchFolder** 。</span><span class="sxs-lookup"><span data-stu-id="6fe11-139">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="6fe11-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6fe11-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6fe11-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fe11-141">All of the properties will be returned from an actual call.</span></span>
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
