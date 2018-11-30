---
title: 列出用户
description: 检索 user 对象列表。 这些 user 对象将包含特定于教育的属性。
ms.openlocfilehash: 476741b04da049c019276f78b4842e9732ff9c29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042912"
---
# <a name="list-users"></a><span data-ttu-id="5da99-104">列出用户</span><span class="sxs-lookup"><span data-stu-id="5da99-104">List users</span></span>

> <span data-ttu-id="5da99-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5da99-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5da99-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5da99-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5da99-107">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="5da99-107">Retrieve a list of user objects.</span></span> <span data-ttu-id="5da99-108">这些 user 对象将包含特定于教育的属性。</span><span class="sxs-lookup"><span data-stu-id="5da99-108">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5da99-109">权限</span><span class="sxs-lookup"><span data-stu-id="5da99-109">Permissions</span></span>
<span data-ttu-id="5da99-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5da99-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5da99-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5da99-112">Permission type</span></span>      | <span data-ttu-id="5da99-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5da99-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5da99-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5da99-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="5da99-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5da99-115">Not supported.</span></span>  |
|<span data-ttu-id="5da99-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5da99-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5da99-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5da99-117">Not supported.</span></span>  |
|<span data-ttu-id="5da99-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5da99-118">Application</span></span> | <span data-ttu-id="5da99-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da99-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5da99-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5da99-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5da99-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5da99-121">Optional query parameters</span></span>
<span data-ttu-id="5da99-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5da99-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5da99-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5da99-123">Request headers</span></span>
| <span data-ttu-id="5da99-124">标头</span><span class="sxs-lookup"><span data-stu-id="5da99-124">Header</span></span>       | <span data-ttu-id="5da99-125">值</span><span class="sxs-lookup"><span data-stu-id="5da99-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5da99-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5da99-126">Authorization</span></span>  | <span data-ttu-id="5da99-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5da99-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5da99-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5da99-129">Request body</span></span>
<span data-ttu-id="5da99-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5da99-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5da99-131">响应</span><span class="sxs-lookup"><span data-stu-id="5da99-131">Response</span></span>
<span data-ttu-id="5da99-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5da99-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5da99-133">示例</span><span class="sxs-lookup"><span data-stu-id="5da99-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5da99-134">请求</span><span class="sxs-lookup"><span data-stu-id="5da99-134">Request</span></span>
<span data-ttu-id="5da99-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5da99-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/users
```
##### <a name="response"></a><span data-ttu-id="5da99-136">响应</span><span class="sxs-lookup"><span data-stu-id="5da99-136">Response</span></span>
<span data-ttu-id="5da99-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5da99-137">The following is an example of the response.</span></span> 

><span data-ttu-id="5da99-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5da99-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": null,
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
