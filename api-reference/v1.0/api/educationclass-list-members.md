---
title: 列出成员
description: 检索参加课程的教师和学生。 请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: db7013f2f98c9e36220a022a8ad5b3ea9f7c269f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370443"
---
# <a name="list-members"></a><span data-ttu-id="a4324-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="a4324-104">List members</span></span>

<span data-ttu-id="a4324-105">检索参加课程的教师和学生。</span><span class="sxs-lookup"><span data-stu-id="a4324-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="a4324-106">请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。</span><span class="sxs-lookup"><span data-stu-id="a4324-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4324-107">权限</span><span class="sxs-lookup"><span data-stu-id="a4324-107">Permissions</span></span>
<span data-ttu-id="a4324-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4324-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4324-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4324-110">Permission type</span></span>      | <span data-ttu-id="a4324-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4324-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4324-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4324-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a4324-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a4324-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a4324-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4324-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a4324-115">不支持</span><span class="sxs-lookup"><span data-stu-id="a4324-115">Not supported</span></span>  |
|<span data-ttu-id="a4324-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4324-116">Application</span></span> | <span data-ttu-id="a4324-117">Eduroster.read.all, Eduroster.read.all, All + Member。 Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="a4324-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a4324-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4324-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4324-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4324-119">Optional query parameters</span></span>
<span data-ttu-id="a4324-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4324-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4324-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4324-121">Request headers</span></span>
| <span data-ttu-id="a4324-122">标头</span><span class="sxs-lookup"><span data-stu-id="a4324-122">Header</span></span>       | <span data-ttu-id="a4324-123">值</span><span class="sxs-lookup"><span data-stu-id="a4324-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4324-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4324-124">Authorization</span></span>  | <span data-ttu-id="a4324-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4324-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4324-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4324-127">Request body</span></span>
<span data-ttu-id="a4324-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4324-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a4324-129">响应</span><span class="sxs-lookup"><span data-stu-id="a4324-129">Response</span></span>
<span data-ttu-id="a4324-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a4324-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a4324-131">示例</span><span class="sxs-lookup"><span data-stu-id="a4324-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4324-132">请求</span><span class="sxs-lookup"><span data-stu-id="a4324-132">Request</span></span>
<span data-ttu-id="a4324-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a4324-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4324-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a4324-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4324-135">C#</span><span class="sxs-lookup"><span data-stu-id="a4324-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4324-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4324-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4324-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="a4324-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4324-138">Java</span><span class="sxs-lookup"><span data-stu-id="a4324-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a4324-139">响应</span><span class="sxs-lookup"><span data-stu-id="a4324-139">Response</span></span>
<span data-ttu-id="a4324-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a4324-140">The following is an example of the response.</span></span> 

><span data-ttu-id="a4324-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a4324-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
