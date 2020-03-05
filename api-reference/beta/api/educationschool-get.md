---
title: 获取 educationSchool
description: 检索 school 对象的属性和关系。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c4aa211da24bb95cc810916f933b64c372c9b574
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425469"
---
# <a name="get-educationschool"></a><span data-ttu-id="df4d0-103">获取 educationSchool</span><span class="sxs-lookup"><span data-stu-id="df4d0-103">Get educationSchool</span></span>

<span data-ttu-id="df4d0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="df4d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df4d0-105">检索 school 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df4d0-105">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df4d0-106">权限</span><span class="sxs-lookup"><span data-stu-id="df4d0-106">Permissions</span></span>
<span data-ttu-id="df4d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df4d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df4d0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df4d0-109">Permission type</span></span>      | <span data-ttu-id="df4d0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df4d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df4d0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df4d0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="df4d0-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="df4d0-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="df4d0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df4d0-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="df4d0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df4d0-114">Not supported.</span></span>  |
|<span data-ttu-id="df4d0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df4d0-115">Application</span></span> | <span data-ttu-id="df4d0-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df4d0-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="df4d0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df4d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="df4d0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="df4d0-118">Optional query parameters</span></span>
<span data-ttu-id="df4d0-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="df4d0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df4d0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df4d0-120">Request headers</span></span>
| <span data-ttu-id="df4d0-121">标头</span><span class="sxs-lookup"><span data-stu-id="df4d0-121">Header</span></span>       | <span data-ttu-id="df4d0-122">值</span><span class="sxs-lookup"><span data-stu-id="df4d0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df4d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df4d0-123">Authorization</span></span>  | <span data-ttu-id="df4d0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df4d0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df4d0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="df4d0-126">Request body</span></span>
<span data-ttu-id="df4d0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df4d0-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="df4d0-128">响应</span><span class="sxs-lookup"><span data-stu-id="df4d0-128">Response</span></span>
<span data-ttu-id="df4d0-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df4d0-129">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df4d0-130">示例</span><span class="sxs-lookup"><span data-stu-id="df4d0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df4d0-131">请求</span><span class="sxs-lookup"><span data-stu-id="df4d0-131">Request</span></span>
<span data-ttu-id="df4d0-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df4d0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df4d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="df4d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10001
```
# <a name="c"></a>[<span data-ttu-id="df4d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="df4d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df4d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df4d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df4d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df4d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="df4d0-137">响应</span><span class="sxs-lookup"><span data-stu-id="df4d0-137">Response</span></span>
<span data-ttu-id="df4d0-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df4d0-138">The following is an example of the response.</span></span> 

><span data-ttu-id="df4d0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="df4d0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "schoolPrincipalEmail": "AmyRoebuck@contoso.com",
  "schoolPrincipalName": "Amy Roebuck",
  "externalSchoolPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
