---
title: 列出成员
description: 检索参加课程的教师和学生。 请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2ff31d2c899a8406678a4bded7bd782e0d95803d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517584"
---
# <a name="list-members"></a><span data-ttu-id="76c61-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="76c61-104">List members</span></span>

<span data-ttu-id="76c61-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76c61-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76c61-106">检索参加课程的教师和学生。</span><span class="sxs-lookup"><span data-stu-id="76c61-106">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="76c61-107">请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。</span><span class="sxs-lookup"><span data-stu-id="76c61-107">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="76c61-108">权限</span><span class="sxs-lookup"><span data-stu-id="76c61-108">Permissions</span></span>
<span data-ttu-id="76c61-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76c61-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76c61-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="76c61-111">Permission type</span></span>      | <span data-ttu-id="76c61-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76c61-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76c61-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76c61-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="76c61-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="76c61-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="76c61-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76c61-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="76c61-116">不支持</span><span class="sxs-lookup"><span data-stu-id="76c61-116">Not supported</span></span>  |
|<span data-ttu-id="76c61-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="76c61-117">Application</span></span> | <span data-ttu-id="76c61-118">Eduroster.read.all，Eduroster.read.all，All + Member。 Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="76c61-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="76c61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76c61-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="76c61-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="76c61-120">Optional query parameters</span></span>
<span data-ttu-id="76c61-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76c61-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76c61-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="76c61-122">Request headers</span></span>
| <span data-ttu-id="76c61-123">标头</span><span class="sxs-lookup"><span data-stu-id="76c61-123">Header</span></span>       | <span data-ttu-id="76c61-124">值</span><span class="sxs-lookup"><span data-stu-id="76c61-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76c61-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="76c61-125">Authorization</span></span>  | <span data-ttu-id="76c61-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76c61-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76c61-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="76c61-128">Request body</span></span>
<span data-ttu-id="76c61-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76c61-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="76c61-130">响应</span><span class="sxs-lookup"><span data-stu-id="76c61-130">Response</span></span>
<span data-ttu-id="76c61-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="76c61-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76c61-132">示例</span><span class="sxs-lookup"><span data-stu-id="76c61-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76c61-133">请求</span><span class="sxs-lookup"><span data-stu-id="76c61-133">Request</span></span>
<span data-ttu-id="76c61-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76c61-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76c61-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="76c61-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="c"></a>[<span data-ttu-id="76c61-136">C#</span><span class="sxs-lookup"><span data-stu-id="76c61-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76c61-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76c61-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76c61-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76c61-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76c61-139">Java</span><span class="sxs-lookup"><span data-stu-id="76c61-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="76c61-140">响应</span><span class="sxs-lookup"><span data-stu-id="76c61-140">Response</span></span>
<span data-ttu-id="76c61-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76c61-141">The following is an example of the response.</span></span> 

><span data-ttu-id="76c61-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="76c61-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
