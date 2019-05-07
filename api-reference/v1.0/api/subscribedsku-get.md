---
title: 获取 subscribedSku
description: 检索组织已获取的特定商业订阅。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ec532769248a5cc7058bf8a52695c19cf2505219
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603187"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="cc45d-103">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="cc45d-103">Get subscribedSku</span></span>
<span data-ttu-id="cc45d-104">检索组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="cc45d-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc45d-105">权限</span><span class="sxs-lookup"><span data-stu-id="cc45d-105">Permissions</span></span>
<span data-ttu-id="cc45d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc45d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cc45d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc45d-108">Permission type</span></span>      | <span data-ttu-id="cc45d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc45d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc45d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc45d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc45d-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc45d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc45d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc45d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc45d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc45d-113">Not supported.</span></span>    |
|<span data-ttu-id="cc45d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc45d-114">Application</span></span> | <span data-ttu-id="cc45d-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc45d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc45d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc45d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc45d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc45d-117">Optional query parameters</span></span>
<span data-ttu-id="cc45d-118">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="cc45d-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc45d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc45d-119">Request headers</span></span>
| <span data-ttu-id="cc45d-120">名称</span><span class="sxs-lookup"><span data-stu-id="cc45d-120">Name</span></span>       | <span data-ttu-id="cc45d-121">类型</span><span class="sxs-lookup"><span data-stu-id="cc45d-121">Type</span></span> | <span data-ttu-id="cc45d-122">说明</span><span class="sxs-lookup"><span data-stu-id="cc45d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cc45d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc45d-123">Authorization</span></span>  | <span data-ttu-id="cc45d-124">string</span><span class="sxs-lookup"><span data-stu-id="cc45d-124">string</span></span>  | <span data-ttu-id="cc45d-p102">持有者&lt;令牌&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="cc45d-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc45d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc45d-127">Request body</span></span>
<span data-ttu-id="cc45d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc45d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc45d-129">响应</span><span class="sxs-lookup"><span data-stu-id="cc45d-129">Response</span></span>

<span data-ttu-id="cc45d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc45d-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc45d-131">示例</span><span class="sxs-lookup"><span data-stu-id="cc45d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc45d-132">请求</span><span class="sxs-lookup"><span data-stu-id="cc45d-132">Request</span></span>
<span data-ttu-id="cc45d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc45d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="cc45d-134">响应</span><span class="sxs-lookup"><span data-stu-id="cc45d-134">Response</span></span>
<span data-ttu-id="cc45d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc45d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cc45d-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="cc45d-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cc45d-139">语言</span><span class="sxs-lookup"><span data-stu-id="cc45d-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc45d-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc45d-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
