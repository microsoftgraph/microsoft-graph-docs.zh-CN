---
title: 列出 mailFolder
description: 获取已登录用户的邮箱中的所有邮件文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: af3a6970edf051da3cce2c5fc51458ea6f45a388
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812849"
---
# <a name="list-mailfolders"></a><span data-ttu-id="dbe84-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="dbe84-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbe84-104">获取登录用户的邮箱中的所有邮件文件夹, 包括任何[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="dbe84-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dbe84-105">权限</span><span class="sxs-lookup"><span data-stu-id="dbe84-105">Permissions</span></span>
<span data-ttu-id="dbe84-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbe84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbe84-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbe84-108">Permission type</span></span>      | <span data-ttu-id="dbe84-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbe84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbe84-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dbe84-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe84-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dbe84-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbe84-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe84-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dbe84-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbe84-114">Application</span></span> | <span data-ttu-id="dbe84-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe84-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbe84-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbe84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dbe84-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dbe84-117">Optional query parameters</span></span>
<span data-ttu-id="dbe84-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dbe84-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dbe84-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbe84-119">Request headers</span></span>
| <span data-ttu-id="dbe84-120">标头</span><span class="sxs-lookup"><span data-stu-id="dbe84-120">Header</span></span>       | <span data-ttu-id="dbe84-121">值</span><span class="sxs-lookup"><span data-stu-id="dbe84-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dbe84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbe84-122">Authorization</span></span>  | <span data-ttu-id="dbe84-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dbe84-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dbe84-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbe84-125">Content-Type</span></span>   | <span data-ttu-id="dbe84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbe84-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dbe84-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbe84-127">Request body</span></span>
<span data-ttu-id="dbe84-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbe84-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbe84-129">响应</span><span class="sxs-lookup"><span data-stu-id="dbe84-129">Response</span></span>

<span data-ttu-id="dbe84-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="dbe84-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dbe84-131">示例</span><span class="sxs-lookup"><span data-stu-id="dbe84-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbe84-132">请求</span><span class="sxs-lookup"><span data-stu-id="dbe84-132">Request</span></span>
<span data-ttu-id="dbe84-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbe84-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="dbe84-134">响应</span><span class="sxs-lookup"><span data-stu-id="dbe84-134">Response</span></span>
<span data-ttu-id="dbe84-135">下面是一个响应示例, 其中包含一个作为 "收件箱" 下的子文件夹的**mailSearchFolder** 。</span><span class="sxs-lookup"><span data-stu-id="dbe84-135">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="dbe84-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dbe84-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dbe84-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbe84-137">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dbe84-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dbe84-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dbe84-139">C#</span><span class="sxs-lookup"><span data-stu-id="dbe84-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbe84-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="dbe84-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolders-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
