---
title: 列出联系人
description: 获取用户的邮箱中的联系人。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b427be9872aff70ecf5ed3166e94a48b94a62ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953628"
---
# <a name="list-contacts"></a><span data-ttu-id="bc392-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="bc392-103">List contacts</span></span>

> <span data-ttu-id="bc392-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc392-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc392-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc392-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc392-106">获取用户的邮箱中的联系人。</span><span class="sxs-lookup"><span data-stu-id="bc392-106">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="bc392-107">有两种方案，其中应用程序可在另一个用户的联系人文件夹中获取联系人：</span><span class="sxs-lookup"><span data-stu-id="bc392-107">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="bc392-108">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="bc392-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="bc392-109">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享联系人文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="bc392-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="bc392-110">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="bc392-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="bc392-111">权限</span><span class="sxs-lookup"><span data-stu-id="bc392-111">Permissions</span></span>
<span data-ttu-id="bc392-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc392-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc392-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc392-114">Permission type</span></span>      | <span data-ttu-id="bc392-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc392-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc392-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc392-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bc392-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc392-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bc392-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc392-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc392-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc392-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bc392-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc392-120">Application</span></span> | <span data-ttu-id="bc392-121">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc392-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc392-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc392-122">HTTP request</span></span>

<span data-ttu-id="bc392-123">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="bc392-123">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="bc392-124">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="bc392-124">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc392-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc392-125">Optional query parameters</span></span>
<span data-ttu-id="bc392-126">您可以使用`$filter`筛选器的联系人的查询参数基于其电子邮件地址：</span><span class="sxs-lookup"><span data-stu-id="bc392-126">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="bc392-127">请注意，您可以使用`$filter`， `any`，和`eq`仅子的**address**属性**emailAddresses**集合中的实例上的运算符。</span><span class="sxs-lookup"><span data-stu-id="bc392-127">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="bc392-128">即您不能筛选所依据的**名称**或任何其他子属性的实例**emailAddresses**，也可以应用任何其他运算符或运行`filter`，如`ne`， `le`，和`startswith()`。</span><span class="sxs-lookup"><span data-stu-id="bc392-128">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="bc392-129">有关一般信息`$filter`查询参数，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bc392-129">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc392-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc392-130">Request headers</span></span>
| <span data-ttu-id="bc392-131">标头</span><span class="sxs-lookup"><span data-stu-id="bc392-131">Header</span></span>       | <span data-ttu-id="bc392-132">值</span><span class="sxs-lookup"><span data-stu-id="bc392-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc392-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc392-133">Authorization</span></span>  | <span data-ttu-id="bc392-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc392-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc392-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc392-136">Request body</span></span>
<span data-ttu-id="bc392-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc392-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc392-138">响应</span><span class="sxs-lookup"><span data-stu-id="bc392-138">Response</span></span>

<span data-ttu-id="bc392-139">如果成功，此方法返回`200 OK`响应代码和响应正文中的[联系人](../resources/contact.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="bc392-139">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc392-140">示例</span><span class="sxs-lookup"><span data-stu-id="bc392-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc392-141">请求</span><span class="sxs-lookup"><span data-stu-id="bc392-141">Request</span></span>
<span data-ttu-id="bc392-142">下面的示例获取已登录的用户的联系人的**displayName**和**emailAddresses**属性。</span><span class="sxs-lookup"><span data-stu-id="bc392-142">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="bc392-143">响应</span><span class="sxs-lookup"><span data-stu-id="bc392-143">Response</span></span>
<span data-ttu-id="bc392-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc392-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
