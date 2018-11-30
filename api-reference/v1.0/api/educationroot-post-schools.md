---
title: 创建 educationSchool
description: 创建学校。
ms.openlocfilehash: c6be0d1b22b15e92c324b6a3c5c43c4c49894fc3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011158"
---
# <a name="create-educationschool"></a><span data-ttu-id="a3bc9-103">创建 educationSchool</span><span class="sxs-lookup"><span data-stu-id="a3bc9-103">Create educationSchool</span></span>

<span data-ttu-id="a3bc9-104">创建学校。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-104">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3bc9-105">权限</span><span class="sxs-lookup"><span data-stu-id="a3bc9-105">Permissions</span></span>
<span data-ttu-id="a3bc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3bc9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3bc9-108">Permission type</span></span>      | <span data-ttu-id="a3bc9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3bc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3bc9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3bc9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a3bc9-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-111">Not supported.</span></span>  |
|<span data-ttu-id="a3bc9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3bc9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a3bc9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-113">Not supported.</span></span>  |
|<span data-ttu-id="a3bc9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3bc9-114">Application</span></span> | <span data-ttu-id="a3bc9-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3bc9-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a3bc9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3bc9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="a3bc9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3bc9-117">Request headers</span></span>
| <span data-ttu-id="a3bc9-118">标头</span><span class="sxs-lookup"><span data-stu-id="a3bc9-118">Header</span></span>       | <span data-ttu-id="a3bc9-119">值</span><span class="sxs-lookup"><span data-stu-id="a3bc9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3bc9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3bc9-120">Authorization</span></span>  | <span data-ttu-id="a3bc9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3bc9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3bc9-123">Content-Type</span></span>  | <span data-ttu-id="a3bc9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3bc9-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3bc9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3bc9-125">Request body</span></span>
<span data-ttu-id="a3bc9-126">在请求正文中，提供 [educationSchool](../resources/educationschool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-126">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a3bc9-127">响应</span><span class="sxs-lookup"><span data-stu-id="a3bc9-127">Response</span></span>
<span data-ttu-id="a3bc9-128">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-128">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3bc9-129">示例</span><span class="sxs-lookup"><span data-stu-id="a3bc9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3bc9-130">请求</span><span class="sxs-lookup"><span data-stu-id="a3bc9-130">Request</span></span>
<span data-ttu-id="a3bc9-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-131">The following is an example of the request.</span></span>
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
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="a3bc9-132">响应</span><span class="sxs-lookup"><span data-stu-id="a3bc9-132">Response</span></span>
<span data-ttu-id="a3bc9-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-133">The following is an example of the response.</span></span> 

><span data-ttu-id="a3bc9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3bc9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "fax": "+1 (253) 555-0101",
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
  "tocPath": ""
}-->