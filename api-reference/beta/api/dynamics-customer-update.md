---
title: 更新客户
description: 更新 Dynamics 365 Business Central 中的客户对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e19c24cd453a5702e64019e6fb96903786d41a19
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045626"
---
# <a name="update-customers"></a><span data-ttu-id="125f6-103">更新客户</span><span class="sxs-lookup"><span data-stu-id="125f6-103">Update customers</span></span>

<span data-ttu-id="125f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="125f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="125f6-105">更新 Dynamics 365 Business Central 的客户对象的属性。</span><span class="sxs-lookup"><span data-stu-id="125f6-105">Update the properties of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="125f6-106">权限</span><span class="sxs-lookup"><span data-stu-id="125f6-106">Permissions</span></span>
<span data-ttu-id="125f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="125f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="125f6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="125f6-109">Permission type</span></span> |<span data-ttu-id="125f6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="125f6-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="125f6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="125f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="125f6-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="125f6-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="125f6-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="125f6-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="125f6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="125f6-114">Not supported.</span></span>|
|<span data-ttu-id="125f6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="125f6-115">Application</span></span>|<span data-ttu-id="125f6-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="125f6-116">Financials.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="125f6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="125f6-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="125f6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="125f6-118">Optional query parameters</span></span>
<span data-ttu-id="125f6-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="125f6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="125f6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="125f6-120">Request headers</span></span>
|<span data-ttu-id="125f6-121">标头</span><span class="sxs-lookup"><span data-stu-id="125f6-121">Header</span></span>         |<span data-ttu-id="125f6-122">值</span><span class="sxs-lookup"><span data-stu-id="125f6-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="125f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="125f6-123">Authorization</span></span>  |<span data-ttu-id="125f6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="125f6-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="125f6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="125f6-126">Content-Type</span></span>   |<span data-ttu-id="125f6-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="125f6-127">application/json.</span></span>         |
|<span data-ttu-id="125f6-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="125f6-128">If-Match</span></span>       |<span data-ttu-id="125f6-129">必需。</span><span class="sxs-lookup"><span data-stu-id="125f6-129">Required.</span></span> <span data-ttu-id="125f6-130">如果包含此请求标头且提供的 eTag 与客户的当前标记不匹配，**将不会** 更新客户。</span><span class="sxs-lookup"><span data-stu-id="125f6-130">When this request header is included and the eTag provided does not match the current tag on the **customers**, the **customers** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="125f6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="125f6-131">Request body</span></span>
<span data-ttu-id="125f6-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="125f6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="125f6-135">响应</span><span class="sxs-lookup"><span data-stu-id="125f6-135">Response</span></span>
<span data-ttu-id="125f6-136">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 **customers** 对象。</span><span class="sxs-lookup"><span data-stu-id="125f6-136">If successful, this method returns a `200 OK` response code and an updated **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="125f6-137">示例</span><span class="sxs-lookup"><span data-stu-id="125f6-137">Example</span></span>

<span data-ttu-id="125f6-138">**请求**</span><span class="sxs-lookup"><span data-stu-id="125f6-138">**Request**</span></span>

<span data-ttu-id="125f6-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="125f6-139">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
Content-type: application/json

{
  "displayName": "Coho Winery Inc.",
  "phoneNumber": "(555) 555-1234"
}
```

<span data-ttu-id="125f6-140">**响应**</span><span class="sxs-lookup"><span data-stu-id="125f6-140">**Response**</span></span>

<span data-ttu-id="125f6-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="125f6-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="125f6-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="125f6-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery Inc.",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "(555) 555-1234"
  "email": "jim.glynn@cronuscorp.net",
  "website": "",
  "taxLiable": true,
  "taxAreaId": "taxAreaId-value",
  "taxAreaDisplayName": "tax area",
  "taxRegistrationNumber": "28012001T",
  "currencyId": "currencyId-value",
  "currencyCode": "USD",
  "paymentTermsId": "paymentTermsId-value",
  "shipmentMethodId": "shipmentMethodId-value",
  "paymentMethodId": "paymentMethod-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```




