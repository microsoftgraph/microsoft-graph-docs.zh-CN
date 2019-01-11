---
title: 列出教师
description: 检索课程的教师列表。 委派令牌必须是课程的成员才能获取教师列表。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 57210efa64228d3643507ea4cfc1529be84810c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860492"
---
# <a name="list-teachers"></a><span data-ttu-id="a0744-104">列出教师</span><span class="sxs-lookup"><span data-stu-id="a0744-104">List teachers</span></span>

<span data-ttu-id="a0744-105">检索课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="a0744-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="a0744-106">委派令牌必须是课程的成员才能获取教师列表。</span><span class="sxs-lookup"><span data-stu-id="a0744-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0744-107">权限</span><span class="sxs-lookup"><span data-stu-id="a0744-107">Permissions</span></span>
<span data-ttu-id="a0744-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0744-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0744-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0744-110">Permission type</span></span>      | <span data-ttu-id="a0744-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0744-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0744-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0744-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a0744-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a0744-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a0744-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0744-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="a0744-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0744-115">Not supported.</span></span>  |
|<span data-ttu-id="a0744-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0744-116">Application</span></span> | <span data-ttu-id="a0744-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0744-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a0744-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0744-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0744-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0744-119">Optional query parameters</span></span>
<span data-ttu-id="a0744-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0744-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0744-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0744-121">Request headers</span></span>
| <span data-ttu-id="a0744-122">标头</span><span class="sxs-lookup"><span data-stu-id="a0744-122">Header</span></span>       | <span data-ttu-id="a0744-123">值</span><span class="sxs-lookup"><span data-stu-id="a0744-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0744-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0744-124">Authorization</span></span>  | <span data-ttu-id="a0744-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0744-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0744-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0744-127">Request body</span></span>
<span data-ttu-id="a0744-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0744-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a0744-129">响应</span><span class="sxs-lookup"><span data-stu-id="a0744-129">Response</span></span>
<span data-ttu-id="a0744-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a0744-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0744-131">示例</span><span class="sxs-lookup"><span data-stu-id="a0744-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0744-132">请求</span><span class="sxs-lookup"><span data-stu-id="a0744-132">Request</span></span>
<span data-ttu-id="a0744-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0744-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
##### <a name="response"></a><span data-ttu-id="a0744-134">响应</span><span class="sxs-lookup"><span data-stu-id="a0744-134">Response</span></span>
<span data-ttu-id="a0744-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0744-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a0744-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0744-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
