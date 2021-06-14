---
title: 列出 educationUser 的学校
description: 检索用户所在的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 180309cb87e3d8678e81235309338a1817fb0b91
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911996"
---
# <a name="list-schools-of-an-educationuser"></a><span data-ttu-id="6c9d8-103">列出 educationUser 的学校</span><span class="sxs-lookup"><span data-stu-id="6c9d8-103">List schools of an educationUser</span></span>

<span data-ttu-id="6c9d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c9d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c9d8-105">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-105">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="6c9d8-106">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="6c9d8-107">在这种情况下，使用 `...v1.0/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-107">Use the `...v1.0/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c9d8-108">权限</span><span class="sxs-lookup"><span data-stu-id="6c9d8-108">Permissions</span></span>

<span data-ttu-id="6c9d8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c9d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c9d8-111">Permission type</span></span>                        | <span data-ttu-id="6c9d8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c9d8-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6c9d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c9d8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c9d8-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="6c9d8-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="6c9d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c9d8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c9d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-116">Not supported.</span></span>                              |
| <span data-ttu-id="6c9d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c9d8-117">Application</span></span>                            | <span data-ttu-id="6c9d8-118">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9d8-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c9d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c9d8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{educationUserId}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c9d8-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6c9d8-120">Optional query parameters</span></span>

<span data-ttu-id="6c9d8-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c9d8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c9d8-122">Request headers</span></span>

| <span data-ttu-id="6c9d8-123">标头</span><span class="sxs-lookup"><span data-stu-id="6c9d8-123">Header</span></span>        | <span data-ttu-id="6c9d8-124">值</span><span class="sxs-lookup"><span data-stu-id="6c9d8-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6c9d8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c9d8-125">Authorization</span></span> | <span data-ttu-id="6c9d8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c9d8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c9d8-128">Request body</span></span>

<span data-ttu-id="6c9d8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c9d8-130">响应</span><span class="sxs-lookup"><span data-stu-id="6c9d8-130">Response</span></span>

<span data-ttu-id="6c9d8-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-131">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c9d8-132">示例</span><span class="sxs-lookup"><span data-stu-id="6c9d8-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6c9d8-133">请求</span><span class="sxs-lookup"><span data-stu-id="6c9d8-133">Request</span></span>

<span data-ttu-id="6c9d8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c9d8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c9d8-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="6c9d8-136">C#</span><span class="sxs-lookup"><span data-stu-id="6c9d8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c9d8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c9d8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c9d8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c9d8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c9d8-139">Java</span><span class="sxs-lookup"><span data-stu-id="6c9d8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6c9d8-140">响应</span><span class="sxs-lookup"><span data-stu-id="6c9d8-140">Response</span></span>

<span data-ttu-id="6c9d8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-141">The following is an example of the response.</span></span>

><span data-ttu-id="6c9d8-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6c9d8-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
