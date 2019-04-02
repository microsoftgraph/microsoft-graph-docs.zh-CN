---
title: 列出联系人
description: 获取用户邮箱中的联系人。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a1eaeac682f511bf9b895e06e6a19b3bc728a38c
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026008"
---
# <a name="list-contacts"></a><span data-ttu-id="09ef5-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="09ef5-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ef5-104">获取用户邮箱中的联系人。</span><span class="sxs-lookup"><span data-stu-id="09ef5-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="09ef5-105">在以下两种情况下, 应用可以在其他用户的 "联系人" 文件夹中获取联系人:</span><span class="sxs-lookup"><span data-stu-id="09ef5-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="09ef5-106">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="09ef5-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="09ef5-107">如果应用程序具有来自一个用户的相应委派权限, 而另一个用户与该用户共享了一个联系人文件夹, 或者, 已向该用户授予了对该用户的委派访问[权限](#permissions)。</span><span class="sxs-lookup"><span data-stu-id="09ef5-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="09ef5-108">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="09ef5-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="09ef5-109">权限</span><span class="sxs-lookup"><span data-stu-id="09ef5-109">Permissions</span></span>
<span data-ttu-id="09ef5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09ef5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09ef5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="09ef5-112">Permission type</span></span>      | <span data-ttu-id="09ef5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09ef5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09ef5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09ef5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="09ef5-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09ef5-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="09ef5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09ef5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ef5-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09ef5-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="09ef5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="09ef5-118">Application</span></span> | <span data-ttu-id="09ef5-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09ef5-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="09ef5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09ef5-120">HTTP request</span></span>

<span data-ttu-id="09ef5-121">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="09ef5-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="09ef5-122">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="09ef5-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09ef5-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="09ef5-123">Optional query parameters</span></span>
<span data-ttu-id="09ef5-124">您可以使用`$filter`查询参数根据其电子邮件地址筛选联系人:</span><span class="sxs-lookup"><span data-stu-id="09ef5-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="09ef5-125">请注意, 只能在`$filter`emailAddresses `any`集合中的`eq`实例的**address**子属性上使用、和运算符。 \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="09ef5-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="09ef5-126">也就是说, 不能对 emailAddresses 实例的**名称**或任何其他子属性进行筛选, 也不\*\*\*\* 能将任何其他运算符或函数`filter`应用于 ( `ne`如`le`、和`startswith()`)。</span><span class="sxs-lookup"><span data-stu-id="09ef5-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="09ef5-127">有关`$filter`查询参数的一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="09ef5-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="09ef5-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="09ef5-128">Request headers</span></span>
| <span data-ttu-id="09ef5-129">标头</span><span class="sxs-lookup"><span data-stu-id="09ef5-129">Header</span></span>       | <span data-ttu-id="09ef5-130">值</span><span class="sxs-lookup"><span data-stu-id="09ef5-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09ef5-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ef5-131">Authorization</span></span>  | <span data-ttu-id="09ef5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09ef5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09ef5-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="09ef5-134">Request body</span></span>
<span data-ttu-id="09ef5-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09ef5-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09ef5-136">响应</span><span class="sxs-lookup"><span data-stu-id="09ef5-136">Response</span></span>

<span data-ttu-id="09ef5-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[contact](../resources/contact.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="09ef5-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09ef5-138">示例</span><span class="sxs-lookup"><span data-stu-id="09ef5-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09ef5-139">请求</span><span class="sxs-lookup"><span data-stu-id="09ef5-139">Request</span></span>
<span data-ttu-id="09ef5-140">下面的示例获取已登录用户的联系人的**displayName**和**emailAddresses**属性。</span><span class="sxs-lookup"><span data-stu-id="09ef5-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="09ef5-141">响应</span><span class="sxs-lookup"><span data-stu-id="09ef5-141">Response</span></span>
<span data-ttu-id="09ef5-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09ef5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
