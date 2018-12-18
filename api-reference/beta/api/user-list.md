---
title: 列出用户
description: 检索 user 对象列表。
author: dkershaw10
ms.openlocfilehash: 6d80bde11d5370a87432394c191519bc9a1780ab
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361934"
---
# <a name="list-users"></a><span data-ttu-id="fba1f-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="fba1f-103">List users</span></span>

> <span data-ttu-id="fba1f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fba1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fba1f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fba1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fba1f-106">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="fba1f-106">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fba1f-107">权限</span><span class="sxs-lookup"><span data-stu-id="fba1f-107">Permissions</span></span>

<span data-ttu-id="fba1f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fba1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba1f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fba1f-110">Permission type</span></span>      | <span data-ttu-id="fba1f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fba1f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fba1f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fba1f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fba1f-113">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fba1f-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fba1f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fba1f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fba1f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fba1f-115">Not supported.</span></span>    |
|<span data-ttu-id="fba1f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fba1f-116">Application</span></span> | <span data-ttu-id="fba1f-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fba1f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fba1f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fba1f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fba1f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fba1f-119">Optional query parameters</span></span>

<span data-ttu-id="fba1f-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fba1f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fba1f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fba1f-121">Request headers</span></span>
| <span data-ttu-id="fba1f-122">标头</span><span class="sxs-lookup"><span data-stu-id="fba1f-122">Header</span></span>        | <span data-ttu-id="fba1f-123">值</span><span class="sxs-lookup"><span data-stu-id="fba1f-123">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="fba1f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fba1f-124">Authorization</span></span> | <span data-ttu-id="fba1f-125">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="fba1f-125">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="fba1f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fba1f-126">Content-Type</span></span>  | <span data-ttu-id="fba1f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fba1f-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="fba1f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fba1f-128">Request body</span></span>

<span data-ttu-id="fba1f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fba1f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fba1f-130">响应</span><span class="sxs-lookup"><span data-stu-id="fba1f-130">Response</span></span>

<span data-ttu-id="fba1f-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fba1f-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fba1f-132">示例</span><span class="sxs-lookup"><span data-stu-id="fba1f-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fba1f-133">请求</span><span class="sxs-lookup"><span data-stu-id="fba1f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="fba1f-134">响应</span><span class="sxs-lookup"><span data-stu-id="fba1f-134">Response</span></span>

<span data-ttu-id="fba1f-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fba1f-135">Here is an example of the response.</span></span> <span data-ttu-id="fba1f-136">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fba1f-136">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
