---
title: 列出联系人
description: 从已登录用户的默认联系人文件夹中获取联系人集合。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3c648e753c3959d3b22072edbd4b796d0f8c154b
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026022"
---
# <a name="list-contacts"></a><span data-ttu-id="84189-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="84189-103">List contacts</span></span>

<span data-ttu-id="84189-104">从已登录用户的默认联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="84189-104">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>

<span data-ttu-id="84189-105">在以下两种情况下，应用可以获取其他用户的联系人文件夹中的联系人：</span><span class="sxs-lookup"><span data-stu-id="84189-105">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="84189-106">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="84189-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="84189-107">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="84189-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="84189-108">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="84189-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="84189-109">权限</span><span class="sxs-lookup"><span data-stu-id="84189-109">Permissions</span></span>
<span data-ttu-id="84189-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84189-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84189-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="84189-112">Permission type</span></span>      | <span data-ttu-id="84189-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84189-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84189-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84189-114">Delegated (work or school account)</span></span> | <span data-ttu-id="84189-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84189-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="84189-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84189-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84189-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84189-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="84189-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="84189-118">Application</span></span> | <span data-ttu-id="84189-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84189-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="84189-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84189-120">HTTP request</span></span>

<span data-ttu-id="84189-121">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="84189-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="84189-122">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="84189-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84189-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="84189-123">Optional query parameters</span></span>
<span data-ttu-id="84189-124">可以使用 `$filter` 查询参数根据联系人的电子邮件地址来筛选联系人：</span><span class="sxs-lookup"><span data-stu-id="84189-124">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="84189-125">请注意，可以仅针对 **emailAddresses** 集合的实例的 **address** 子属性使用 `$filter`、`any` 和 `eq` 运算符。</span><span class="sxs-lookup"><span data-stu-id="84189-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="84189-126">也就是说，不能筛选 **emailAddresses** 的实例的 **name** 或其他子属性，也不能对 `filter` 应用任何其他运算符或函数，例如 `ne`、`le` 和 `startswith()`。</span><span class="sxs-lookup"><span data-stu-id="84189-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="84189-127">有关 `$filter` 查询参数的一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="84189-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="84189-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="84189-128">Request headers</span></span>
| <span data-ttu-id="84189-129">标头</span><span class="sxs-lookup"><span data-stu-id="84189-129">Header</span></span>       | <span data-ttu-id="84189-130">值</span><span class="sxs-lookup"><span data-stu-id="84189-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84189-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="84189-131">Authorization</span></span>  | <span data-ttu-id="84189-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84189-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="84189-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84189-134">Content-Type</span></span>   | <span data-ttu-id="84189-135">application/json</span><span class="sxs-lookup"><span data-stu-id="84189-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84189-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="84189-136">Request body</span></span>
<span data-ttu-id="84189-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84189-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84189-138">响应</span><span class="sxs-lookup"><span data-stu-id="84189-138">Response</span></span>

<span data-ttu-id="84189-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="84189-139">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84189-140">示例</span><span class="sxs-lookup"><span data-stu-id="84189-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84189-141">请求</span><span class="sxs-lookup"><span data-stu-id="84189-141">Request</span></span>
<span data-ttu-id="84189-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84189-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="84189-143">响应</span><span class="sxs-lookup"><span data-stu-id="84189-143">Response</span></span>
<span data-ttu-id="84189-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84189-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
