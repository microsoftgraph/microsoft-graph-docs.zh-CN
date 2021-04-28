---
title: 获取 educationSchool
description: 检索 school 对象的属性和关系。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ad8567c13a6fd505f53c3e99a3a9651b3d68a032
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035552"
---
# <a name="get-educationschool"></a><span data-ttu-id="88e98-103">获取 educationSchool</span><span class="sxs-lookup"><span data-stu-id="88e98-103">Get educationSchool</span></span>

<span data-ttu-id="88e98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88e98-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88e98-105">检索 school 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88e98-105">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88e98-106">权限</span><span class="sxs-lookup"><span data-stu-id="88e98-106">Permissions</span></span>
<span data-ttu-id="88e98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88e98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e98-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88e98-109">Permission type</span></span>      | <span data-ttu-id="88e98-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88e98-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88e98-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88e98-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="88e98-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="88e98-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="88e98-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88e98-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="88e98-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88e98-114">Not supported.</span></span>  |
|<span data-ttu-id="88e98-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88e98-115">Application</span></span> | <span data-ttu-id="88e98-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e98-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="88e98-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88e98-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88e98-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88e98-118">Optional query parameters</span></span>
<span data-ttu-id="88e98-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="88e98-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88e98-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88e98-120">Request headers</span></span>
| <span data-ttu-id="88e98-121">标头</span><span class="sxs-lookup"><span data-stu-id="88e98-121">Header</span></span>       | <span data-ttu-id="88e98-122">值</span><span class="sxs-lookup"><span data-stu-id="88e98-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88e98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88e98-123">Authorization</span></span>  | <span data-ttu-id="88e98-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88e98-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88e98-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="88e98-126">Request body</span></span>
<span data-ttu-id="88e98-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88e98-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="88e98-128">响应</span><span class="sxs-lookup"><span data-stu-id="88e98-128">Response</span></span>
<span data-ttu-id="88e98-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88e98-129">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88e98-130">示例</span><span class="sxs-lookup"><span data-stu-id="88e98-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88e98-131">请求</span><span class="sxs-lookup"><span data-stu-id="88e98-131">Request</span></span>
<span data-ttu-id="88e98-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88e98-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88e98-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="88e98-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="c"></a>[<span data-ttu-id="88e98-134">C#</span><span class="sxs-lookup"><span data-stu-id="88e98-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88e98-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88e98-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88e98-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88e98-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88e98-137">Java</span><span class="sxs-lookup"><span data-stu-id="88e98-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="88e98-138">响应</span><span class="sxs-lookup"><span data-stu-id="88e98-138">Response</span></span>
<span data-ttu-id="88e98-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="88e98-139">The following is an example of the response.</span></span> 

><span data-ttu-id="88e98-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88e98-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "principalEmail": "AmyRoebuck@contoso.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
