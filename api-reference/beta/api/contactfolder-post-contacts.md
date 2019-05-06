---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ba4e0022913ca0173eb3f0c6390dd8ec0ddeae64
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591264"
---
# <a name="create-contact"></a><span data-ttu-id="4dd34-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="4dd34-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dd34-104">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="4dd34-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4dd34-105">权限</span><span class="sxs-lookup"><span data-stu-id="4dd34-105">Permissions</span></span>
<span data-ttu-id="4dd34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dd34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dd34-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dd34-108">Permission type</span></span>      | <span data-ttu-id="4dd34-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4dd34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dd34-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd34-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4dd34-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dd34-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4dd34-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dd34-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dd34-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4dd34-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dd34-114">Application</span></span> | <span data-ttu-id="4dd34-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dd34-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dd34-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dd34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="4dd34-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dd34-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="4dd34-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dd34-118">Request headers</span></span>
| <span data-ttu-id="4dd34-119">标头</span><span class="sxs-lookup"><span data-stu-id="4dd34-119">Header</span></span>       | <span data-ttu-id="4dd34-120">值</span><span class="sxs-lookup"><span data-stu-id="4dd34-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4dd34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dd34-121">Authorization</span></span>  | <span data-ttu-id="4dd34-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4dd34-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4dd34-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4dd34-124">Content-Type</span></span>  | <span data-ttu-id="4dd34-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4dd34-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4dd34-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dd34-127">Request body</span></span>
<span data-ttu-id="4dd34-128">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dd34-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4dd34-129">响应</span><span class="sxs-lookup"><span data-stu-id="4dd34-129">Response</span></span>

<span data-ttu-id="4dd34-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dd34-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dd34-131">示例</span><span class="sxs-lookup"><span data-stu-id="4dd34-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4dd34-132">请求</span><span class="sxs-lookup"><span data-stu-id="4dd34-132">Request</span></span>
<span data-ttu-id="4dd34-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4dd34-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="4dd34-134">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dd34-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4dd34-135">响应</span><span class="sxs-lookup"><span data-stu-id="4dd34-135">Response</span></span>
<span data-ttu-id="4dd34-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dd34-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4dd34-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4dd34-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4dd34-140">语言</span><span class="sxs-lookup"><span data-stu-id="4dd34-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4dd34-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="4dd34-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
