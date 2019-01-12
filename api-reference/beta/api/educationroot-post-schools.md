---
title: 创建 educationSchool
description: 创建学校。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6fda4389c74b975eb1d6a622b153dfa4459f8870
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945473"
---
# <a name="create-educationschool"></a><span data-ttu-id="00e1a-103">创建 educationSchool</span><span class="sxs-lookup"><span data-stu-id="00e1a-103">Create educationSchool</span></span>

> <span data-ttu-id="00e1a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00e1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00e1a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00e1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00e1a-106">创建学校。</span><span class="sxs-lookup"><span data-stu-id="00e1a-106">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="00e1a-107">权限</span><span class="sxs-lookup"><span data-stu-id="00e1a-107">Permissions</span></span>
<span data-ttu-id="00e1a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00e1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00e1a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="00e1a-110">Permission type</span></span>      | <span data-ttu-id="00e1a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00e1a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00e1a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00e1a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="00e1a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="00e1a-113">Not supported.</span></span>  |
|<span data-ttu-id="00e1a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00e1a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="00e1a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00e1a-115">Not supported.</span></span>  |
|<span data-ttu-id="00e1a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="00e1a-116">Application</span></span> | <span data-ttu-id="00e1a-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e1a-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="00e1a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00e1a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="00e1a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="00e1a-119">Request headers</span></span>
| <span data-ttu-id="00e1a-120">标头</span><span class="sxs-lookup"><span data-stu-id="00e1a-120">Header</span></span>       | <span data-ttu-id="00e1a-121">值</span><span class="sxs-lookup"><span data-stu-id="00e1a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00e1a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00e1a-122">Authorization</span></span>  | <span data-ttu-id="00e1a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00e1a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="00e1a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00e1a-125">Content-Type</span></span>  | <span data-ttu-id="00e1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00e1a-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00e1a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="00e1a-127">Request body</span></span>
<span data-ttu-id="00e1a-128">在请求正文中，提供 [educationSchool](../resources/educationschool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00e1a-128">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="00e1a-129">响应</span><span class="sxs-lookup"><span data-stu-id="00e1a-129">Response</span></span>
<span data-ttu-id="00e1a-130">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00e1a-130">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00e1a-131">示例</span><span class="sxs-lookup"><span data-stu-id="00e1a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00e1a-132">请求</span><span class="sxs-lookup"><span data-stu-id="00e1a-132">Request</span></span>
<span data-ttu-id="00e1a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="00e1a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools
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

##### <a name="response"></a><span data-ttu-id="00e1a-134">响应</span><span class="sxs-lookup"><span data-stu-id="00e1a-134">Response</span></span>
<span data-ttu-id="00e1a-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="00e1a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="00e1a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="00e1a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
