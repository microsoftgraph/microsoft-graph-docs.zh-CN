---
title: 获取 educationSchool
description: 检索 school 对象的属性和关系。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 7fe3e094ca06286a8a89768185ed131dd27e1fa3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839072"
---
# <a name="get-educationschool"></a><span data-ttu-id="be275-103">获取 educationSchool</span><span class="sxs-lookup"><span data-stu-id="be275-103">Get educationSchool</span></span>

<span data-ttu-id="be275-104">检索 school 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be275-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be275-105">权限</span><span class="sxs-lookup"><span data-stu-id="be275-105">Permissions</span></span>
<span data-ttu-id="be275-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be275-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="be275-108">Permission type</span></span>      | <span data-ttu-id="be275-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be275-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be275-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be275-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="be275-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="be275-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="be275-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be275-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="be275-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="be275-113">Not supported.</span></span>  |
|<span data-ttu-id="be275-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="be275-114">Application</span></span> | <span data-ttu-id="be275-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be275-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="be275-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be275-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be275-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be275-117">Optional query parameters</span></span>
<span data-ttu-id="be275-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be275-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be275-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="be275-119">Request headers</span></span>
| <span data-ttu-id="be275-120">标头</span><span class="sxs-lookup"><span data-stu-id="be275-120">Header</span></span>       | <span data-ttu-id="be275-121">值</span><span class="sxs-lookup"><span data-stu-id="be275-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be275-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be275-122">Authorization</span></span>  | <span data-ttu-id="be275-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be275-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be275-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="be275-125">Request body</span></span>
<span data-ttu-id="be275-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be275-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="be275-127">响应</span><span class="sxs-lookup"><span data-stu-id="be275-127">Response</span></span>
<span data-ttu-id="be275-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be275-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be275-129">示例</span><span class="sxs-lookup"><span data-stu-id="be275-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be275-130">请求</span><span class="sxs-lookup"><span data-stu-id="be275-130">Request</span></span>
<span data-ttu-id="be275-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be275-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="be275-132">响应</span><span class="sxs-lookup"><span data-stu-id="be275-132">Response</span></span>
<span data-ttu-id="be275-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be275-133">The following is an example of the response.</span></span> 

><span data-ttu-id="be275-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be275-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
