---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级 '
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 73a812b9f1b3899d52d112649ceebb0c594b8489
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666466"
---
# <a name="list-childfolders"></a><span data-ttu-id="db0de-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="db0de-104">List childFolders</span></span>

<span data-ttu-id="db0de-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db0de-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db0de-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="db0de-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

<span data-ttu-id="db0de-108">默认情况下，此操作不会返回隐藏文件夹。</span><span class="sxs-lookup"><span data-stu-id="db0de-108">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="db0de-109">使用查询参数 _includeHiddenFolders_，将它们包括在答复中。</span><span class="sxs-lookup"><span data-stu-id="db0de-109">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="db0de-110">权限</span><span class="sxs-lookup"><span data-stu-id="db0de-110">Permissions</span></span>
<span data-ttu-id="db0de-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db0de-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db0de-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="db0de-113">Permission type</span></span>      | <span data-ttu-id="db0de-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db0de-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db0de-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db0de-115">Delegated (work or school account)</span></span> | <span data-ttu-id="db0de-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db0de-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db0de-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db0de-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db0de-118">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db0de-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db0de-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="db0de-119">Application</span></span> | <span data-ttu-id="db0de-120">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db0de-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db0de-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db0de-121">HTTP request</span></span>

<span data-ttu-id="db0de-122">若要获取指定文件夹的所有子文件夹（隐藏文件夹除外），请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="db0de-122">To get all the child folders under the specified folder, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="db0de-123">若要在答复中包括 _隐藏的_ 子文件夹，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="db0de-123">To include _hidden_ child folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db0de-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db0de-124">Optional query parameters</span></span>
<span data-ttu-id="db0de-125">若要返回所有 childFolder 的列表（包括隐藏的项目，其 **isHidden** 属性为 true），则如 [HTTP 请求](#http-request) 部分所示，在请求 URL 中，将 `includeHiddenFolders` 查询参数指定为 `true`。</span><span class="sxs-lookup"><span data-stu-id="db0de-125">To return a list of all childFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="db0de-126">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db0de-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="db0de-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="db0de-127">Request headers</span></span>
| <span data-ttu-id="db0de-128">名称</span><span class="sxs-lookup"><span data-stu-id="db0de-128">Name</span></span>       | <span data-ttu-id="db0de-129">类型</span><span class="sxs-lookup"><span data-stu-id="db0de-129">Type</span></span> | <span data-ttu-id="db0de-130">说明</span><span class="sxs-lookup"><span data-stu-id="db0de-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db0de-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="db0de-131">Authorization</span></span>  | <span data-ttu-id="db0de-132">string</span><span class="sxs-lookup"><span data-stu-id="db0de-132">string</span></span>  | <span data-ttu-id="db0de-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db0de-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db0de-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="db0de-135">Request body</span></span>
<span data-ttu-id="db0de-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db0de-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db0de-137">响应</span><span class="sxs-lookup"><span data-stu-id="db0de-137">Response</span></span>

<span data-ttu-id="db0de-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="db0de-138">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db0de-139">示例</span><span class="sxs-lookup"><span data-stu-id="db0de-139">Example</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="db0de-140">示例 1：列出邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="db0de-140">Example 1: List mail folders</span></span>

<span data-ttu-id="db0de-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db0de-141">The following is an example of the request.</span></span>

##### <a name="request"></a><span data-ttu-id="db0de-142">请求</span><span class="sxs-lookup"><span data-stu-id="db0de-142">Request</span></span>
<span data-ttu-id="db0de-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db0de-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db0de-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="db0de-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="db0de-145">C#</span><span class="sxs-lookup"><span data-stu-id="db0de-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db0de-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db0de-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db0de-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db0de-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db0de-148">Java</span><span class="sxs-lookup"><span data-stu-id="db0de-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db0de-149">响应</span><span class="sxs-lookup"><span data-stu-id="db0de-149">Response</span></span>
<span data-ttu-id="db0de-p106">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="db0de-p106">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "isHidden": false
    }
  ]
}
```
### <a name="example-2-include-hidden-child-folders-under-a-specified-mail-folder"></a><span data-ttu-id="db0de-152">示例 2：在指定的邮件文件夹中包含隐藏的子文件夹</span><span class="sxs-lookup"><span data-stu-id="db0de-152">Example 2: Include hidden child folders under a specified mail folder</span></span>

<span data-ttu-id="db0de-153">下一个示例使用 `includeHiddenFolders` 查询参数获取特定邮件文件夹中的子文件夹列表（包括隐藏的邮件文件夹）。</span><span class="sxs-lookup"><span data-stu-id="db0de-153">The next example uses the `includeHiddenFolders` query parameter to get a list of child folders under a specified mail folder including hidden mail folders.</span></span> <span data-ttu-id="db0de-154">答复包含 **isHidden** 设置为 true 的“待筛选邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="db0de-154">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

##### <a name="request"></a><span data-ttu-id="db0de-155">请求</span><span class="sxs-lookup"><span data-stu-id="db0de-155">Request</span></span>
<span data-ttu-id="db0de-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db0de-156">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db0de-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="db0de-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_hiddenchildfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="db0de-158">C#</span><span class="sxs-lookup"><span data-stu-id="db0de-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-hiddenchildfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db0de-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db0de-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-hiddenchildfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db0de-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db0de-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-hiddenchildfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db0de-161">Java</span><span class="sxs-lookup"><span data-stu-id="db0de-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-hiddenchildfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db0de-162">响应</span><span class="sxs-lookup"><span data-stu-id="db0de-162">Response</span></span>
<span data-ttu-id="db0de-p108">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="db0de-p108">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Clutters",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "isHidden": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
