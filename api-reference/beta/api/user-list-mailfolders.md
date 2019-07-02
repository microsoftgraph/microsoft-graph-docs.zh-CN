---
title: 列出 mailFolder
description: 获取已登录用户的邮箱中的所有邮件文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: be5b7d684c01dcc8fd22ee83d120ea67696a3c9d
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417666"
---
# <a name="list-mailfolders"></a><span data-ttu-id="daad7-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="daad7-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daad7-104">获取登录用户的邮箱中的所有邮件文件夹, 包括任何[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="daad7-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="daad7-105">权限</span><span class="sxs-lookup"><span data-stu-id="daad7-105">Permissions</span></span>
<span data-ttu-id="daad7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="daad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daad7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="daad7-108">Permission type</span></span>      | <span data-ttu-id="daad7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="daad7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="daad7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="daad7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="daad7-111">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="daad7-111">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="daad7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="daad7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daad7-113">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="daad7-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="daad7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="daad7-114">Application</span></span> | <span data-ttu-id="daad7-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="daad7-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="daad7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="daad7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="daad7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="daad7-117">Optional query parameters</span></span>
<span data-ttu-id="daad7-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="daad7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="daad7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="daad7-119">Request headers</span></span>
| <span data-ttu-id="daad7-120">标头</span><span class="sxs-lookup"><span data-stu-id="daad7-120">Header</span></span>       | <span data-ttu-id="daad7-121">值</span><span class="sxs-lookup"><span data-stu-id="daad7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="daad7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="daad7-122">Authorization</span></span>  | <span data-ttu-id="daad7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="daad7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="daad7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="daad7-125">Content-Type</span></span>   | <span data-ttu-id="daad7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="daad7-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="daad7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="daad7-127">Request body</span></span>
<span data-ttu-id="daad7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="daad7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daad7-129">响应</span><span class="sxs-lookup"><span data-stu-id="daad7-129">Response</span></span>

<span data-ttu-id="daad7-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="daad7-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="daad7-131">示例</span><span class="sxs-lookup"><span data-stu-id="daad7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="daad7-132">请求</span><span class="sxs-lookup"><span data-stu-id="daad7-132">Request</span></span>
<span data-ttu-id="daad7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="daad7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="daad7-134">响应</span><span class="sxs-lookup"><span data-stu-id="daad7-134">Response</span></span>
<span data-ttu-id="daad7-135">下面是一个响应示例, 其中包含一个作为 "收件箱" 下的子文件夹的**mailSearchFolder** 。</span><span class="sxs-lookup"><span data-stu-id="daad7-135">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="daad7-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="daad7-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="daad7-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="daad7-137">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="daad7-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="daad7-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="daad7-139">C#</span><span class="sxs-lookup"><span data-stu-id="daad7-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="daad7-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="daad7-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="daad7-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="daad7-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
