---
title: 列出联系人
description: 从登录用户的邮箱文件夹或指定的联系人文件夹中 (.../me/contacts) 联系人。
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0cda56fb840d7a09ec5ad36614effe0e5564bc8b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047082"
---
# <a name="list-contacts"></a><span data-ttu-id="91c15-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="91c15-103">List contacts</span></span>

<span data-ttu-id="91c15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91c15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91c15-105">从登录用户的邮箱文件夹或指定的联系人文件夹中 (.../me/contacts) 联系人。</span><span class="sxs-lookup"><span data-stu-id="91c15-105">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="91c15-106">权限</span><span class="sxs-lookup"><span data-stu-id="91c15-106">Permissions</span></span>
<span data-ttu-id="91c15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91c15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91c15-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="91c15-109">Permission type</span></span>      | <span data-ttu-id="91c15-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91c15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91c15-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91c15-111">Delegated (work or school account)</span></span> | <span data-ttu-id="91c15-112">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91c15-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="91c15-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91c15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91c15-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91c15-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="91c15-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="91c15-115">Application</span></span> | <span data-ttu-id="91c15-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91c15-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="91c15-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91c15-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91c15-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="91c15-118">Optional query parameters</span></span>
<span data-ttu-id="91c15-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="91c15-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="91c15-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="91c15-120">Request headers</span></span>
| <span data-ttu-id="91c15-121">名称</span><span class="sxs-lookup"><span data-stu-id="91c15-121">Name</span></span>       | <span data-ttu-id="91c15-122">类型</span><span class="sxs-lookup"><span data-stu-id="91c15-122">Type</span></span> | <span data-ttu-id="91c15-123">说明</span><span class="sxs-lookup"><span data-stu-id="91c15-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91c15-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="91c15-124">Authorization</span></span>  | <span data-ttu-id="91c15-125">string</span><span class="sxs-lookup"><span data-stu-id="91c15-125">string</span></span>  | <span data-ttu-id="91c15-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91c15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91c15-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="91c15-128">Request body</span></span>
<span data-ttu-id="91c15-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91c15-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91c15-130">响应</span><span class="sxs-lookup"><span data-stu-id="91c15-130">Response</span></span>

<span data-ttu-id="91c15-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="91c15-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91c15-132">示例</span><span class="sxs-lookup"><span data-stu-id="91c15-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91c15-133">请求</span><span class="sxs-lookup"><span data-stu-id="91c15-133">Request</span></span>
<span data-ttu-id="91c15-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91c15-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91c15-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="91c15-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="c"></a>[<span data-ttu-id="91c15-136">C#</span><span class="sxs-lookup"><span data-stu-id="91c15-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91c15-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91c15-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91c15-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91c15-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91c15-139">Java</span><span class="sxs-lookup"><span data-stu-id="91c15-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91c15-140">响应</span><span class="sxs-lookup"><span data-stu-id="91c15-140">Response</span></span>
<span data-ttu-id="91c15-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="91c15-141">Here is an example of the response.</span></span> <span data-ttu-id="91c15-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="91c15-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
