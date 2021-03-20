---
title: 列出学校
description: 检索教授该课程的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: db96137a067389ca9042cda971bf7ddf41f30e22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951595"
---
# <a name="list-schools"></a><span data-ttu-id="61477-103">列出学校</span><span class="sxs-lookup"><span data-stu-id="61477-103">List schools</span></span>

<span data-ttu-id="61477-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61477-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61477-105">检索教授该课程的学校列表。</span><span class="sxs-lookup"><span data-stu-id="61477-105">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="61477-106">权限</span><span class="sxs-lookup"><span data-stu-id="61477-106">Permissions</span></span>

<span data-ttu-id="61477-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61477-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="61477-109">Permission type</span></span>                        | <span data-ttu-id="61477-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61477-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="61477-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61477-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="61477-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="61477-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="61477-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61477-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61477-114">不支持</span><span class="sxs-lookup"><span data-stu-id="61477-114">Not supported</span></span>                               |
| <span data-ttu-id="61477-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="61477-115">Application</span></span>                            | <span data-ttu-id="61477-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61477-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61477-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61477-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61477-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="61477-118">Optional query parameters</span></span>

<span data-ttu-id="61477-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="61477-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61477-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="61477-120">Request headers</span></span>

| <span data-ttu-id="61477-121">标头</span><span class="sxs-lookup"><span data-stu-id="61477-121">Header</span></span>        | <span data-ttu-id="61477-122">值</span><span class="sxs-lookup"><span data-stu-id="61477-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="61477-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61477-123">Authorization</span></span> | <span data-ttu-id="61477-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61477-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61477-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="61477-126">Request body</span></span>

<span data-ttu-id="61477-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61477-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61477-128">响应</span><span class="sxs-lookup"><span data-stu-id="61477-128">Response</span></span>

<span data-ttu-id="61477-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="61477-129">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61477-130">示例</span><span class="sxs-lookup"><span data-stu-id="61477-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="61477-131">请求</span><span class="sxs-lookup"><span data-stu-id="61477-131">Request</span></span>

<span data-ttu-id="61477-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61477-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61477-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="61477-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11014/schools
```

# <a name="c"></a>[<span data-ttu-id="61477-134">C#</span><span class="sxs-lookup"><span data-stu-id="61477-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61477-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61477-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61477-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61477-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61477-137">Java</span><span class="sxs-lookup"><span data-stu-id="61477-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="61477-138">响应</span><span class="sxs-lookup"><span data-stu-id="61477-138">Response</span></span>

<span data-ttu-id="61477-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61477-139">The following is an example of the response.</span></span>

><span data-ttu-id="61477-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="61477-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10002",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
