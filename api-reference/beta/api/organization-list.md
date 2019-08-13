---
title: 列出组织
description: 检索组织对象列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8382e36945331ef63e01379842d452474049193f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342486"
---
# <a name="list-organization"></a><span data-ttu-id="f0d86-103">列出组织</span><span class="sxs-lookup"><span data-stu-id="f0d86-103">List organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0d86-104">检索组织对象列表。</span><span class="sxs-lookup"><span data-stu-id="f0d86-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0d86-105">权限</span><span class="sxs-lookup"><span data-stu-id="f0d86-105">Permissions</span></span>
<span data-ttu-id="f0d86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0d86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0d86-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0d86-108">Permission type</span></span>      | <span data-ttu-id="f0d86-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0d86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0d86-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0d86-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0d86-111">Not supported.</span></span>    |
|<span data-ttu-id="f0d86-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0d86-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0d86-113">Not supported.</span></span>    |
|<span data-ttu-id="f0d86-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0d86-114">Application</span></span> | <span data-ttu-id="f0d86-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0d86-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0d86-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0d86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0d86-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0d86-117">Optional query parameters</span></span>
<span data-ttu-id="f0d86-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f0d86-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0d86-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0d86-119">Request headers</span></span>
| <span data-ttu-id="f0d86-120">名称</span><span class="sxs-lookup"><span data-stu-id="f0d86-120">Name</span></span>       | <span data-ttu-id="f0d86-121">类型</span><span class="sxs-lookup"><span data-stu-id="f0d86-121">Type</span></span> | <span data-ttu-id="f0d86-122">说明</span><span class="sxs-lookup"><span data-stu-id="f0d86-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f0d86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0d86-123">Authorization</span></span>  | <span data-ttu-id="f0d86-124">string</span><span class="sxs-lookup"><span data-stu-id="f0d86-124">string</span></span>  | <span data-ttu-id="f0d86-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0d86-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0d86-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0d86-127">Request body</span></span>
<span data-ttu-id="f0d86-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0d86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0d86-129">响应</span><span class="sxs-lookup"><span data-stu-id="f0d86-129">Response</span></span>

<span data-ttu-id="f0d86-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f0d86-130">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0d86-131">示例</span><span class="sxs-lookup"><span data-stu-id="f0d86-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0d86-132">请求</span><span class="sxs-lookup"><span data-stu-id="f0d86-132">Request</span></span>
<span data-ttu-id="f0d86-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0d86-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f0d86-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f0d86-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f0d86-135">C#</span><span class="sxs-lookup"><span data-stu-id="f0d86-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0d86-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0d86-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f0d86-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="f0d86-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f0d86-138">Java</span><span class="sxs-lookup"><span data-stu-id="f0d86-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0d86-139">响应</span><span class="sxs-lookup"><span data-stu-id="f0d86-139">Response</span></span>
<span data-ttu-id="f0d86-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0d86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
