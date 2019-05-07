---
title: 列出组织
description: 检索组织对象列表。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e62157fe7fec29df4afd1e4d931a28fa6e3b77f8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611661"
---
# <a name="list-organization"></a><span data-ttu-id="e25da-103">列出组织</span><span class="sxs-lookup"><span data-stu-id="e25da-103">List organization</span></span>



<span data-ttu-id="e25da-104">检索组织对象列表。</span><span class="sxs-lookup"><span data-stu-id="e25da-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e25da-105">权限</span><span class="sxs-lookup"><span data-stu-id="e25da-105">Permissions</span></span>
<span data-ttu-id="e25da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e25da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e25da-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e25da-108">Permission type</span></span>      | <span data-ttu-id="e25da-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e25da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e25da-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e25da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e25da-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e25da-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="e25da-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e25da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e25da-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e25da-113">Not supported.</span></span>    |
|<span data-ttu-id="e25da-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e25da-114">Application</span></span> | <span data-ttu-id="e25da-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e25da-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e25da-116">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="e25da-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="e25da-117">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="e25da-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="e25da-118">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="e25da-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="e25da-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e25da-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e25da-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e25da-120">Optional query parameters</span></span>
<span data-ttu-id="e25da-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e25da-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e25da-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e25da-122">Request headers</span></span>
| <span data-ttu-id="e25da-123">名称</span><span class="sxs-lookup"><span data-stu-id="e25da-123">Name</span></span>       | <span data-ttu-id="e25da-124">类型</span><span class="sxs-lookup"><span data-stu-id="e25da-124">Type</span></span> | <span data-ttu-id="e25da-125">说明</span><span class="sxs-lookup"><span data-stu-id="e25da-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e25da-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e25da-126">Authorization</span></span>  | <span data-ttu-id="e25da-127">string</span><span class="sxs-lookup"><span data-stu-id="e25da-127">string</span></span>  | <span data-ttu-id="e25da-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e25da-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e25da-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e25da-130">Request body</span></span>
<span data-ttu-id="e25da-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e25da-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e25da-132">响应</span><span class="sxs-lookup"><span data-stu-id="e25da-132">Response</span></span>

<span data-ttu-id="e25da-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e25da-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e25da-134">示例</span><span class="sxs-lookup"><span data-stu-id="e25da-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e25da-135">请求</span><span class="sxs-lookup"><span data-stu-id="e25da-135">Request</span></span>
<span data-ttu-id="e25da-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e25da-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="e25da-137">响应</span><span class="sxs-lookup"><span data-stu-id="e25da-137">Response</span></span>
<span data-ttu-id="e25da-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e25da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e25da-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e25da-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e25da-142">语言</span><span class="sxs-lookup"><span data-stu-id="e25da-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e25da-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="e25da-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
