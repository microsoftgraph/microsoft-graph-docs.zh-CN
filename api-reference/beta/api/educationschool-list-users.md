---
title: 列出 educationUsers
description: 检索学校中的用户列表。
author: mmast-msft
ms.openlocfilehash: 6e642792b8cb3d7463b13288b0ed95838590ec52
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336412"
---
# <a name="list-educationusers"></a><span data-ttu-id="8d84b-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="8d84b-103">List educationUsers</span></span>

> <span data-ttu-id="8d84b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d84b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d84b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d84b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d84b-106">检索学校中的用户列表。</span><span class="sxs-lookup"><span data-stu-id="8d84b-106">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d84b-107">权限</span><span class="sxs-lookup"><span data-stu-id="8d84b-107">Permissions</span></span>
<span data-ttu-id="8d84b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d84b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d84b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d84b-110">Permission type</span></span>      | <span data-ttu-id="8d84b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d84b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d84b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d84b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="8d84b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d84b-113">Not supported.</span></span>  |
|<span data-ttu-id="8d84b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d84b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8d84b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d84b-115">Not supported.</span></span>  |
|<span data-ttu-id="8d84b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d84b-116">Application</span></span> | <span data-ttu-id="8d84b-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d84b-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8d84b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d84b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d84b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d84b-119">Optional query parameters</span></span>
<span data-ttu-id="8d84b-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8d84b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d84b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d84b-121">Request headers</span></span>
| <span data-ttu-id="8d84b-122">标头</span><span class="sxs-lookup"><span data-stu-id="8d84b-122">Header</span></span>       | <span data-ttu-id="8d84b-123">值</span><span class="sxs-lookup"><span data-stu-id="8d84b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d84b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d84b-124">Authorization</span></span>  | <span data-ttu-id="8d84b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d84b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d84b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d84b-127">Request body</span></span>
<span data-ttu-id="8d84b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d84b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8d84b-129">响应</span><span class="sxs-lookup"><span data-stu-id="8d84b-129">Response</span></span>
<span data-ttu-id="8d84b-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="8d84b-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d84b-131">示例</span><span class="sxs-lookup"><span data-stu-id="8d84b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d84b-132">请求</span><span class="sxs-lookup"><span data-stu-id="8d84b-132">Request</span></span>
<span data-ttu-id="8d84b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d84b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="8d84b-134">响应</span><span class="sxs-lookup"><span data-stu-id="8d84b-134">Response</span></span>
<span data-ttu-id="8d84b-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8d84b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8d84b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d84b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
