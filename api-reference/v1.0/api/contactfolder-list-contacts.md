---
title: 列出联系人
description: 从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或从指定的联系人文件夹中获取联系人集合。
localization_priority: Normal
ms.openlocfilehash: a617cae074ee467d0c47ffcc86351a5e4d65e45a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855466"
---
# <a name="list-contacts"></a><span data-ttu-id="b7f7a-103">列出联系人</span><span class="sxs-lookup"><span data-stu-id="b7f7a-103">List contacts</span></span>

<span data-ttu-id="b7f7a-104">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或从指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-104">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7f7a-105">权限</span><span class="sxs-lookup"><span data-stu-id="b7f7a-105">Permissions</span></span>
<span data-ttu-id="b7f7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f7a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7f7a-108">Permission type</span></span>      | <span data-ttu-id="b7f7a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7f7a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7f7a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7f7a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7f7a-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7f7a-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b7f7a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7f7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f7a-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7f7a-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b7f7a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7f7a-114">Application</span></span> | <span data-ttu-id="b7f7a-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7f7a-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7f7a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7f7a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7f7a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b7f7a-117">Optional query parameters</span></span>
<span data-ttu-id="b7f7a-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b7f7a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7f7a-119">Request headers</span></span>
| <span data-ttu-id="b7f7a-120">名称</span><span class="sxs-lookup"><span data-stu-id="b7f7a-120">Name</span></span>       | <span data-ttu-id="b7f7a-121">类型</span><span class="sxs-lookup"><span data-stu-id="b7f7a-121">Type</span></span> | <span data-ttu-id="b7f7a-122">说明</span><span class="sxs-lookup"><span data-stu-id="b7f7a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7f7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7f7a-123">Authorization</span></span>  | <span data-ttu-id="b7f7a-124">string</span><span class="sxs-lookup"><span data-stu-id="b7f7a-124">string</span></span>  | <span data-ttu-id="b7f7a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7f7a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7f7a-127">Request body</span></span>
<span data-ttu-id="b7f7a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7f7a-129">响应</span><span class="sxs-lookup"><span data-stu-id="b7f7a-129">Response</span></span>

<span data-ttu-id="b7f7a-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7f7a-131">示例</span><span class="sxs-lookup"><span data-stu-id="b7f7a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7f7a-132">请求</span><span class="sxs-lookup"><span data-stu-id="b7f7a-132">Request</span></span>
<span data-ttu-id="b7f7a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="b7f7a-134">响应</span><span class="sxs-lookup"><span data-stu-id="b7f7a-134">Response</span></span>
<span data-ttu-id="b7f7a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7f7a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
