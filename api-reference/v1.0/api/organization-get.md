---
title: 获取组织
description: 检索当前经过身份验证的组织的属性和关系。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6233a9fdf9db149a622b95eb18962bc16c355624
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274408"
---
# <a name="get-organization"></a><span data-ttu-id="2fe49-103">获取组织</span><span class="sxs-lookup"><span data-stu-id="2fe49-103">Get organization</span></span>

<span data-ttu-id="2fe49-104">检索当前经过身份验证的组织的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2fe49-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fe49-105">权限</span><span class="sxs-lookup"><span data-stu-id="2fe49-105">Permissions</span></span>

<span data-ttu-id="2fe49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fe49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fe49-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fe49-108">Permission type</span></span>      | <span data-ttu-id="2fe49-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fe49-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fe49-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fe49-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2fe49-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fe49-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="2fe49-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fe49-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fe49-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fe49-113">Not supported.</span></span>    |
|<span data-ttu-id="2fe49-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fe49-114">Application</span></span> | <span data-ttu-id="2fe49-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fe49-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="2fe49-116">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="2fe49-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="2fe49-117">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="2fe49-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="2fe49-118">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="2fe49-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="2fe49-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fe49-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fe49-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2fe49-120">Optional query parameters</span></span>

<span data-ttu-id="2fe49-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2fe49-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fe49-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fe49-122">Request headers</span></span>

| <span data-ttu-id="2fe49-123">名称</span><span class="sxs-lookup"><span data-stu-id="2fe49-123">Name</span></span>       | <span data-ttu-id="2fe49-124">类型</span><span class="sxs-lookup"><span data-stu-id="2fe49-124">Type</span></span> | <span data-ttu-id="2fe49-125">说明</span><span class="sxs-lookup"><span data-stu-id="2fe49-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2fe49-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fe49-126">Authorization</span></span>  | <span data-ttu-id="2fe49-127">string</span><span class="sxs-lookup"><span data-stu-id="2fe49-127">string</span></span>  | <span data-ttu-id="2fe49-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2fe49-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fe49-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fe49-130">Request body</span></span>

<span data-ttu-id="2fe49-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2fe49-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fe49-132">响应</span><span class="sxs-lookup"><span data-stu-id="2fe49-132">Response</span></span>

<span data-ttu-id="2fe49-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一个[组织](../resources/organization.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="2fe49-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fe49-134">示例</span><span class="sxs-lookup"><span data-stu-id="2fe49-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2fe49-135">请求</span><span class="sxs-lookup"><span data-stu-id="2fe49-135">Request</span></span>

<span data-ttu-id="2fe49-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2fe49-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```

##### <a name="response"></a><span data-ttu-id="2fe49-137">响应</span><span class="sxs-lookup"><span data-stu-id="2fe49-137">Response</span></span>

<span data-ttu-id="2fe49-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2fe49-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2fe49-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2fe49-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2fe49-142">C#</span><span class="sxs-lookup"><span data-stu-id="2fe49-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fe49-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fe49-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2fe49-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fe49-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_organization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
