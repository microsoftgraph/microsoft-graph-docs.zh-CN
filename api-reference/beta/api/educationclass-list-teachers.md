---
title: 列出教师
description: 检索课程的教师列表。 委派令牌必须是课程的成员才能获取教师列表。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: d8030f9d3adb61b678c4224205a7f9d1f6a36b5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878999"
---
# <a name="list-teachers"></a><span data-ttu-id="87db3-104">列出教师</span><span class="sxs-lookup"><span data-stu-id="87db3-104">List teachers</span></span>

> <span data-ttu-id="87db3-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="87db3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87db3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="87db3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87db3-107">检索课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="87db3-107">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="87db3-108">委派令牌必须是课程的成员才能获取教师列表。</span><span class="sxs-lookup"><span data-stu-id="87db3-108">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="87db3-109">权限</span><span class="sxs-lookup"><span data-stu-id="87db3-109">Permissions</span></span>
<span data-ttu-id="87db3-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87db3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87db3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="87db3-112">Permission type</span></span>      | <span data-ttu-id="87db3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87db3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87db3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87db3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="87db3-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="87db3-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="87db3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87db3-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="87db3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="87db3-117">Not supported.</span></span>  |
|<span data-ttu-id="87db3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="87db3-118">Application</span></span> | <span data-ttu-id="87db3-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87db3-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="87db3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87db3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87db3-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="87db3-121">Optional query parameters</span></span>
<span data-ttu-id="87db3-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="87db3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87db3-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="87db3-123">Request headers</span></span>
| <span data-ttu-id="87db3-124">标头</span><span class="sxs-lookup"><span data-stu-id="87db3-124">Header</span></span>       | <span data-ttu-id="87db3-125">值</span><span class="sxs-lookup"><span data-stu-id="87db3-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87db3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="87db3-126">Authorization</span></span>  | <span data-ttu-id="87db3-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87db3-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87db3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="87db3-129">Request body</span></span>
<span data-ttu-id="87db3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="87db3-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="87db3-131">响应</span><span class="sxs-lookup"><span data-stu-id="87db3-131">Response</span></span>
<span data-ttu-id="87db3-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="87db3-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87db3-133">示例</span><span class="sxs-lookup"><span data-stu-id="87db3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87db3-134">请求</span><span class="sxs-lookup"><span data-stu-id="87db3-134">Request</span></span>
<span data-ttu-id="87db3-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="87db3-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023/teachers
```
##### <a name="response"></a><span data-ttu-id="87db3-136">响应</span><span class="sxs-lookup"><span data-stu-id="87db3-136">Response</span></span>
<span data-ttu-id="87db3-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="87db3-137">The following is an example of the response.</span></span> 

><span data-ttu-id="87db3-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="87db3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
