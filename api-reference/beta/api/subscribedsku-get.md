---
title: 获取 subscribedSku
description: 检索组织已获取的特定商业订阅。
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0370ee0109b397f75aaac78f07426c689ca545fc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443566"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="b3a5d-103">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="b3a5d-103">Get subscribedSku</span></span>

<span data-ttu-id="b3a5d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3a5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3a5d-105">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-105">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3a5d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b3a5d-106">Permissions</span></span>
<span data-ttu-id="b3a5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b3a5d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3a5d-109">Permission type</span></span>      | <span data-ttu-id="b3a5d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3a5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3a5d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3a5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3a5d-112">Organization.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3a5d-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3a5d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3a5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3a5d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-114">Not supported.</span></span>    |
|<span data-ttu-id="b3a5d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3a5d-115">Application</span></span> | <span data-ttu-id="b3a5d-116">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3a5d-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3a5d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3a5d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3a5d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b3a5d-118">Optional query parameters</span></span>
<span data-ttu-id="b3a5d-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b3a5d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3a5d-120">Request headers</span></span>

| <span data-ttu-id="b3a5d-121">名称</span><span class="sxs-lookup"><span data-stu-id="b3a5d-121">Name</span></span>       | <span data-ttu-id="b3a5d-122">说明</span><span class="sxs-lookup"><span data-stu-id="b3a5d-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="b3a5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3a5d-123">Authorization</span></span>  | <span data-ttu-id="b3a5d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3a5d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3a5d-126">Request body</span></span>
<span data-ttu-id="b3a5d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3a5d-128">响应</span><span class="sxs-lookup"><span data-stu-id="b3a5d-128">Response</span></span>

<span data-ttu-id="b3a5d-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-129">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3a5d-130">示例</span><span class="sxs-lookup"><span data-stu-id="b3a5d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3a5d-131">请求</span><span class="sxs-lookup"><span data-stu-id="b3a5d-131">Request</span></span>
<span data-ttu-id="b3a5d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3a5d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3a5d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
# <a name="c"></a>[<span data-ttu-id="b3a5d-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3a5d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3a5d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3a5d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3a5d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3a5d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3a5d-137">Java</span><span class="sxs-lookup"><span data-stu-id="b3a5d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedsku-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3a5d-138">响应</span><span class="sxs-lookup"><span data-stu-id="b3a5d-138">Response</span></span>
<span data-ttu-id="b3a5d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3a5d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 450

{
  "capabilityStatus": "capabilityStatus-value",
  "consumedUnits": 99,
  "prepaidUnits": {
    "enabled": 99,
    "suspended": 99,
    "warning": 99
  },
  "servicePlans": [
    {
      "servicePlanId": "servicePlanId-value",
      "servicePlanName": "servicePlanName-value",
      "provisioningStatus": "provisioningStatus-value",
      "appliesTo": "appliesTo-value"
    }
  ],
  "skuId": "skuId-value",
  "skuPartNumber": "skuPartNumber-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
