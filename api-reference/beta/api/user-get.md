---
title: 获取用户
description: 检索用户对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: cf517326c32a964617e12264079a94ce441413e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815013"
---
# <a name="get-a-user"></a><span data-ttu-id="cb5a4-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="cb5a4-103">Get a user</span></span>

> <span data-ttu-id="cb5a4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb5a4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb5a4-106">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-106">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="cb5a4-107">由于**用户**资源支持[扩展](/graph/extensibility-overview)，您还可以使用`GET`操作来获取**用户**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-107">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb5a4-108">权限</span><span class="sxs-lookup"><span data-stu-id="cb5a4-108">Permissions</span></span>
<span data-ttu-id="cb5a4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb5a4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb5a4-111">Permission type</span></span>      | <span data-ttu-id="cb5a4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb5a4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb5a4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb5a4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cb5a4-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb5a4-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb5a4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb5a4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb5a4-116">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb5a4-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="cb5a4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb5a4-117">Application</span></span> | <span data-ttu-id="cb5a4-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5a4-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb5a4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb5a4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb5a4-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cb5a4-120">Optional query parameters</span></span>
<span data-ttu-id="cb5a4-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cb5a4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb5a4-122">Request headers</span></span>
| <span data-ttu-id="cb5a4-123">标头</span><span class="sxs-lookup"><span data-stu-id="cb5a4-123">Header</span></span>       | <span data-ttu-id="cb5a4-124">值</span><span class="sxs-lookup"><span data-stu-id="cb5a4-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="cb5a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb5a4-125">Authorization</span></span>  | <span data-ttu-id="cb5a4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cb5a4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb5a4-128">Content-Type</span></span>   | <span data-ttu-id="cb5a4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="cb5a4-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb5a4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb5a4-130">Request body</span></span>
<span data-ttu-id="cb5a4-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb5a4-132">响应</span><span class="sxs-lookup"><span data-stu-id="cb5a4-132">Response</span></span>

<span data-ttu-id="cb5a4-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb5a4-134">示例</span><span class="sxs-lookup"><span data-stu-id="cb5a4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb5a4-135">请求</span><span class="sxs-lookup"><span data-stu-id="cb5a4-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="cb5a4-136">响应</span><span class="sxs-lookup"><span data-stu-id="cb5a4-136">Response</span></span>
<span data-ttu-id="cb5a4-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-137">Here is an example of the response.</span></span> <span data-ttu-id="cb5a4-138">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-138">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="cb5a4-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="cb5a4-139">See also</span></span>

- [<span data-ttu-id="cb5a4-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="cb5a4-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cb5a4-141">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="cb5a4-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cb5a4-142">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="cb5a4-142">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
