---
title: 列出组织
description: 检索组织对象列表。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f11ed888ad14334584a8f2e6aea9bb821f86438f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441730"
---
# <a name="list-organization"></a><span data-ttu-id="89f3f-103">列出组织</span><span class="sxs-lookup"><span data-stu-id="89f3f-103">List organization</span></span>

<span data-ttu-id="89f3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89f3f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="89f3f-105">检索组织对象列表。</span><span class="sxs-lookup"><span data-stu-id="89f3f-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="89f3f-106">权限</span><span class="sxs-lookup"><span data-stu-id="89f3f-106">Permissions</span></span>
<span data-ttu-id="89f3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89f3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89f3f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="89f3f-109">Permission type</span></span>      | <span data-ttu-id="89f3f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89f3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89f3f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89f3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="89f3f-112">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89f3f-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="89f3f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89f3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89f3f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89f3f-114">Not supported.</span></span>    |
|<span data-ttu-id="89f3f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="89f3f-115">Application</span></span> | <span data-ttu-id="89f3f-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89f3f-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="89f3f-117">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="89f3f-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="89f3f-118">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="89f3f-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="89f3f-119">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="89f3f-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="89f3f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89f3f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89f3f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="89f3f-121">Optional query parameters</span></span>
<span data-ttu-id="89f3f-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="89f3f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="89f3f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="89f3f-123">Request headers</span></span>
| <span data-ttu-id="89f3f-124">名称</span><span class="sxs-lookup"><span data-stu-id="89f3f-124">Name</span></span>       | <span data-ttu-id="89f3f-125">类型</span><span class="sxs-lookup"><span data-stu-id="89f3f-125">Type</span></span> | <span data-ttu-id="89f3f-126">说明</span><span class="sxs-lookup"><span data-stu-id="89f3f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="89f3f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="89f3f-127">Authorization</span></span>  | <span data-ttu-id="89f3f-128">string</span><span class="sxs-lookup"><span data-stu-id="89f3f-128">string</span></span>  | <span data-ttu-id="89f3f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89f3f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89f3f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="89f3f-131">Request body</span></span>
<span data-ttu-id="89f3f-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89f3f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89f3f-133">响应</span><span class="sxs-lookup"><span data-stu-id="89f3f-133">Response</span></span>

<span data-ttu-id="89f3f-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="89f3f-134">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89f3f-135">示例</span><span class="sxs-lookup"><span data-stu-id="89f3f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89f3f-136">请求</span><span class="sxs-lookup"><span data-stu-id="89f3f-136">Request</span></span>
<span data-ttu-id="89f3f-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89f3f-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89f3f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="89f3f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[<span data-ttu-id="89f3f-139">C#</span><span class="sxs-lookup"><span data-stu-id="89f3f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89f3f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89f3f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89f3f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89f3f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89f3f-142">Java</span><span class="sxs-lookup"><span data-stu-id="89f3f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="89f3f-143">响应</span><span class="sxs-lookup"><span data-stu-id="89f3f-143">Response</span></span>
<span data-ttu-id="89f3f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89f3f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
