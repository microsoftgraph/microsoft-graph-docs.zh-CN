---
title: 列出组织
description: 检索组织对象列表。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fcfca5ed7d51949dc5bd479ec98491bac6ff4eee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955830"
---
# <a name="list-organization"></a><span data-ttu-id="12a74-103">列出组织</span><span class="sxs-lookup"><span data-stu-id="12a74-103">List organization</span></span>

<span data-ttu-id="12a74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12a74-105">检索组织对象列表。</span><span class="sxs-lookup"><span data-stu-id="12a74-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="12a74-106">权限</span><span class="sxs-lookup"><span data-stu-id="12a74-106">Permissions</span></span>
<span data-ttu-id="12a74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12a74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12a74-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12a74-109">Permission type</span></span>      | <span data-ttu-id="12a74-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12a74-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12a74-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12a74-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12a74-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="12a74-112">Not supported.</span></span>    |
|<span data-ttu-id="12a74-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12a74-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a74-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12a74-114">Not supported.</span></span>    |
|<span data-ttu-id="12a74-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="12a74-115">Application</span></span> | <span data-ttu-id="12a74-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12a74-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12a74-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12a74-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12a74-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="12a74-118">Optional query parameters</span></span>
<span data-ttu-id="12a74-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="12a74-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="12a74-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12a74-120">Request headers</span></span>
| <span data-ttu-id="12a74-121">名称</span><span class="sxs-lookup"><span data-stu-id="12a74-121">Name</span></span>       | <span data-ttu-id="12a74-122">类型</span><span class="sxs-lookup"><span data-stu-id="12a74-122">Type</span></span> | <span data-ttu-id="12a74-123">说明</span><span class="sxs-lookup"><span data-stu-id="12a74-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="12a74-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="12a74-124">Authorization</span></span>  | <span data-ttu-id="12a74-125">string</span><span class="sxs-lookup"><span data-stu-id="12a74-125">string</span></span>  | <span data-ttu-id="12a74-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12a74-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12a74-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="12a74-128">Request body</span></span>
<span data-ttu-id="12a74-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12a74-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a74-130">响应</span><span class="sxs-lookup"><span data-stu-id="12a74-130">Response</span></span>

<span data-ttu-id="12a74-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="12a74-131">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12a74-132">示例</span><span class="sxs-lookup"><span data-stu-id="12a74-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12a74-133">请求</span><span class="sxs-lookup"><span data-stu-id="12a74-133">Request</span></span>
<span data-ttu-id="12a74-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12a74-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12a74-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="12a74-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="c"></a>[<span data-ttu-id="12a74-136">C#</span><span class="sxs-lookup"><span data-stu-id="12a74-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12a74-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12a74-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12a74-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12a74-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12a74-139">Java</span><span class="sxs-lookup"><span data-stu-id="12a74-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="12a74-140">响应</span><span class="sxs-lookup"><span data-stu-id="12a74-140">Response</span></span>
<span data-ttu-id="12a74-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12a74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
