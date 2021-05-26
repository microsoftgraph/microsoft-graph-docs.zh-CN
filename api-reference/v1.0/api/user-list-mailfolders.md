---
title: 列出 mailFolder
description: '在已登录用户的根文件夹下获取邮件文件夹集合。 '
author: abheek-das
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 2f6d8a749cd01f921f201657fd047a90642e4fe9
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666201"
---
# <a name="list-mailfolders"></a><span data-ttu-id="e0e1c-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="e0e1c-103">List mailFolders</span></span>

<span data-ttu-id="e0e1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0e1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0e1c-105">直接在已登录用户的根文件夹下获取邮件文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-105">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="e0e1c-106">返回的集合包括直接在根目录下的所有[邮件搜索文件夹](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-106">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

<span data-ttu-id="e0e1c-107">默认情况下，此操作不会返回隐藏文件夹。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-107">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="e0e1c-108">使用查询参数 _includeHiddenFolders_，将它们包括在答复中。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-108">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0e1c-109">权限</span><span class="sxs-lookup"><span data-stu-id="e0e1c-109">Permissions</span></span>
<span data-ttu-id="e0e1c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0e1c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0e1c-112">Permission type</span></span>      | <span data-ttu-id="e0e1c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0e1c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0e1c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0e1c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e0e1c-115">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0e1c-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e0e1c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0e1c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0e1c-117">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0e1c-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e0e1c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0e1c-118">Application</span></span> | <span data-ttu-id="e0e1c-119">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0e1c-119">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0e1c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0e1c-120">HTTP request</span></span>

<span data-ttu-id="e0e1c-121">若要获取指定用户邮箱内的所有邮件文件夹（隐藏文件夹除外），请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e0e1c-121">To get all the mail folders in the specified user's mailbox, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

<span data-ttu-id="e0e1c-122">若要在答复中包括 _隐藏的_ 邮件文件夹，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e0e1c-122">To include _hidden_ mail folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0e1c-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e0e1c-123">Optional query parameters</span></span>
<span data-ttu-id="e0e1c-124">若要返回所有 mailFolder 的列表（包括隐藏的项目，其 **isHidden** 属性为 true），则如 [HTTP 请求](#http-request) 部分所示，在请求 URL 中，将 `includeHiddenFolders` 查询参数指定为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-124">To return a list of all mailFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="e0e1c-125">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e0e1c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0e1c-126">Request headers</span></span>
| <span data-ttu-id="e0e1c-127">标头</span><span class="sxs-lookup"><span data-stu-id="e0e1c-127">Header</span></span>       | <span data-ttu-id="e0e1c-128">值</span><span class="sxs-lookup"><span data-stu-id="e0e1c-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0e1c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0e1c-129">Authorization</span></span>  | <span data-ttu-id="e0e1c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0e1c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0e1c-132">Content-Type</span></span>   | <span data-ttu-id="e0e1c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e0e1c-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0e1c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0e1c-134">Request body</span></span>
<span data-ttu-id="e0e1c-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0e1c-136">响应</span><span class="sxs-lookup"><span data-stu-id="e0e1c-136">Response</span></span>

<span data-ttu-id="e0e1c-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-137">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e0e1c-138">示例</span><span class="sxs-lookup"><span data-stu-id="e0e1c-138">Examples</span></span>

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="e0e1c-139">示例 1：列出已登录用户邮箱中的邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="e0e1c-139">Example 1: List mail folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="e0e1c-140">此示例在答复中包括了 **mailSearchFolder** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-140">This example includes a **mailSearchFolder** object in the response.</span></span> <span data-ttu-id="e0e1c-141">邮件搜索文件夹是收件箱下的子文件夹，显示名称为"每周摘要"。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-141">The mail search folder is a child folder under the Inbox with the display name "Weekly digests".</span></span>

#### <a name="request"></a><span data-ttu-id="e0e1c-142">请求</span><span class="sxs-lookup"><span data-stu-id="e0e1c-142">Request</span></span>
<span data-ttu-id="e0e1c-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0e1c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e1c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="e0e1c-145">C#</span><span class="sxs-lookup"><span data-stu-id="e0e1c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0e1c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0e1c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0e1c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0e1c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0e1c-148">Java</span><span class="sxs-lookup"><span data-stu-id="e0e1c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0e1c-149">响应</span><span class="sxs-lookup"><span data-stu-id="e0e1c-149">Response</span></span>
<span data-ttu-id="e0e1c-150">以下是响应示例，其中包含一个收件箱下的子文件夹 **mailSearchFolder**。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-150">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="e0e1c-151">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e0e1c-152">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-152">All of the properties will be returned from an actual call.</span></span>

><span data-ttu-id="e0e1c-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
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
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        }
    ]
}
```

### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="e0e1c-154">示例 2：包含已登录用户邮箱中的隐藏文件夹</span><span class="sxs-lookup"><span data-stu-id="e0e1c-154">Example 2: Include hidden folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="e0e1c-155">下一个示例使用 `includeHiddenFolders` 查询参数获取邮件文件夹列表（包括隐藏的邮件文件夹）。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-155">The next example uses the `includeHiddenFolders` query parameter to get a list of mail folders including hidden mail folders.</span></span> <span data-ttu-id="e0e1c-156">答复包含 **isHidden** 设置为 true 的“待筛选邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-156">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="e0e1c-157">请求</span><span class="sxs-lookup"><span data-stu-id="e0e1c-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e0e1c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e1c-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="e0e1c-159">C#</span><span class="sxs-lookup"><span data-stu-id="e0e1c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hiddenmailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0e1c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0e1c-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hiddenmailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0e1c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0e1c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hiddenmailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0e1c-162">Java</span><span class="sxs-lookup"><span data-stu-id="e0e1c-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hiddenmailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e0e1c-163">响应</span><span class="sxs-lookup"><span data-stu-id="e0e1c-163">Response</span></span>
<span data-ttu-id="e0e1c-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-164">Here is an example of the response.</span></span>

><span data-ttu-id="e0e1c-165">**注意：** 为提高可读性，此处显示的答复对象已缩短，并且用户邮箱中不包含所有默认文件夹。</span><span class="sxs-lookup"><span data-stu-id="e0e1c-165">**Note:** The response object shown here is shortened for readability, and doesn't include all the default folders in a user mailbox.</span></span>
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
            "isHidden": true
        },
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Conversation History",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
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
