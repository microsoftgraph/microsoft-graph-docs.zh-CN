---
title: 列出学校
description: 检索用户所在的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 594a38d82de173d3a6a93607fdac61cca60e7cac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508564"
---
# <a name="list-schools"></a><span data-ttu-id="0ef20-103">列出学校</span><span class="sxs-lookup"><span data-stu-id="0ef20-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ef20-104">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="0ef20-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="0ef20-105">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="0ef20-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="0ef20-106">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="0ef20-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ef20-107">权限</span><span class="sxs-lookup"><span data-stu-id="0ef20-107">Permissions</span></span>
<span data-ttu-id="0ef20-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ef20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ef20-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ef20-110">Permission type</span></span>      | <span data-ttu-id="0ef20-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ef20-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ef20-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ef20-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0ef20-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="0ef20-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="0ef20-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ef20-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0ef20-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ef20-115">Not supported.</span></span>  |
|<span data-ttu-id="0ef20-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ef20-116">Application</span></span> | <span data-ttu-id="0ef20-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ef20-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0ef20-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ef20-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ef20-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ef20-119">Optional query parameters</span></span>
<span data-ttu-id="0ef20-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ef20-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ef20-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ef20-121">Request headers</span></span>
| <span data-ttu-id="0ef20-122">标头</span><span class="sxs-lookup"><span data-stu-id="0ef20-122">Header</span></span>       | <span data-ttu-id="0ef20-123">值</span><span class="sxs-lookup"><span data-stu-id="0ef20-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ef20-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ef20-124">Authorization</span></span>  | <span data-ttu-id="0ef20-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ef20-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ef20-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ef20-127">Request body</span></span>
<span data-ttu-id="0ef20-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ef20-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0ef20-129">响应</span><span class="sxs-lookup"><span data-stu-id="0ef20-129">Response</span></span>
<span data-ttu-id="0ef20-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0ef20-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ef20-131">示例</span><span class="sxs-lookup"><span data-stu-id="0ef20-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ef20-132">请求</span><span class="sxs-lookup"><span data-stu-id="0ef20-132">Request</span></span>
<span data-ttu-id="0ef20-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ef20-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="0ef20-134">响应</span><span class="sxs-lookup"><span data-stu-id="0ef20-134">Response</span></span>
<span data-ttu-id="0ef20-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ef20-135">The following is an example of the response.</span></span> 

><span data-ttu-id="0ef20-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0ef20-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
