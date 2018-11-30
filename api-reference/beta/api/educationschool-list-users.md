---
title: 列出 educationUsers
description: 检索学校中的用户列表。
ms.openlocfilehash: 24bcf5b680cdb29684f9647bd3e9632b896594a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043646"
---
# <a name="list-educationusers"></a><span data-ttu-id="e1fa6-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="e1fa6-103">List educationUsers</span></span>

> <span data-ttu-id="e1fa6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1fa6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1fa6-106">检索学校中的用户列表。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-106">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1fa6-107">权限</span><span class="sxs-lookup"><span data-stu-id="e1fa6-107">Permissions</span></span>
<span data-ttu-id="e1fa6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1fa6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1fa6-110">Permission type</span></span>      | <span data-ttu-id="e1fa6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1fa6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1fa6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1fa6-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1fa6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-113">Not supported.</span></span>  |
|<span data-ttu-id="e1fa6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1fa6-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e1fa6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-115">Not supported.</span></span>  |
|<span data-ttu-id="e1fa6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1fa6-116">Application</span></span> | <span data-ttu-id="e1fa6-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fa6-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e1fa6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1fa6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e1fa6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e1fa6-119">Optional query parameters</span></span>
<span data-ttu-id="e1fa6-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1fa6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1fa6-121">Request headers</span></span>
| <span data-ttu-id="e1fa6-122">标头</span><span class="sxs-lookup"><span data-stu-id="e1fa6-122">Header</span></span>       | <span data-ttu-id="e1fa6-123">值</span><span class="sxs-lookup"><span data-stu-id="e1fa6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1fa6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1fa6-124">Authorization</span></span>  | <span data-ttu-id="e1fa6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1fa6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1fa6-127">Request body</span></span>
<span data-ttu-id="e1fa6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e1fa6-129">响应</span><span class="sxs-lookup"><span data-stu-id="e1fa6-129">Response</span></span>
<span data-ttu-id="e1fa6-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1fa6-131">示例</span><span class="sxs-lookup"><span data-stu-id="e1fa6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1fa6-132">请求</span><span class="sxs-lookup"><span data-stu-id="e1fa6-132">Request</span></span>
<span data-ttu-id="e1fa6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="e1fa6-134">响应</span><span class="sxs-lookup"><span data-stu-id="e1fa6-134">Response</span></span>
<span data-ttu-id="e1fa6-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-135">The following is an example of the response.</span></span> 

><span data-ttu-id="e1fa6-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e1fa6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "middleName": " ",
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
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
