---
title: 列出联系人
description: 从已登录用户的默认联系人文件夹中获取联系人集合。
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1d5d12fc90bd713ec4df1f96d69a9bf0c74e880b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050218"
---
# <a name="list-contacts"></a><span data-ttu-id="968d6-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="968d6-103">List contacts</span></span>

<span data-ttu-id="968d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="968d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="968d6-105">从已登录用户的默认联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="968d6-105">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="968d6-106">在以下两种情况下，应用可以获取其他用户的联系人文件夹中的联系人：</span><span class="sxs-lookup"><span data-stu-id="968d6-106">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="968d6-107">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="968d6-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="968d6-108">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="968d6-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="968d6-109">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="968d6-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="968d6-110">权限</span><span class="sxs-lookup"><span data-stu-id="968d6-110">Permissions</span></span>
<span data-ttu-id="968d6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="968d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="968d6-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="968d6-113">Permission type</span></span>      | <span data-ttu-id="968d6-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="968d6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="968d6-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="968d6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="968d6-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="968d6-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="968d6-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="968d6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="968d6-118">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="968d6-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="968d6-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="968d6-119">Application</span></span> | <span data-ttu-id="968d6-120">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="968d6-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="968d6-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="968d6-121">HTTP request</span></span>

<span data-ttu-id="968d6-122">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="968d6-122">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="968d6-123">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="968d6-123">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolders/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="968d6-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="968d6-124">Optional query parameters</span></span>
<span data-ttu-id="968d6-125">可以使用 `$filter` 查询参数根据联系人的电子邮件地址来筛选联系人：</span><span class="sxs-lookup"><span data-stu-id="968d6-125">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="968d6-126">请注意，可以仅针对 **emailAddresses** 集合的实例的 **address** 子属性使用 `$filter`、`any` 和 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="968d6-126">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="968d6-127">也就是说，不能筛选 **emailAddresses** 的实例的 **name** 或其他子属性，也不能对 `filter` 应用任何其他运算符或函数，例如 `ne`、`le` 和 `startswith()`。</span><span class="sxs-lookup"><span data-stu-id="968d6-127">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="968d6-128">有关 `$filter` 查询参数的一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="968d6-128">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="968d6-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="968d6-129">Request headers</span></span>
| <span data-ttu-id="968d6-130">标头</span><span class="sxs-lookup"><span data-stu-id="968d6-130">Header</span></span>       | <span data-ttu-id="968d6-131">值</span><span class="sxs-lookup"><span data-stu-id="968d6-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="968d6-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="968d6-132">Authorization</span></span>  | <span data-ttu-id="968d6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="968d6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="968d6-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="968d6-135">Content-Type</span></span>   | <span data-ttu-id="968d6-136">application/json</span><span class="sxs-lookup"><span data-stu-id="968d6-136">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="968d6-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="968d6-137">Request body</span></span>
<span data-ttu-id="968d6-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="968d6-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="968d6-139">响应</span><span class="sxs-lookup"><span data-stu-id="968d6-139">Response</span></span>

<span data-ttu-id="968d6-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="968d6-140">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="968d6-141">示例</span><span class="sxs-lookup"><span data-stu-id="968d6-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="968d6-142">请求</span><span class="sxs-lookup"><span data-stu-id="968d6-142">Request</span></span>
<span data-ttu-id="968d6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="968d6-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="968d6-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="968d6-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contacts
```
# <a name="c"></a>[<span data-ttu-id="968d6-145">C#</span><span class="sxs-lookup"><span data-stu-id="968d6-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="968d6-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="968d6-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="968d6-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="968d6-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="968d6-148">Java</span><span class="sxs-lookup"><span data-stu-id="968d6-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="968d6-149">响应</span><span class="sxs-lookup"><span data-stu-id="968d6-149">Response</span></span>
<span data-ttu-id="968d6-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="968d6-150">Here is an example of the response.</span></span> <span data-ttu-id="968d6-151">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="968d6-151">Note: The response object shown here might be shortened for readability.</span></span>
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

