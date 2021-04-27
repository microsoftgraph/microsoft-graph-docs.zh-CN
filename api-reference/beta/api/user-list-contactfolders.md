---
title: List contactFolders
description: 获取已登录用户的邮箱中所有的联系人文件夹。
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c8b69f7e76802ffd092b0ef854e42f2815b08e9b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051723"
---
# <a name="list-contactfolders"></a><span data-ttu-id="cc074-103">List contactFolders</span><span class="sxs-lookup"><span data-stu-id="cc074-103">List contactFolders</span></span>

<span data-ttu-id="cc074-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc074-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc074-105">获取已登录用户的邮箱中所有的联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="cc074-105">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc074-106">权限</span><span class="sxs-lookup"><span data-stu-id="cc074-106">Permissions</span></span>
<span data-ttu-id="cc074-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc074-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc074-109">Permission type</span></span>      | <span data-ttu-id="cc074-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc074-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc074-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc074-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc074-112">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc074-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cc074-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc074-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc074-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc074-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cc074-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc074-115">Application</span></span> | <span data-ttu-id="cc074-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc074-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc074-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc074-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc074-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc074-118">Optional query parameters</span></span>
<span data-ttu-id="cc074-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cc074-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cc074-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc074-120">Request headers</span></span>
| <span data-ttu-id="cc074-121">标头</span><span class="sxs-lookup"><span data-stu-id="cc074-121">Header</span></span>       | <span data-ttu-id="cc074-122">值</span><span class="sxs-lookup"><span data-stu-id="cc074-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc074-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc074-123">Authorization</span></span>  | <span data-ttu-id="cc074-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc074-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc074-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc074-126">Content-Type</span></span>   | <span data-ttu-id="cc074-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cc074-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc074-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc074-128">Request body</span></span>
<span data-ttu-id="cc074-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc074-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc074-130">响应</span><span class="sxs-lookup"><span data-stu-id="cc074-130">Response</span></span>

<span data-ttu-id="cc074-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cc074-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc074-132">示例</span><span class="sxs-lookup"><span data-stu-id="cc074-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc074-133">请求</span><span class="sxs-lookup"><span data-stu-id="cc074-133">Request</span></span>
<span data-ttu-id="cc074-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc074-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc074-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc074-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="cc074-136">C#</span><span class="sxs-lookup"><span data-stu-id="cc074-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc074-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc074-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc074-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc074-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc074-139">Java</span><span class="sxs-lookup"><span data-stu-id="cc074-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cc074-140">响应</span><span class="sxs-lookup"><span data-stu-id="cc074-140">Response</span></span>
<span data-ttu-id="cc074-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc074-141">Here is an example of the response.</span></span> <span data-ttu-id="cc074-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc074-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBCAAAAA==",
      "displayName": "Contacts",
      "id": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
      "wellKnownName": "contacts"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
