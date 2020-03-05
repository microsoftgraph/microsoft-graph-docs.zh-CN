---
title: 列出联系人
description: 获取登录用户的邮箱中的所有联系人（../me/contacts），或从指定的联系人文件夹中获取。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 052569c5c58f0e3cfb932724b549767d984b8ca7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436893"
---
# <a name="list-contacts"></a><span data-ttu-id="efd27-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="efd27-103">List contacts</span></span>

<span data-ttu-id="efd27-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="efd27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd27-105">获取登录用户的邮箱中的所有联系人（../me/contacts），或从指定的联系人文件夹中获取。</span><span class="sxs-lookup"><span data-stu-id="efd27-105">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="efd27-106">权限</span><span class="sxs-lookup"><span data-stu-id="efd27-106">Permissions</span></span>
<span data-ttu-id="efd27-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efd27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd27-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd27-109">Permission type</span></span>      | <span data-ttu-id="efd27-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efd27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efd27-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd27-111">Delegated (work or school account)</span></span> | <span data-ttu-id="efd27-112">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efd27-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="efd27-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efd27-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efd27-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="efd27-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd27-115">Application</span></span> | <span data-ttu-id="efd27-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efd27-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="efd27-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd27-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="efd27-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="efd27-118">Optional query parameters</span></span>
<span data-ttu-id="efd27-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="efd27-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="efd27-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd27-120">Request headers</span></span>
| <span data-ttu-id="efd27-121">名称</span><span class="sxs-lookup"><span data-stu-id="efd27-121">Name</span></span>       | <span data-ttu-id="efd27-122">类型</span><span class="sxs-lookup"><span data-stu-id="efd27-122">Type</span></span> | <span data-ttu-id="efd27-123">说明</span><span class="sxs-lookup"><span data-stu-id="efd27-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="efd27-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd27-124">Authorization</span></span>  | <span data-ttu-id="efd27-125">string</span><span class="sxs-lookup"><span data-stu-id="efd27-125">string</span></span>  | <span data-ttu-id="efd27-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efd27-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efd27-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd27-128">Request body</span></span>
<span data-ttu-id="efd27-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efd27-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efd27-130">响应</span><span class="sxs-lookup"><span data-stu-id="efd27-130">Response</span></span>

<span data-ttu-id="efd27-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="efd27-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="efd27-132">示例</span><span class="sxs-lookup"><span data-stu-id="efd27-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efd27-133">请求</span><span class="sxs-lookup"><span data-stu-id="efd27-133">Request</span></span>
<span data-ttu-id="efd27-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efd27-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="efd27-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="efd27-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="c"></a>[<span data-ttu-id="efd27-136">C#</span><span class="sxs-lookup"><span data-stu-id="efd27-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efd27-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efd27-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efd27-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efd27-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="efd27-139">响应</span><span class="sxs-lookup"><span data-stu-id="efd27-139">Response</span></span>
<span data-ttu-id="efd27-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efd27-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
