---
title: 列出 subscribedSkus
description: 检索组织已获取的商业订阅列表。
localization_priority: Priority
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0e1d403e4930c9edcf48dd7c008fd95c9d3fbe61
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442535"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="547dc-103">列出 subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="547dc-103">List subscribedSkus</span></span>

<span data-ttu-id="547dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="547dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="547dc-105">获取组织已获取的商业版订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="547dc-105">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="547dc-106">权限</span><span class="sxs-lookup"><span data-stu-id="547dc-106">Permissions</span></span>
<span data-ttu-id="547dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="547dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="547dc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="547dc-109">Permission type</span></span>      | <span data-ttu-id="547dc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="547dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="547dc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="547dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="547dc-112">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="547dc-112">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="547dc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="547dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="547dc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="547dc-114">Not supported.</span></span>    |
|<span data-ttu-id="547dc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="547dc-115">Application</span></span> | <span data-ttu-id="547dc-116">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="547dc-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="547dc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="547dc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="547dc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="547dc-118">Optional query parameters</span></span>
<span data-ttu-id="547dc-119">此方法 **不** 支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="547dc-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="547dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="547dc-120">Request headers</span></span>

| <span data-ttu-id="547dc-121">名称</span><span class="sxs-lookup"><span data-stu-id="547dc-121">Name</span></span>       | <span data-ttu-id="547dc-122">说明</span><span class="sxs-lookup"><span data-stu-id="547dc-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="547dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="547dc-123">Authorization</span></span>  | <span data-ttu-id="547dc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="547dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="547dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="547dc-126">Request body</span></span>
<span data-ttu-id="547dc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="547dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="547dc-128">响应</span><span class="sxs-lookup"><span data-stu-id="547dc-128">Response</span></span>

<span data-ttu-id="547dc-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="547dc-129">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="547dc-130">示例</span><span class="sxs-lookup"><span data-stu-id="547dc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="547dc-131">请求</span><span class="sxs-lookup"><span data-stu-id="547dc-131">Request</span></span>
<span data-ttu-id="547dc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="547dc-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="547dc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="547dc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
# <a name="c"></a>[<span data-ttu-id="547dc-134">C#</span><span class="sxs-lookup"><span data-stu-id="547dc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="547dc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="547dc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="547dc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="547dc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="547dc-137">Java</span><span class="sxs-lookup"><span data-stu-id="547dc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="547dc-138">响应</span><span class="sxs-lookup"><span data-stu-id="547dc-138">Response</span></span>
<span data-ttu-id="547dc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="547dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus",
    "value": [
        {
            "capabilityStatus": "Enabled",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
            "prepaidUnits": {
                "enabled": 25,
                "suspended": 0,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
                    "servicePlanName": "ADALLOM_S_O365",
                    "provisioningStatus": "Success",
                    "appliesTo": "User"
                }
            ],
            "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
            "skuPartNumber": "ENTERPRISEPREMIUM",
            "appliesTo": "User"
        },
        {
            "capabilityStatus": "Suspended",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_d17b27af-3f49-4822-99f9-56a661538792",
            "prepaidUnits": {
                "enabled": 0,
                "suspended": 25,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "f9646fb2-e3b2-4309-95de-dc4833737456",
                    "servicePlanName": "CRMSTANDARD",
                    "provisioningStatus": "Disabled",
                    "appliesTo": "User"
                }
            ],
            "skuId": "d17b27af-3f49-4822-99f9-56a661538792",
            "skuPartNumber": "CRMSTANDARD",
            "appliesTo": "User"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
