---
title: 创建客户
description: 在 Dynamics 365 Business Central 中创建 customer 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3eb9717f980120e4acb7d9e3c192a95cc2e2872b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008356"
---
# <a name="create-customers"></a><span data-ttu-id="0f8e4-103">创建客户</span><span class="sxs-lookup"><span data-stu-id="0f8e4-103">Create customers</span></span>

<span data-ttu-id="0f8e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f8e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f8e4-105">在 Dynamics 365 Business Central 中创建 customer 对象。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-105">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f8e4-106">权限</span><span class="sxs-lookup"><span data-stu-id="0f8e4-106">Permissions</span></span>
<span data-ttu-id="0f8e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f8e4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f8e4-109">Permission type</span></span> |<span data-ttu-id="0f8e4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f8e4-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0f8e4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f8e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f8e4-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f8e4-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0f8e4-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="0f8e4-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0f8e4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-114">Not supported.</span></span>|
|<span data-ttu-id="0f8e4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f8e4-115">Application</span></span>|<span data-ttu-id="0f8e4-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f8e4-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f8e4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f8e4-117">HTTP request</span></span>
```
POST /financials/companies/{id}/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f8e4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0f8e4-118">Optional query parameters</span></span>
<span data-ttu-id="0f8e4-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f8e4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f8e4-120">Request headers</span></span>
|<span data-ttu-id="0f8e4-121">标头</span><span class="sxs-lookup"><span data-stu-id="0f8e4-121">Header</span></span>         |<span data-ttu-id="0f8e4-122">值</span><span class="sxs-lookup"><span data-stu-id="0f8e4-122">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="0f8e4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f8e4-123">Authorization</span></span>  |<span data-ttu-id="0f8e4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0f8e4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f8e4-126">Content-Type</span></span>   |<span data-ttu-id="0f8e4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0f8e4-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="0f8e4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f8e4-128">Request body</span></span>
<span data-ttu-id="0f8e4-129">在请求正文中，提供 **customers** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-129">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="0f8e4-130">响应</span><span class="sxs-lookup"><span data-stu-id="0f8e4-130">Response</span></span>
<span data-ttu-id="0f8e4-131">如果成功，此方法 ```201 Created``` 在响应正文中返回响应代码和 **customers** 对象。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-131">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f8e4-132">示例</span><span class="sxs-lookup"><span data-stu-id="0f8e4-132">Example</span></span>

<span data-ttu-id="0f8e4-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="0f8e4-133">**Request**</span></span>

<span data-ttu-id="0f8e4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/customers
Content-type: application/json

{
  "number": "10000",
  "displayName": "Coho Winery",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
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
  "paymentMethodId": "paymentMethodId-value",
  "blocked": " ",
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
}

```

<span data-ttu-id="0f8e4-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="0f8e4-135">**Response**</span></span>

<span data-ttu-id="0f8e4-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="0f8e4-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0f8e4-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0f8e4-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "jim.glynn@cronuscorp.net",
  "website": "",
  "taxLiable": true,
  "taxAreaId": "taxAreaId-value",
  "taxAreaDisplayName": "tax area",
  "taxRegistrationNumber": "28012001T",
  "currencyCode": "USD",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}

```



