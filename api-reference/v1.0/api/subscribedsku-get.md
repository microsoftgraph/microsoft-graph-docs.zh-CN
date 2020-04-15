---
title: 获取 subscribedSku
description: 检索组织已获取的特定商业订阅。
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a00d823c881ee315887ab42fb98c143cf0685efe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442385"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="42849-103">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="42849-103">Get subscribedSku</span></span>

<span data-ttu-id="42849-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42849-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42849-105">获取组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="42849-105">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="42849-106">权限</span><span class="sxs-lookup"><span data-stu-id="42849-106">Permissions</span></span>
<span data-ttu-id="42849-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="42849-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="42849-109">Permission type</span></span>      | <span data-ttu-id="42849-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42849-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42849-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42849-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42849-112">全部、全部、全部、Directory.accessasuser.all、全部、目录、全部、</span><span class="sxs-lookup"><span data-stu-id="42849-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42849-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42849-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42849-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="42849-114">Not supported.</span></span>    |
|<span data-ttu-id="42849-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="42849-115">Application</span></span> | <span data-ttu-id="42849-116">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42849-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42849-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42849-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42849-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="42849-118">Optional query parameters</span></span>
<span data-ttu-id="42849-119">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="42849-119">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42849-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42849-120">Request headers</span></span>

| <span data-ttu-id="42849-121">名称</span><span class="sxs-lookup"><span data-stu-id="42849-121">Name</span></span>       | <span data-ttu-id="42849-122">说明</span><span class="sxs-lookup"><span data-stu-id="42849-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="42849-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42849-123">Authorization</span></span>  | <span data-ttu-id="42849-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42849-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42849-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42849-126">Request body</span></span>
<span data-ttu-id="42849-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42849-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42849-128">响应</span><span class="sxs-lookup"><span data-stu-id="42849-128">Response</span></span>

<span data-ttu-id="42849-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42849-129">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42849-130">示例</span><span class="sxs-lookup"><span data-stu-id="42849-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42849-131">请求</span><span class="sxs-lookup"><span data-stu-id="42849-131">Request</span></span>
<span data-ttu-id="42849-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42849-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42849-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="42849-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
# <a name="c"></a>[<span data-ttu-id="42849-134">C#</span><span class="sxs-lookup"><span data-stu-id="42849-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42849-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42849-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42849-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42849-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42849-137">Java</span><span class="sxs-lookup"><span data-stu-id="42849-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedsku-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42849-138">响应</span><span class="sxs-lookup"><span data-stu-id="42849-138">Response</span></span>
<span data-ttu-id="42849-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42849-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus/$entity",
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
        },
        {
            "servicePlanId": "9f431833-0334-42de-a7dc-70aa40db46db",
            "servicePlanName": "LOCKBOX_ENTERPRISE",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        }
    ],
    "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "skuPartNumber": "ENTERPRISEPREMIUM",
    "appliesTo": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
