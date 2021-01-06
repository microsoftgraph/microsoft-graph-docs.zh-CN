---
title: 列出 mailFolder
description: 获取已登录用户的邮箱中的所有邮件文件夹。
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: c2cf43dc9d01ba2de2a3426cce84aaf3f92bbbb3
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768202"
---
# <a name="list-mailfolders"></a><span data-ttu-id="88216-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="88216-103">List mailFolders</span></span>

<span data-ttu-id="88216-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88216-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88216-105">获取指定用户邮箱中所有的邮件文件夹，包括任何 [邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="88216-105">Get all the mail folders in the specified user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="88216-106">默认情况下，此操作不会返回隐藏文件夹。</span><span class="sxs-lookup"><span data-stu-id="88216-106">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="88216-107">使用查询参数 _includeHiddenFolders_ 将其包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="88216-107">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="88216-108">权限</span><span class="sxs-lookup"><span data-stu-id="88216-108">Permissions</span></span>
<span data-ttu-id="88216-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88216-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88216-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88216-111">Permission type</span></span>      | <span data-ttu-id="88216-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88216-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88216-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88216-113">Delegated (work or school account)</span></span> | <span data-ttu-id="88216-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88216-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="88216-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88216-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88216-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88216-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="88216-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88216-117">Application</span></span> | <span data-ttu-id="88216-118">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88216-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="88216-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88216-119">HTTP request</span></span>

<span data-ttu-id="88216-120">若要获取指定用户邮箱中所有邮件文件夹（不包括隐藏的文件夹）：</span><span class="sxs-lookup"><span data-stu-id="88216-120">To get all the mail folders in the specified user's mailbox, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

<span data-ttu-id="88216-121">若要在 _响应_ 中包括隐藏的邮件文件夹：</span><span class="sxs-lookup"><span data-stu-id="88216-121">To include _hidden_ mail folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="query-parameters"></a><span data-ttu-id="88216-122">查询参数</span><span class="sxs-lookup"><span data-stu-id="88216-122">Query parameters</span></span>
<span data-ttu-id="88216-123">若要返回所有 mailFolders 的列表，包括隐藏的 mailFolders (其 **isHidden** 属性为 true) ，在请求 URL 中，将查询参数指定为 ， `includeHiddenFolders` 如 `true` [HTTP](#http-request) 请求部分所示。</span><span class="sxs-lookup"><span data-stu-id="88216-123">To return a list of all mailFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="88216-124">此方法还支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="88216-124">This method also supports [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88216-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="88216-125">Request headers</span></span>
| <span data-ttu-id="88216-126">标头</span><span class="sxs-lookup"><span data-stu-id="88216-126">Header</span></span>       | <span data-ttu-id="88216-127">值</span><span class="sxs-lookup"><span data-stu-id="88216-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88216-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="88216-128">Authorization</span></span>  | <span data-ttu-id="88216-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88216-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88216-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="88216-131">Request body</span></span>
<span data-ttu-id="88216-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88216-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88216-133">响应</span><span class="sxs-lookup"><span data-stu-id="88216-133">Response</span></span>

<span data-ttu-id="88216-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="88216-134">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="88216-135">示例</span><span class="sxs-lookup"><span data-stu-id="88216-135">Examples</span></span>

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="88216-136">示例 1：列出已登录用户的邮箱中的邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="88216-136">Example 1: List mail folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="88216-137">本示例在响应 **中包含 mailSearchFolder** 对象。</span><span class="sxs-lookup"><span data-stu-id="88216-137">This example includes a **mailSearchFolder** object in the response.</span></span> <span data-ttu-id="88216-138">邮件搜索文件夹是收件箱下的子文件夹，其显示名称摘要"。</span><span class="sxs-lookup"><span data-stu-id="88216-138">The mail search folder is a child folder under the Inbox with the display name "Weekly digests".</span></span>

#### <a name="request"></a><span data-ttu-id="88216-139">请求</span><span class="sxs-lookup"><span data-stu-id="88216-139">Request</span></span>
<span data-ttu-id="88216-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88216-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88216-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="88216-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="88216-142">C#</span><span class="sxs-lookup"><span data-stu-id="88216-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88216-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88216-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88216-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88216-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88216-145">Java</span><span class="sxs-lookup"><span data-stu-id="88216-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="88216-146">响应</span><span class="sxs-lookup"><span data-stu-id="88216-146">Response</span></span>
<span data-ttu-id="88216-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88216-147">Here is an example of the response.</span></span> 

><span data-ttu-id="88216-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88216-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
            "wellKnownName": "archive",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "deleteditems",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "drafts",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "wellKnownName": "inbox",
            "isHidden": false
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
            "isHidden": false,
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
            "wellKnownName": "junkemail",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "outbox",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "sentitems",
            "isHidden": false
        }
    ]
}
```


### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="88216-149">示例 2：在登录用户的邮箱中包括隐藏文件夹</span><span class="sxs-lookup"><span data-stu-id="88216-149">Example 2: Include hidden folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="88216-150">下一个示例使用 `includeHiddenFolders` 查询参数获取包含隐藏邮件文件夹的邮件文件夹列表。</span><span class="sxs-lookup"><span data-stu-id="88216-150">The next example uses the `includeHiddenFolders` query parameter to get a list of mail folders including hidden mail folders.</span></span> <span data-ttu-id="88216-151">该响应包括将 **isHidden** 设置为 true 的"待筛选邮件"文件夹。</span><span class="sxs-lookup"><span data-stu-id="88216-151">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="88216-152">请求</span><span class="sxs-lookup"><span data-stu-id="88216-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88216-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="88216-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="88216-154">C#</span><span class="sxs-lookup"><span data-stu-id="88216-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hiddenmailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88216-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88216-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hiddenmailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88216-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88216-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hiddenmailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88216-157">Java</span><span class="sxs-lookup"><span data-stu-id="88216-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hiddenmailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="88216-158">响应</span><span class="sxs-lookup"><span data-stu-id="88216-158">Response</span></span>
<span data-ttu-id="88216-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88216-159">Here is an example of the response.</span></span>

><span data-ttu-id="88216-160">**注意：** 为了可读性，此处所示的响应对象已缩短，并且不包含用户邮箱中所有的默认文件夹。</span><span class="sxs-lookup"><span data-stu-id="88216-160">**Note:** The response object shown here is shortened for readability, and doesn't include all the default folders in a user mailbox.</span></span>
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
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Clutters",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": null,
            "isHidden": true
        },
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Conversation History",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory",
            "isHidden": false
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
