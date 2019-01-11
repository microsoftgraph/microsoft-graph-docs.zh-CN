---
title: 创建 educationUser
description: 新建用户。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 1636d137ae1a5b8938a59acf60a5eaae578e83f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892153"
---
# <a name="create-educationuser"></a><span data-ttu-id="62139-103">创建 educationUser</span><span class="sxs-lookup"><span data-stu-id="62139-103">Create educationUser</span></span>

> <span data-ttu-id="62139-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="62139-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62139-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="62139-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62139-106">新建用户。</span><span class="sxs-lookup"><span data-stu-id="62139-106">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="62139-107">权限</span><span class="sxs-lookup"><span data-stu-id="62139-107">Permissions</span></span>
<span data-ttu-id="62139-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62139-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62139-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="62139-110">Permission type</span></span>      | <span data-ttu-id="62139-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62139-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62139-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62139-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="62139-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="62139-113">Not supported.</span></span>  |
|<span data-ttu-id="62139-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62139-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="62139-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="62139-115">Not supported.</span></span>  |
|<span data-ttu-id="62139-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="62139-116">Application</span></span> | <span data-ttu-id="62139-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62139-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="62139-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62139-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="62139-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="62139-119">Request headers</span></span>
| <span data-ttu-id="62139-120">标头</span><span class="sxs-lookup"><span data-stu-id="62139-120">Header</span></span>       | <span data-ttu-id="62139-121">值</span><span class="sxs-lookup"><span data-stu-id="62139-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="62139-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62139-122">Authorization</span></span>  | <span data-ttu-id="62139-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62139-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62139-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62139-125">Content-Type</span></span>  | <span data-ttu-id="62139-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62139-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62139-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62139-127">Request body</span></span>
<span data-ttu-id="62139-128">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62139-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="62139-129">响应</span><span class="sxs-lookup"><span data-stu-id="62139-129">Response</span></span>
<span data-ttu-id="62139-130">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62139-130">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62139-131">示例</span><span class="sxs-lookup"><span data-stu-id="62139-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62139-132">请求</span><span class="sxs-lookup"><span data-stu-id="62139-132">Request</span></span>
<span data-ttu-id="62139-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62139-133">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="62139-134">响应</span><span class="sxs-lookup"><span data-stu-id="62139-134">Response</span></span>
<span data-ttu-id="62139-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62139-135">The following is an example of the response.</span></span> 

><span data-ttu-id="62139-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62139-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
