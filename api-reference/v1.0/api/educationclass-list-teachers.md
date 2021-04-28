---
title: 列出教师
description: 检索课程的教师列表。 委派令牌必须是课程的成员才能获取教师列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c1e3ca9fe9a82ca4590bf629065df15e6f809bb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051464"
---
# <a name="list-teachers"></a><span data-ttu-id="71f9d-104">列出教师</span><span class="sxs-lookup"><span data-stu-id="71f9d-104">List teachers</span></span>

<span data-ttu-id="71f9d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71f9d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71f9d-106">检索课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="71f9d-106">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="71f9d-107">委派令牌必须是课程的成员才能获取教师列表。</span><span class="sxs-lookup"><span data-stu-id="71f9d-107">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="71f9d-108">权限</span><span class="sxs-lookup"><span data-stu-id="71f9d-108">Permissions</span></span>
<span data-ttu-id="71f9d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71f9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71f9d-111">Permission type</span></span>      | <span data-ttu-id="71f9d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71f9d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71f9d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="71f9d-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="71f9d-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="71f9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71f9d-115">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="71f9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71f9d-116">Not supported.</span></span>  |
|<span data-ttu-id="71f9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="71f9d-117">Application</span></span> | <span data-ttu-id="71f9d-118">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f9d-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="71f9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71f9d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71f9d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="71f9d-120">Optional query parameters</span></span>
<span data-ttu-id="71f9d-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="71f9d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71f9d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="71f9d-122">Request headers</span></span>
| <span data-ttu-id="71f9d-123">标头</span><span class="sxs-lookup"><span data-stu-id="71f9d-123">Header</span></span>       | <span data-ttu-id="71f9d-124">值</span><span class="sxs-lookup"><span data-stu-id="71f9d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71f9d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="71f9d-125">Authorization</span></span>  | <span data-ttu-id="71f9d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71f9d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71f9d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="71f9d-128">Request body</span></span>
<span data-ttu-id="71f9d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71f9d-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71f9d-130">响应</span><span class="sxs-lookup"><span data-stu-id="71f9d-130">Response</span></span>
<span data-ttu-id="71f9d-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="71f9d-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71f9d-132">示例</span><span class="sxs-lookup"><span data-stu-id="71f9d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71f9d-133">请求</span><span class="sxs-lookup"><span data-stu-id="71f9d-133">Request</span></span>
<span data-ttu-id="71f9d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71f9d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71f9d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="71f9d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
# <a name="c"></a>[<span data-ttu-id="71f9d-136">C#</span><span class="sxs-lookup"><span data-stu-id="71f9d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teachers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71f9d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71f9d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teachers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71f9d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71f9d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teachers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71f9d-139">Java</span><span class="sxs-lookup"><span data-stu-id="71f9d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teachers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="71f9d-140">响应</span><span class="sxs-lookup"><span data-stu-id="71f9d-140">Response</span></span>
<span data-ttu-id="71f9d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71f9d-141">The following is an example of the response.</span></span> 

><span data-ttu-id="71f9d-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="71f9d-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
