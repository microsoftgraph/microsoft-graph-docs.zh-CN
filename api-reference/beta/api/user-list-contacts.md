---
title: 列出联系人
description: 获取用户邮箱中的联系人。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca9766c81ee6ee7121f856bf88c094191da02fb9
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724209"
---
# <a name="list-contacts"></a><span data-ttu-id="c3d58-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="c3d58-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3d58-104">获取用户邮箱中的联系人。</span><span class="sxs-lookup"><span data-stu-id="c3d58-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="c3d58-105">在以下两种情况下，应用可以获取其他用户的联系人文件夹中的联系人：</span><span class="sxs-lookup"><span data-stu-id="c3d58-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="c3d58-106">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="c3d58-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="c3d58-107">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c3d58-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="c3d58-108">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="c3d58-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="c3d58-109">权限</span><span class="sxs-lookup"><span data-stu-id="c3d58-109">Permissions</span></span>
<span data-ttu-id="c3d58-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3d58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3d58-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3d58-112">Permission type</span></span>      | <span data-ttu-id="c3d58-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3d58-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3d58-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3d58-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c3d58-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3d58-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c3d58-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3d58-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3d58-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3d58-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c3d58-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3d58-118">Application</span></span> | <span data-ttu-id="c3d58-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3d58-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3d58-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3d58-120">HTTP request</span></span>

<span data-ttu-id="c3d58-121">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c3d58-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="c3d58-122">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c3d58-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3d58-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c3d58-123">Optional query parameters</span></span>
<span data-ttu-id="c3d58-124">可以使用 `$filter` 查询参数根据联系人的电子邮件地址来筛选联系人：</span><span class="sxs-lookup"><span data-stu-id="c3d58-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="c3d58-125">请注意，可以仅针对 **emailAddresses** 集合的实例的 **address** 子属性使用 `$filter`、`any` 和 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="c3d58-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="c3d58-126">也就是说，不能筛选 **emailAddresses** 的实例的 **name** 或其他子属性，也不能对 `filter` 应用任何其他运算符或函数，例如 `ne`、`le` 和 `startswith()`。</span><span class="sxs-lookup"><span data-stu-id="c3d58-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="c3d58-127">有关 `$filter` 查询参数的一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c3d58-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3d58-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3d58-128">Request headers</span></span>
| <span data-ttu-id="c3d58-129">标头</span><span class="sxs-lookup"><span data-stu-id="c3d58-129">Header</span></span>       | <span data-ttu-id="c3d58-130">值</span><span class="sxs-lookup"><span data-stu-id="c3d58-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3d58-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3d58-131">Authorization</span></span>  | <span data-ttu-id="c3d58-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3d58-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3d58-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3d58-134">Request body</span></span>
<span data-ttu-id="c3d58-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c3d58-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3d58-136">响应</span><span class="sxs-lookup"><span data-stu-id="c3d58-136">Response</span></span>

<span data-ttu-id="c3d58-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[contact](../resources/contact.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c3d58-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3d58-138">示例</span><span class="sxs-lookup"><span data-stu-id="c3d58-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3d58-139">请求</span><span class="sxs-lookup"><span data-stu-id="c3d58-139">Request</span></span>
<span data-ttu-id="c3d58-140">下面的示例获取已登录用户的联系人的**displayName**和**emailAddresses**属性。</span><span class="sxs-lookup"><span data-stu-id="c3d58-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3d58-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c3d58-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3d58-142">C#</span><span class="sxs-lookup"><span data-stu-id="c3d58-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3d58-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3d58-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3d58-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="c3d58-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="c3d58-145">响应</span><span class="sxs-lookup"><span data-stu-id="c3d58-145">Response</span></span>
<span data-ttu-id="c3d58-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3d58-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts(displayName,emailAddresses)",
    "value":[
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
            "id":"AAMkADh6v5AAAvgTCFAAA=",
            "displayName":"Elvis Blank",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Elvis Blank",
                    "address":"elvisb@relecloud.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Elvis Blank",
                    "address":"elvisb@fabrikam.onmicrosoft.com"
                }
            ]
        },
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
            "id":"AAMkADh6v5AAAvgTCEAAA=",
            "displayName":"Pavel Bansky",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Pavel Bansky",
                    "address":"pavelb@contoso.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Pavel Bansky",
                    "address":"pavelb@fabrikam.onmicrosoft.com"
                }
            ]
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
