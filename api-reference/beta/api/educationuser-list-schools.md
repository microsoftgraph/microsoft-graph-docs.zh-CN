---
title: 列出学校
description: 检索用户所在的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1608ce9085bfcdb52cd781192e67714789780743
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980655"
---
# <a name="list-schools"></a><span data-ttu-id="3689b-103">列出学校</span><span class="sxs-lookup"><span data-stu-id="3689b-103">List schools</span></span>

> <span data-ttu-id="3689b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3689b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3689b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3689b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3689b-106">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="3689b-106">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="3689b-107">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="3689b-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="3689b-108">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="3689b-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="3689b-109">权限</span><span class="sxs-lookup"><span data-stu-id="3689b-109">Permissions</span></span>
<span data-ttu-id="3689b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3689b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3689b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3689b-112">Permission type</span></span>      | <span data-ttu-id="3689b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3689b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3689b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3689b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="3689b-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3689b-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="3689b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3689b-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3689b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3689b-117">Not supported.</span></span>  |
|<span data-ttu-id="3689b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3689b-118">Application</span></span> | <span data-ttu-id="3689b-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3689b-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3689b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3689b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3689b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3689b-121">Optional query parameters</span></span>
<span data-ttu-id="3689b-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3689b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3689b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3689b-123">Request headers</span></span>
| <span data-ttu-id="3689b-124">标头</span><span class="sxs-lookup"><span data-stu-id="3689b-124">Header</span></span>       | <span data-ttu-id="3689b-125">值</span><span class="sxs-lookup"><span data-stu-id="3689b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3689b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3689b-126">Authorization</span></span>  | <span data-ttu-id="3689b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3689b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3689b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3689b-129">Request body</span></span>
<span data-ttu-id="3689b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3689b-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3689b-131">响应</span><span class="sxs-lookup"><span data-stu-id="3689b-131">Response</span></span>
<span data-ttu-id="3689b-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="3689b-132">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3689b-133">示例</span><span class="sxs-lookup"><span data-stu-id="3689b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3689b-134">请求</span><span class="sxs-lookup"><span data-stu-id="3689b-134">Request</span></span>
<span data-ttu-id="3689b-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3689b-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="3689b-136">响应</span><span class="sxs-lookup"><span data-stu-id="3689b-136">Response</span></span>
<span data-ttu-id="3689b-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3689b-137">The following is an example of the response.</span></span> 

><span data-ttu-id="3689b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3689b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
