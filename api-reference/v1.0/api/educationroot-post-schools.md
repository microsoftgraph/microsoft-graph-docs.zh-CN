---
title: 创建 educationSchool
description: 创建学校。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1f3c35e04dddaa5f9b1e8e22ec5173d553f3332f
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345749"
---
# <a name="create-educationschool"></a><span data-ttu-id="4c8e3-103">创建 educationSchool</span><span class="sxs-lookup"><span data-stu-id="4c8e3-103">Create educationSchool</span></span>

<span data-ttu-id="4c8e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c8e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c8e3-105">创建学校。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-105">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c8e3-106">权限</span><span class="sxs-lookup"><span data-stu-id="4c8e3-106">Permissions</span></span>

<span data-ttu-id="4c8e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c8e3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c8e3-109">Permission type</span></span>                        | <span data-ttu-id="4c8e3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c8e3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4c8e3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c8e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c8e3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-112">Not supported.</span></span>                              |
| <span data-ttu-id="4c8e3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c8e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c8e3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-114">Not supported.</span></span>                              |
| <span data-ttu-id="4c8e3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c8e3-115">Application</span></span>                            | <span data-ttu-id="4c8e3-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c8e3-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="4c8e3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c8e3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="4c8e3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c8e3-118">Request headers</span></span>

| <span data-ttu-id="4c8e3-119">标头</span><span class="sxs-lookup"><span data-stu-id="4c8e3-119">Header</span></span>        | <span data-ttu-id="4c8e3-120">值</span><span class="sxs-lookup"><span data-stu-id="4c8e3-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="4c8e3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c8e3-121">Authorization</span></span> | <span data-ttu-id="4c8e3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c8e3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c8e3-124">Content-Type</span></span>  | <span data-ttu-id="4c8e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c8e3-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="4c8e3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c8e3-126">Request body</span></span>

<span data-ttu-id="4c8e3-127">在请求正文中，提供 [educationSchool](../resources/educationschool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-127">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4c8e3-128">响应</span><span class="sxs-lookup"><span data-stu-id="4c8e3-128">Response</span></span>

<span data-ttu-id="4c8e3-129">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-129">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c8e3-130">示例</span><span class="sxs-lookup"><span data-stu-id="4c8e3-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4c8e3-131">请求</span><span class="sxs-lookup"><span data-stu-id="4c8e3-131">Request</span></span>

<span data-ttu-id="4c8e3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c8e3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c8e3-133">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="4c8e3-134">C#</span><span class="sxs-lookup"><span data-stu-id="4c8e3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c8e3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c8e3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c8e3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c8e3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c8e3-137">Java</span><span class="sxs-lookup"><span data-stu-id="4c8e3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c8e3-138">响应</span><span class="sxs-lookup"><span data-stu-id="4c8e3-138">Response</span></span>

<span data-ttu-id="4c8e3-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-139">The following is an example of the response.</span></span>

><span data-ttu-id="4c8e3-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4c8e3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
