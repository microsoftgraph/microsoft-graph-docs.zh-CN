---
title: 创建 educationUser
description: 新建用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 18ced2a58fa4974ddca18bfc5b31d3e5e39fb46c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043582"
---
# <a name="create-educationuser"></a><span data-ttu-id="e4e91-103">创建 educationUser</span><span class="sxs-lookup"><span data-stu-id="e4e91-103">Create educationUser</span></span>

<span data-ttu-id="e4e91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4e91-105">新建用户。</span><span class="sxs-lookup"><span data-stu-id="e4e91-105">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="e4e91-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4e91-106">Permissions</span></span>
<span data-ttu-id="e4e91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4e91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4e91-109">Permission type</span></span>      | <span data-ttu-id="e4e91-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4e91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4e91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e91-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e4e91-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4e91-112">Not supported.</span></span>  |
|<span data-ttu-id="e4e91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e91-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e4e91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4e91-114">Not supported.</span></span>  |
|<span data-ttu-id="e4e91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4e91-115">Application</span></span> | <span data-ttu-id="e4e91-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e91-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e4e91-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4e91-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="e4e91-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4e91-118">Request headers</span></span>
| <span data-ttu-id="e4e91-119">标头</span><span class="sxs-lookup"><span data-stu-id="e4e91-119">Header</span></span>       | <span data-ttu-id="e4e91-120">值</span><span class="sxs-lookup"><span data-stu-id="e4e91-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4e91-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4e91-121">Authorization</span></span>  | <span data-ttu-id="e4e91-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4e91-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4e91-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4e91-124">Content-Type</span></span>  | <span data-ttu-id="e4e91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4e91-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4e91-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4e91-126">Request body</span></span>
<span data-ttu-id="e4e91-127">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4e91-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e4e91-128">响应</span><span class="sxs-lookup"><span data-stu-id="e4e91-128">Response</span></span>
<span data-ttu-id="e4e91-129">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4e91-129">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e91-130">示例</span><span class="sxs-lookup"><span data-stu-id="e4e91-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4e91-131">请求</span><span class="sxs-lookup"><span data-stu-id="e4e91-131">Request</span></span>
<span data-ttu-id="e4e91-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e4e91-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4e91-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4e91-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/users
Content-type: application/json
Content-length: 508

{
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": null,
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e4e91-134">C#</span><span class="sxs-lookup"><span data-stu-id="e4e91-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4e91-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4e91-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4e91-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4e91-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4e91-137">Java</span><span class="sxs-lookup"><span data-stu-id="e4e91-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4e91-138">响应</span><span class="sxs-lookup"><span data-stu-id="e4e91-138">Response</span></span>
<span data-ttu-id="e4e91-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e4e91-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e4e91-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e4e91-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


