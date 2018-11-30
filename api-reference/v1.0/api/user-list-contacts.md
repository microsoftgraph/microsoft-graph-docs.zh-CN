---
title: 列出联系人
description: 从已登录的用户默认联系人文件夹中获取联系人的集合。
ms.openlocfilehash: 296844eb4eea93c5bd46e8028f3423fe797142ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009822"
---
# <a name="list-contacts"></a><span data-ttu-id="fb887-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="fb887-103">List contacts</span></span>

<span data-ttu-id="fb887-104">从已登录的用户默认联系人文件夹中获取联系人的集合。</span><span class="sxs-lookup"><span data-stu-id="fb887-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="fb887-105">有两种方案，其中应用程序可在另一个用户的联系人文件夹中获取联系人：</span><span class="sxs-lookup"><span data-stu-id="fb887-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="fb887-106">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="fb887-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="fb887-107">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享联系人文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="fb887-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="fb887-108">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="fb887-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="fb887-109">权限</span><span class="sxs-lookup"><span data-stu-id="fb887-109">Permissions</span></span>
<span data-ttu-id="fb887-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb887-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb887-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb887-112">Permission type</span></span>      | <span data-ttu-id="fb887-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb887-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb887-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb887-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fb887-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb887-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fb887-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb887-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb887-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb887-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fb887-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb887-118">Application</span></span> | <span data-ttu-id="fb887-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb887-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb887-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb887-120">HTTP request</span></span>

<span data-ttu-id="fb887-121">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="fb887-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="fb887-122">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="fb887-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb887-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb887-123">Optional query parameters</span></span>
<span data-ttu-id="fb887-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb887-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="fb887-125">例如，你可以使用 `$filter` 查询参数根据联系人的电子邮件地址的域来过滤联系人：</span><span class="sxs-lookup"><span data-stu-id="fb887-125">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="fb887-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb887-126">Request headers</span></span>
| <span data-ttu-id="fb887-127">标头</span><span class="sxs-lookup"><span data-stu-id="fb887-127">Header</span></span>       | <span data-ttu-id="fb887-128">值</span><span class="sxs-lookup"><span data-stu-id="fb887-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb887-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb887-129">Authorization</span></span>  | <span data-ttu-id="fb887-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb887-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fb887-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb887-132">Content-Type</span></span>   | <span data-ttu-id="fb887-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fb887-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb887-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb887-134">Request body</span></span>
<span data-ttu-id="fb887-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb887-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb887-136">响应</span><span class="sxs-lookup"><span data-stu-id="fb887-136">Response</span></span>

<span data-ttu-id="fb887-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fb887-137">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb887-138">示例</span><span class="sxs-lookup"><span data-stu-id="fb887-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb887-139">请求</span><span class="sxs-lookup"><span data-stu-id="fb887-139">Request</span></span>
<span data-ttu-id="fb887-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb887-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="fb887-141">响应</span><span class="sxs-lookup"><span data-stu-id="fb887-141">Response</span></span>
<span data-ttu-id="fb887-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb887-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
