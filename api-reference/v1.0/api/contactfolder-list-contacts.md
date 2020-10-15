---
title: 列出联系人
description: 从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b06818def9ed051ac536a2f08e29906a001410a7
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459230"
---
# <a name="list-contacts"></a><span data-ttu-id="c7e47-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="c7e47-103">List contacts</span></span>

<span data-ttu-id="c7e47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7e47-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7e47-105">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="c7e47-105">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7e47-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7e47-106">Permissions</span></span>
<span data-ttu-id="c7e47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7e47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e47-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7e47-109">Permission type</span></span>      | <span data-ttu-id="c7e47-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7e47-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7e47-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7e47-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7e47-112">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e47-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c7e47-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7e47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7e47-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e47-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c7e47-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7e47-115">Application</span></span> | <span data-ttu-id="c7e47-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e47-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7e47-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7e47-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7e47-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7e47-118">Optional query parameters</span></span>
<span data-ttu-id="c7e47-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7e47-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c7e47-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7e47-120">Request headers</span></span>
| <span data-ttu-id="c7e47-121">名称</span><span class="sxs-lookup"><span data-stu-id="c7e47-121">Name</span></span>       | <span data-ttu-id="c7e47-122">类型</span><span class="sxs-lookup"><span data-stu-id="c7e47-122">Type</span></span> | <span data-ttu-id="c7e47-123">说明</span><span class="sxs-lookup"><span data-stu-id="c7e47-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c7e47-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7e47-124">Authorization</span></span>  | <span data-ttu-id="c7e47-125">string</span><span class="sxs-lookup"><span data-stu-id="c7e47-125">string</span></span>  | <span data-ttu-id="c7e47-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7e47-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7e47-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7e47-128">Request body</span></span>
<span data-ttu-id="c7e47-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7e47-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7e47-130">响应</span><span class="sxs-lookup"><span data-stu-id="c7e47-130">Response</span></span>

<span data-ttu-id="c7e47-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c7e47-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7e47-132">示例</span><span class="sxs-lookup"><span data-stu-id="c7e47-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7e47-133">请求</span><span class="sxs-lookup"><span data-stu-id="c7e47-133">Request</span></span>
<span data-ttu-id="c7e47-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7e47-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7e47-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7e47-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
# <a name="c"></a>[<span data-ttu-id="c7e47-136">C#</span><span class="sxs-lookup"><span data-stu-id="c7e47-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7e47-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7e47-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7e47-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7e47-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7e47-139">Java</span><span class="sxs-lookup"><span data-stu-id="c7e47-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c7e47-140">响应</span><span class="sxs-lookup"><span data-stu-id="c7e47-140">Response</span></span>
<span data-ttu-id="c7e47-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7e47-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "birthday": "datetime-value",
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
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
