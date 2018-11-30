---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
ms.openlocfilehash: dea355a848b2df1715f02c5042d31221ae3e49b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008478"
---
# <a name="create-contact"></a><span data-ttu-id="7afc9-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="7afc9-103">Create Contact</span></span>

<span data-ttu-id="7afc9-104">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="7afc9-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7afc9-105">权限</span><span class="sxs-lookup"><span data-stu-id="7afc9-105">Permissions</span></span>
<span data-ttu-id="7afc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7afc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7afc9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7afc9-108">Permission type</span></span>      | <span data-ttu-id="7afc9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7afc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7afc9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7afc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7afc9-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7afc9-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7afc9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7afc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7afc9-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7afc9-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7afc9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7afc9-114">Application</span></span> | <span data-ttu-id="7afc9-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7afc9-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7afc9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7afc9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="7afc9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7afc9-117">Request headers</span></span>
| <span data-ttu-id="7afc9-118">标头</span><span class="sxs-lookup"><span data-stu-id="7afc9-118">Header</span></span>       | <span data-ttu-id="7afc9-119">值</span><span class="sxs-lookup"><span data-stu-id="7afc9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7afc9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7afc9-120">Authorization</span></span>  | <span data-ttu-id="7afc9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7afc9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7afc9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7afc9-123">Content-Type</span></span>  | <span data-ttu-id="7afc9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7afc9-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7afc9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7afc9-125">Request body</span></span>
<span data-ttu-id="7afc9-126">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7afc9-126">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7afc9-127">响应</span><span class="sxs-lookup"><span data-stu-id="7afc9-127">Response</span></span>

<span data-ttu-id="7afc9-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7afc9-128">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7afc9-129">示例</span><span class="sxs-lookup"><span data-stu-id="7afc9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7afc9-130">请求</span><span class="sxs-lookup"><span data-stu-id="7afc9-130">Request</span></span>
<span data-ttu-id="7afc9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7afc9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
<span data-ttu-id="7afc9-132">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7afc9-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="7afc9-133">响应</span><span class="sxs-lookup"><span data-stu-id="7afc9-133">Response</span></span>
<span data-ttu-id="7afc9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7afc9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
