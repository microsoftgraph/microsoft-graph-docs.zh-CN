---
title: 列出 childFolder
description: '获取指定文件夹下的文件夹集合。 可以使用 `.../me/MailFolders` 快捷方式来获取顶级 '
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3b8cb47681963233543a40449a1206c3206bb2f0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131605"
---
# <a name="list-childfolders"></a><span data-ttu-id="b9e17-104">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="b9e17-104">List childFolders</span></span>

<span data-ttu-id="b9e17-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9e17-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9e17-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/mailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="b9e17-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9e17-108">权限</span><span class="sxs-lookup"><span data-stu-id="b9e17-108">Permissions</span></span>
<span data-ttu-id="b9e17-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e17-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e17-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e17-111">Permission type</span></span>      | <span data-ttu-id="b9e17-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e17-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9e17-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e17-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9e17-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e17-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b9e17-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e17-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e17-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e17-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b9e17-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e17-117">Application</span></span> | <span data-ttu-id="b9e17-118">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e17-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9e17-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e17-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9e17-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b9e17-120">Optional query parameters</span></span>
<span data-ttu-id="b9e17-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b9e17-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9e17-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e17-122">Request headers</span></span>
| <span data-ttu-id="b9e17-123">名称</span><span class="sxs-lookup"><span data-stu-id="b9e17-123">Name</span></span>       | <span data-ttu-id="b9e17-124">类型</span><span class="sxs-lookup"><span data-stu-id="b9e17-124">Type</span></span> | <span data-ttu-id="b9e17-125">说明</span><span class="sxs-lookup"><span data-stu-id="b9e17-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b9e17-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e17-126">Authorization</span></span>  | <span data-ttu-id="b9e17-127">string</span><span class="sxs-lookup"><span data-stu-id="b9e17-127">string</span></span>  | <span data-ttu-id="b9e17-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e17-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9e17-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e17-130">Request body</span></span>
<span data-ttu-id="b9e17-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9e17-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e17-132">响应</span><span class="sxs-lookup"><span data-stu-id="b9e17-132">Response</span></span>

<span data-ttu-id="b9e17-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b9e17-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9e17-134">示例</span><span class="sxs-lookup"><span data-stu-id="b9e17-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9e17-135">请求</span><span class="sxs-lookup"><span data-stu-id="b9e17-135">Request</span></span>
<span data-ttu-id="b9e17-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9e17-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9e17-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9e17-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="b9e17-138">C#</span><span class="sxs-lookup"><span data-stu-id="b9e17-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9e17-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9e17-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9e17-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9e17-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9e17-141">Java</span><span class="sxs-lookup"><span data-stu-id="b9e17-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9e17-142">响应</span><span class="sxs-lookup"><span data-stu-id="b9e17-142">Response</span></span>
<span data-ttu-id="b9e17-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9e17-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
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
