---
title: 获取 educationUser
description: 检索用户的属性和关系。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 64b31bec8b940893c425c507bdff2af93cacc4c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33321968"
---
# <a name="get-educationuser"></a><span data-ttu-id="b26e5-103">获取 educationUser</span><span class="sxs-lookup"><span data-stu-id="b26e5-103">Get educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b26e5-104">检索用户的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b26e5-104">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b26e5-105">权限</span><span class="sxs-lookup"><span data-stu-id="b26e5-105">Permissions</span></span>
<span data-ttu-id="b26e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b26e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b26e5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b26e5-108">Permission type</span></span>      | <span data-ttu-id="b26e5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b26e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b26e5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b26e5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b26e5-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b26e5-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b26e5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b26e5-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b26e5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b26e5-113">Not supported.</span></span>  |
|<span data-ttu-id="b26e5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b26e5-114">Application</span></span> | <span data-ttu-id="b26e5-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b26e5-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="b26e5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b26e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b26e5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b26e5-117">Optional query parameters</span></span>
<span data-ttu-id="b26e5-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b26e5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b26e5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b26e5-119">Request headers</span></span>
| <span data-ttu-id="b26e5-120">标头</span><span class="sxs-lookup"><span data-stu-id="b26e5-120">Header</span></span>       | <span data-ttu-id="b26e5-121">值</span><span class="sxs-lookup"><span data-stu-id="b26e5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b26e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b26e5-122">Authorization</span></span>  | <span data-ttu-id="b26e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b26e5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b26e5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b26e5-125">Request body</span></span>
<span data-ttu-id="b26e5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b26e5-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b26e5-127">响应</span><span class="sxs-lookup"><span data-stu-id="b26e5-127">Response</span></span>
<span data-ttu-id="b26e5-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b26e5-128">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b26e5-129">示例</span><span class="sxs-lookup"><span data-stu-id="b26e5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b26e5-130">请求</span><span class="sxs-lookup"><span data-stu-id="b26e5-130">Request</span></span>
<span data-ttu-id="b26e5-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b26e5-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/beta/education/users/13012
```
##### <a name="response"></a><span data-ttu-id="b26e5-132">响应</span><span class="sxs-lookup"><span data-stu-id="b26e5-132">Response</span></span>
<span data-ttu-id="b26e5-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b26e5-133">The following is an example of the response.</span></span> 

><span data-ttu-id="b26e5-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b26e5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
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
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
