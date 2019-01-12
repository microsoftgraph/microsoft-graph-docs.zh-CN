---
title: 列出联系人
description: 在登录用户的邮箱 (.../me/contacts)，或从指定的联系人文件夹，则获取所有联系人。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 50b83036d7b818e1ed1b94643bc472a7bc18ed11
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950800"
---
# <a name="list-contacts"></a><span data-ttu-id="4f5b7-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="4f5b7-103">List contacts</span></span>

> <span data-ttu-id="4f5b7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f5b7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f5b7-106">在登录用户的邮箱 (.../me/contacts)，或从指定的联系人文件夹，则获取所有联系人。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-106">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f5b7-107">权限</span><span class="sxs-lookup"><span data-stu-id="4f5b7-107">Permissions</span></span>
<span data-ttu-id="4f5b7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f5b7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f5b7-110">Permission type</span></span>      | <span data-ttu-id="4f5b7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f5b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f5b7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f5b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4f5b7-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f5b7-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4f5b7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f5b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f5b7-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f5b7-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4f5b7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f5b7-116">Application</span></span> | <span data-ttu-id="4f5b7-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f5b7-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f5b7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f5b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4f5b7-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4f5b7-119">Optional query parameters</span></span>
<span data-ttu-id="4f5b7-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4f5b7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f5b7-121">Request headers</span></span>
| <span data-ttu-id="4f5b7-122">名称</span><span class="sxs-lookup"><span data-stu-id="4f5b7-122">Name</span></span>       | <span data-ttu-id="4f5b7-123">类型</span><span class="sxs-lookup"><span data-stu-id="4f5b7-123">Type</span></span> | <span data-ttu-id="4f5b7-124">说明</span><span class="sxs-lookup"><span data-stu-id="4f5b7-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f5b7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f5b7-125">Authorization</span></span>  | <span data-ttu-id="4f5b7-126">string</span><span class="sxs-lookup"><span data-stu-id="4f5b7-126">string</span></span>  | <span data-ttu-id="4f5b7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f5b7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f5b7-129">Request body</span></span>
<span data-ttu-id="4f5b7-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f5b7-131">响应</span><span class="sxs-lookup"><span data-stu-id="4f5b7-131">Response</span></span>

<span data-ttu-id="4f5b7-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-132">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f5b7-133">示例</span><span class="sxs-lookup"><span data-stu-id="4f5b7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f5b7-134">请求</span><span class="sxs-lookup"><span data-stu-id="4f5b7-134">Request</span></span>
<span data-ttu-id="4f5b7-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="4f5b7-136">响应</span><span class="sxs-lookup"><span data-stu-id="4f5b7-136">Response</span></span>
<span data-ttu-id="4f5b7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f5b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "birthday": "2016-10-19T10:37:00Z",
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
