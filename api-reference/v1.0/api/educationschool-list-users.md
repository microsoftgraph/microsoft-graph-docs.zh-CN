---
title: 列出 educationSchool 的用户
description: 检索学校中的用户列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d37bec88be07f9dba3e91d44558508ce82004c74
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232002"
---
# <a name="list-users-of-an-educationschool"></a><span data-ttu-id="56ac2-103">列出 educationSchool 的用户</span><span class="sxs-lookup"><span data-stu-id="56ac2-103">List users of an educationSchool</span></span>

<span data-ttu-id="56ac2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56ac2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56ac2-105">获取与[educationSchool](../resources/educationschool.md)关联的[educationUser](../resources/educationuser.md)资源。</span><span class="sxs-lookup"><span data-stu-id="56ac2-105">Get the [educationUser](../resources/educationuser.md) resources associated with an [educationSchool](../resources/educationschool.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="56ac2-106">权限</span><span class="sxs-lookup"><span data-stu-id="56ac2-106">Permissions</span></span>

<span data-ttu-id="56ac2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56ac2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56ac2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="56ac2-109">Permission type</span></span>                        | <span data-ttu-id="56ac2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56ac2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="56ac2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56ac2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="56ac2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="56ac2-112">Not supported.</span></span>                              |
| <span data-ttu-id="56ac2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56ac2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56ac2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="56ac2-114">Not supported.</span></span>                              |
| <span data-ttu-id="56ac2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="56ac2-115">Application</span></span>                            | <span data-ttu-id="56ac2-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56ac2-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56ac2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56ac2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/{educationSchoolId}/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56ac2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56ac2-118">Optional query parameters</span></span>

<span data-ttu-id="56ac2-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="56ac2-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="56ac2-120">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="56ac2-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="56ac2-121">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="56ac2-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="56ac2-122">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="56ac2-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="56ac2-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="56ac2-123">Request headers</span></span>
| <span data-ttu-id="56ac2-124">标头</span><span class="sxs-lookup"><span data-stu-id="56ac2-124">Header</span></span>       | <span data-ttu-id="56ac2-125">值</span><span class="sxs-lookup"><span data-stu-id="56ac2-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56ac2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="56ac2-126">Authorization</span></span>  | <span data-ttu-id="56ac2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56ac2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56ac2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="56ac2-129">Request body</span></span>
<span data-ttu-id="56ac2-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56ac2-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="56ac2-131">响应</span><span class="sxs-lookup"><span data-stu-id="56ac2-131">Response</span></span>
<span data-ttu-id="56ac2-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="56ac2-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56ac2-133">示例</span><span class="sxs-lookup"><span data-stu-id="56ac2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56ac2-134">请求</span><span class="sxs-lookup"><span data-stu-id="56ac2-134">Request</span></span>
<span data-ttu-id="56ac2-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56ac2-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56ac2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="56ac2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
# <a name="c"></a>[<span data-ttu-id="56ac2-137">C#</span><span class="sxs-lookup"><span data-stu-id="56ac2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56ac2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56ac2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56ac2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56ac2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56ac2-140">Java</span><span class="sxs-lookup"><span data-stu-id="56ac2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="56ac2-141">响应</span><span class="sxs-lookup"><span data-stu-id="56ac2-141">Response</span></span>
<span data-ttu-id="56ac2-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56ac2-142">The following is an example of the response.</span></span> 

><span data-ttu-id="56ac2-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="56ac2-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
