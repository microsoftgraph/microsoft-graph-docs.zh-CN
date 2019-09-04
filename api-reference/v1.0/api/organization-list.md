---
title: 列出组织
description: 检索组织对象列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a56d45fe0570b241156096814792b145b32c579f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730111"
---
# <a name="list-organization"></a><span data-ttu-id="b698b-103">列出组织</span><span class="sxs-lookup"><span data-stu-id="b698b-103">List organization</span></span>



<span data-ttu-id="b698b-104">检索组织对象列表。</span><span class="sxs-lookup"><span data-stu-id="b698b-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b698b-105">权限</span><span class="sxs-lookup"><span data-stu-id="b698b-105">Permissions</span></span>
<span data-ttu-id="b698b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b698b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b698b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b698b-108">Permission type</span></span>      | <span data-ttu-id="b698b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b698b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b698b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b698b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b698b-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b698b-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="b698b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b698b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b698b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b698b-113">Not supported.</span></span>    |
|<span data-ttu-id="b698b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b698b-114">Application</span></span> | <span data-ttu-id="b698b-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b698b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="b698b-116">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="b698b-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="b698b-117">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="b698b-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="b698b-118">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="b698b-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="b698b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b698b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b698b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b698b-120">Optional query parameters</span></span>
<span data-ttu-id="b698b-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b698b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b698b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b698b-122">Request headers</span></span>
| <span data-ttu-id="b698b-123">名称</span><span class="sxs-lookup"><span data-stu-id="b698b-123">Name</span></span>       | <span data-ttu-id="b698b-124">类型</span><span class="sxs-lookup"><span data-stu-id="b698b-124">Type</span></span> | <span data-ttu-id="b698b-125">说明</span><span class="sxs-lookup"><span data-stu-id="b698b-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b698b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b698b-126">Authorization</span></span>  | <span data-ttu-id="b698b-127">string</span><span class="sxs-lookup"><span data-stu-id="b698b-127">string</span></span>  | <span data-ttu-id="b698b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b698b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b698b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b698b-130">Request body</span></span>
<span data-ttu-id="b698b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b698b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b698b-132">响应</span><span class="sxs-lookup"><span data-stu-id="b698b-132">Response</span></span>

<span data-ttu-id="b698b-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b698b-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b698b-134">示例</span><span class="sxs-lookup"><span data-stu-id="b698b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b698b-135">请求</span><span class="sxs-lookup"><span data-stu-id="b698b-135">Request</span></span>
<span data-ttu-id="b698b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b698b-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b698b-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b698b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b698b-138">C#</span><span class="sxs-lookup"><span data-stu-id="b698b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b698b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b698b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b698b-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="b698b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b698b-141">响应</span><span class="sxs-lookup"><span data-stu-id="b698b-141">Response</span></span>
<span data-ttu-id="b698b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b698b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
