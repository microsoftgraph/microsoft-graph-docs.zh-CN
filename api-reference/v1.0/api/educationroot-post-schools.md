---
title: 创建 educationSchool
description: 创建学校。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9f144c13bfb3973af96b10d78e69bb1c21ce09a7
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "37553953"
---
# <a name="create-educationschool"></a><span data-ttu-id="ae286-103">创建 educationSchool</span><span class="sxs-lookup"><span data-stu-id="ae286-103">Create educationSchool</span></span>

<span data-ttu-id="ae286-104">创建学校。</span><span class="sxs-lookup"><span data-stu-id="ae286-104">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae286-105">权限</span><span class="sxs-lookup"><span data-stu-id="ae286-105">Permissions</span></span>

<span data-ttu-id="ae286-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae286-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae286-108">Permission type</span></span>                        | <span data-ttu-id="ae286-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae286-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ae286-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae286-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae286-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae286-111">Not supported.</span></span>                              |
| <span data-ttu-id="ae286-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae286-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae286-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae286-113">Not supported.</span></span>                              |
| <span data-ttu-id="ae286-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae286-114">Application</span></span>                            | <span data-ttu-id="ae286-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae286-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="ae286-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae286-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="ae286-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae286-117">Request headers</span></span>

| <span data-ttu-id="ae286-118">标头</span><span class="sxs-lookup"><span data-stu-id="ae286-118">Header</span></span>        | <span data-ttu-id="ae286-119">值</span><span class="sxs-lookup"><span data-stu-id="ae286-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ae286-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae286-120">Authorization</span></span> | <span data-ttu-id="ae286-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae286-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae286-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae286-123">Content-Type</span></span>  | <span data-ttu-id="ae286-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ae286-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="ae286-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae286-125">Request body</span></span>

<span data-ttu-id="ae286-126">在请求正文中，提供 [educationSchool](../resources/educationschool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae286-126">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae286-127">响应</span><span class="sxs-lookup"><span data-stu-id="ae286-127">Response</span></span>

<span data-ttu-id="ae286-128">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae286-128">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae286-129">示例</span><span class="sxs-lookup"><span data-stu-id="ae286-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ae286-130">请求</span><span class="sxs-lookup"><span data-stu-id="ae286-130">Request</span></span>

<span data-ttu-id="ae286-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae286-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ae286-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae286-132">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-type: application/json
Content-length: 292

{
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
  "externalId": "10002",
  "phone": "+1 (253) 555-0102",
}
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="ae286-133">C#</span><span class="sxs-lookup"><span data-stu-id="ae286-133">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae286-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae286-134">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae286-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae286-135">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ae286-136">Java</span><span class="sxs-lookup"><span data-stu-id="ae286-136">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ae286-137">响应</span><span class="sxs-lookup"><span data-stu-id="ae286-137">Response</span></span>

<span data-ttu-id="ae286-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ae286-138">The following is an example of the response.</span></span>

><span data-ttu-id="ae286-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae286-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
