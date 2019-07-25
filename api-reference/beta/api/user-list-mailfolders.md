---
title: 列出 mailFolder
description: 获取已登录用户的邮箱中的所有邮件文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c006e1f4b8714c332b9a1d3144c660784fda11f5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867235"
---
# <a name="list-mailfolders"></a><span data-ttu-id="35b50-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="35b50-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b50-104">获取登录用户的邮箱中的所有邮件文件夹, 包括任何[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="35b50-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35b50-105">权限</span><span class="sxs-lookup"><span data-stu-id="35b50-105">Permissions</span></span>
<span data-ttu-id="35b50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35b50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35b50-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="35b50-108">Permission type</span></span>      | <span data-ttu-id="35b50-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35b50-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35b50-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35b50-110">Delegated (work or school account)</span></span> | <span data-ttu-id="35b50-111">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="35b50-111">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35b50-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35b50-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35b50-113">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="35b50-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35b50-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="35b50-114">Application</span></span> | <span data-ttu-id="35b50-115">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="35b50-115">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35b50-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35b50-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35b50-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35b50-117">Optional query parameters</span></span>
<span data-ttu-id="35b50-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35b50-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35b50-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="35b50-119">Request headers</span></span>
| <span data-ttu-id="35b50-120">标头</span><span class="sxs-lookup"><span data-stu-id="35b50-120">Header</span></span>       | <span data-ttu-id="35b50-121">值</span><span class="sxs-lookup"><span data-stu-id="35b50-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35b50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35b50-122">Authorization</span></span>  | <span data-ttu-id="35b50-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35b50-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="35b50-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35b50-125">Content-Type</span></span>   | <span data-ttu-id="35b50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35b50-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35b50-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="35b50-127">Request body</span></span>
<span data-ttu-id="35b50-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="35b50-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35b50-129">响应</span><span class="sxs-lookup"><span data-stu-id="35b50-129">Response</span></span>

<span data-ttu-id="35b50-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="35b50-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35b50-131">示例</span><span class="sxs-lookup"><span data-stu-id="35b50-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35b50-132">请求</span><span class="sxs-lookup"><span data-stu-id="35b50-132">Request</span></span>
<span data-ttu-id="35b50-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35b50-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="35b50-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="35b50-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35b50-135">C#</span><span class="sxs-lookup"><span data-stu-id="35b50-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35b50-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="35b50-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35b50-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="35b50-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35b50-138">Java</span><span class="sxs-lookup"><span data-stu-id="35b50-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="35b50-139">响应</span><span class="sxs-lookup"><span data-stu-id="35b50-139">Response</span></span>
<span data-ttu-id="35b50-140">下面是一个响应示例, 其中包含一个作为 "收件箱" 下的子文件夹的**mailSearchFolder** 。</span><span class="sxs-lookup"><span data-stu-id="35b50-140">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="35b50-141">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="35b50-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="35b50-142">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35b50-142">All of the properties will be returned from an actual call.</span></span>
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
