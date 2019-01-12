---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c4ec39584500da4e0aad8f04f03129302fbfd45b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965948"
---
# <a name="create-contact"></a><span data-ttu-id="12819-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="12819-103">Create Contact</span></span>

> <span data-ttu-id="12819-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12819-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12819-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12819-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12819-106">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="12819-106">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="12819-107">权限</span><span class="sxs-lookup"><span data-stu-id="12819-107">Permissions</span></span>
<span data-ttu-id="12819-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12819-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12819-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12819-110">Permission type</span></span>      | <span data-ttu-id="12819-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12819-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12819-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12819-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12819-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12819-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="12819-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12819-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12819-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12819-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="12819-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12819-116">Application</span></span> | <span data-ttu-id="12819-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12819-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="12819-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12819-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="12819-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12819-119">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="12819-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12819-120">Request headers</span></span>
| <span data-ttu-id="12819-121">标头</span><span class="sxs-lookup"><span data-stu-id="12819-121">Header</span></span>       | <span data-ttu-id="12819-122">值</span><span class="sxs-lookup"><span data-stu-id="12819-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12819-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12819-123">Authorization</span></span>  | <span data-ttu-id="12819-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12819-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12819-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12819-126">Content-Type</span></span>  | <span data-ttu-id="12819-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="12819-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12819-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="12819-129">Request body</span></span>
<span data-ttu-id="12819-130">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12819-130">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12819-131">响应</span><span class="sxs-lookup"><span data-stu-id="12819-131">Response</span></span>

<span data-ttu-id="12819-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12819-132">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12819-133">示例</span><span class="sxs-lookup"><span data-stu-id="12819-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12819-134">请求</span><span class="sxs-lookup"><span data-stu-id="12819-134">Request</span></span>
<span data-ttu-id="12819-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12819-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="12819-136">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12819-136">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="12819-137">响应</span><span class="sxs-lookup"><span data-stu-id="12819-137">Response</span></span>
<span data-ttu-id="12819-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12819-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
