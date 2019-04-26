---
title: 列出 educationUsers
description: 检索学校中的用户列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1889dfd19ab5ef461cccff5a2dc0103fce79cb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550271"
---
# <a name="list-educationusers"></a><span data-ttu-id="59c95-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="59c95-103">List educationUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59c95-104">检索学校中的用户列表。</span><span class="sxs-lookup"><span data-stu-id="59c95-104">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="59c95-105">权限</span><span class="sxs-lookup"><span data-stu-id="59c95-105">Permissions</span></span>
<span data-ttu-id="59c95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59c95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59c95-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="59c95-108">Permission type</span></span>      | <span data-ttu-id="59c95-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59c95-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59c95-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59c95-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="59c95-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="59c95-111">Not supported.</span></span>  |
|<span data-ttu-id="59c95-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59c95-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="59c95-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="59c95-113">Not supported.</span></span>  |
|<span data-ttu-id="59c95-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="59c95-114">Application</span></span> | <span data-ttu-id="59c95-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c95-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="59c95-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59c95-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59c95-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59c95-117">Optional query parameters</span></span>
<span data-ttu-id="59c95-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59c95-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59c95-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59c95-119">Request headers</span></span>
| <span data-ttu-id="59c95-120">标头</span><span class="sxs-lookup"><span data-stu-id="59c95-120">Header</span></span>       | <span data-ttu-id="59c95-121">值</span><span class="sxs-lookup"><span data-stu-id="59c95-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59c95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59c95-122">Authorization</span></span>  | <span data-ttu-id="59c95-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59c95-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59c95-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="59c95-125">Request body</span></span>
<span data-ttu-id="59c95-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59c95-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="59c95-127">响应</span><span class="sxs-lookup"><span data-stu-id="59c95-127">Response</span></span>
<span data-ttu-id="59c95-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="59c95-128">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59c95-129">示例</span><span class="sxs-lookup"><span data-stu-id="59c95-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59c95-130">请求</span><span class="sxs-lookup"><span data-stu-id="59c95-130">Request</span></span>
<span data-ttu-id="59c95-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59c95-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="59c95-132">响应</span><span class="sxs-lookup"><span data-stu-id="59c95-132">Response</span></span>
<span data-ttu-id="59c95-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="59c95-133">The following is an example of the response.</span></span> 

><span data-ttu-id="59c95-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="59c95-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
