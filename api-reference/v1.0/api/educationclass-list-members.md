---
title: 列出 educationClass 的成员
description: 检索参加课程的教师和学生。 请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eadc2f00fee83f3663ab983118f92ce84f8cc607
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232089"
---
# <a name="list-members-of-an-educationclass"></a><span data-ttu-id="aefc3-104">列出 educationClass 的成员</span><span class="sxs-lookup"><span data-stu-id="aefc3-104">List members of an educationClass</span></span>

<span data-ttu-id="aefc3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aefc3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aefc3-106">检索 [educationClass 的 educationUser](../resources/educationuser.md) [成员](../resources/educationclass.md)。</span><span class="sxs-lookup"><span data-stu-id="aefc3-106">Retrieves the [educationUser](../resources/educationuser.md) members of an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aefc3-107">权限</span><span class="sxs-lookup"><span data-stu-id="aefc3-107">Permissions</span></span>
<span data-ttu-id="aefc3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aefc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aefc3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aefc3-110">Permission type</span></span>                        | <span data-ttu-id="aefc3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aefc3-111">Permissions (from least to most privileged)</span></span>                         |
| :------------------------------------- | :------------------------------------------------------------------ |
| <span data-ttu-id="aefc3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aefc3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="aefc3-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="aefc3-113">EduRoster.ReadBasic</span></span>                                                 |
| <span data-ttu-id="aefc3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aefc3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aefc3-115">不支持</span><span class="sxs-lookup"><span data-stu-id="aefc3-115">Not supported</span></span>                                                       |
| <span data-ttu-id="aefc3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aefc3-116">Application</span></span>                            | <span data-ttu-id="aefc3-117">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="aefc3-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> |

> [!NOTE]
> <span data-ttu-id="aefc3-118">请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。</span><span class="sxs-lookup"><span data-stu-id="aefc3-118">Note that if the delegated token is used, members can only see information about their own classes.</span></span>

## <a name="http-request"></a><span data-ttu-id="aefc3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aefc3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aefc3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aefc3-120">Optional query parameters</span></span>

<span data-ttu-id="aefc3-121">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="aefc3-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="aefc3-122">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="aefc3-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="aefc3-123">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="aefc3-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="aefc3-124">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="aefc3-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aefc3-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="aefc3-125">Request headers</span></span>
| <span data-ttu-id="aefc3-126">标头</span><span class="sxs-lookup"><span data-stu-id="aefc3-126">Header</span></span>       | <span data-ttu-id="aefc3-127">值</span><span class="sxs-lookup"><span data-stu-id="aefc3-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aefc3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="aefc3-128">Authorization</span></span>  | <span data-ttu-id="aefc3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aefc3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aefc3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="aefc3-131">Request body</span></span>
<span data-ttu-id="aefc3-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aefc3-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="aefc3-133">响应</span><span class="sxs-lookup"><span data-stu-id="aefc3-133">Response</span></span>
<span data-ttu-id="aefc3-134">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="aefc3-134">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aefc3-135">示例</span><span class="sxs-lookup"><span data-stu-id="aefc3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aefc3-136">请求</span><span class="sxs-lookup"><span data-stu-id="aefc3-136">Request</span></span>
<span data-ttu-id="aefc3-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aefc3-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aefc3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="aefc3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="c"></a>[<span data-ttu-id="aefc3-139">C#</span><span class="sxs-lookup"><span data-stu-id="aefc3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aefc3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aefc3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aefc3-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aefc3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aefc3-142">Java</span><span class="sxs-lookup"><span data-stu-id="aefc3-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aefc3-143">响应</span><span class="sxs-lookup"><span data-stu-id="aefc3-143">Response</span></span>
<span data-ttu-id="aefc3-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aefc3-144">The following is an example of the response.</span></span> 

><span data-ttu-id="aefc3-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aefc3-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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
