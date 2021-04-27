---
title: 获取客户
description: 获取 Dynamics 365 Business Central 中的客户对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: df34248e6977752504f1f1c8f0997fbc0fa8f434
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045633"
---
# <a name="get-customers"></a><span data-ttu-id="73289-103">获取客户</span><span class="sxs-lookup"><span data-stu-id="73289-103">Get customers</span></span>

<span data-ttu-id="73289-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73289-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73289-105">检索 Dynamics 365 Business Central 的客户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73289-105">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="73289-106">权限</span><span class="sxs-lookup"><span data-stu-id="73289-106">Permissions</span></span>
<span data-ttu-id="73289-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73289-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73289-109">Permission type</span></span> |<span data-ttu-id="73289-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73289-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="73289-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73289-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73289-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73289-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="73289-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="73289-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="73289-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73289-114">Not supported.</span></span>|
|<span data-ttu-id="73289-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73289-115">Application</span></span>|<span data-ttu-id="73289-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73289-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73289-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73289-117">HTTP request</span></span>
```
GET /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73289-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73289-118">Optional query parameters</span></span>
<span data-ttu-id="73289-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73289-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73289-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73289-120">Request headers</span></span>
|<span data-ttu-id="73289-121">标头</span><span class="sxs-lookup"><span data-stu-id="73289-121">Header</span></span>|<span data-ttu-id="73289-122">值</span><span class="sxs-lookup"><span data-stu-id="73289-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="73289-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73289-123">Authorization</span></span>  |<span data-ttu-id="73289-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73289-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73289-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73289-126">Request body</span></span>
<span data-ttu-id="73289-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73289-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73289-128">响应</span><span class="sxs-lookup"><span data-stu-id="73289-128">Response</span></span>
<span data-ttu-id="73289-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **customers** 对象。</span><span class="sxs-lookup"><span data-stu-id="73289-129">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="73289-130">**请求**</span><span class="sxs-lookup"><span data-stu-id="73289-130">**Request**</span></span>

<span data-ttu-id="73289-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73289-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
```

<span data-ttu-id="73289-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="73289-132">**Response**</span></span>

<span data-ttu-id="73289-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73289-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="73289-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="73289-134">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
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
  "currencyId": "currencyId-value",
  "currencyCode": "USD",
  "paymentTermsId": "paymentTermsId-value",
  "shipmentMethodId": "shipmentMethodId-value",
  "paymentMethodId": "paymentMethodId-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```



