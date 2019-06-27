---
title: 列出成员
description: 检索参加课程的教师和学生。 请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: dc446a12707af45f3851f1990f0c91d6394f5e7f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277887"
---
# <a name="list-members"></a><span data-ttu-id="4a30c-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="4a30c-104">List members</span></span>

<span data-ttu-id="4a30c-105">检索参加课程的教师和学生。</span><span class="sxs-lookup"><span data-stu-id="4a30c-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="4a30c-106">请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。</span><span class="sxs-lookup"><span data-stu-id="4a30c-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a30c-107">权限</span><span class="sxs-lookup"><span data-stu-id="4a30c-107">Permissions</span></span>
<span data-ttu-id="4a30c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a30c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a30c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a30c-110">Permission type</span></span>      | <span data-ttu-id="4a30c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a30c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a30c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a30c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a30c-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="4a30c-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="4a30c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a30c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4a30c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="4a30c-115">Not supported</span></span>  |
|<span data-ttu-id="4a30c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a30c-116">Application</span></span> | <span data-ttu-id="4a30c-117">Eduroster.read.all, Eduroster.read.all, All + Member。 Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="4a30c-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4a30c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a30c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a30c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a30c-119">Optional query parameters</span></span>
<span data-ttu-id="4a30c-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a30c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a30c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a30c-121">Request headers</span></span>
| <span data-ttu-id="4a30c-122">标头</span><span class="sxs-lookup"><span data-stu-id="4a30c-122">Header</span></span>       | <span data-ttu-id="4a30c-123">值</span><span class="sxs-lookup"><span data-stu-id="4a30c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a30c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a30c-124">Authorization</span></span>  | <span data-ttu-id="4a30c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a30c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a30c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a30c-127">Request body</span></span>
<span data-ttu-id="4a30c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a30c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4a30c-129">响应</span><span class="sxs-lookup"><span data-stu-id="4a30c-129">Response</span></span>
<span data-ttu-id="4a30c-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4a30c-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a30c-131">示例</span><span class="sxs-lookup"><span data-stu-id="4a30c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a30c-132">请求</span><span class="sxs-lookup"><span data-stu-id="4a30c-132">Request</span></span>
<span data-ttu-id="4a30c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4a30c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
##### <a name="response"></a><span data-ttu-id="4a30c-134">响应</span><span class="sxs-lookup"><span data-stu-id="4a30c-134">Response</span></span>
<span data-ttu-id="4a30c-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4a30c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="4a30c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4a30c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a30c-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4a30c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a30c-139">C#</span><span class="sxs-lookup"><span data-stu-id="4a30c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a30c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a30c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4a30c-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="4a30c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
