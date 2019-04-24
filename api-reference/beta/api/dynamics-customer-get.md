---
title: 获取客户
description: 获取 Dynamics 365 Business Central 中的 customer 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0512a493032e738bba41362ecdc40e78de951baf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458591"
---
# <a name="get-customers"></a><span data-ttu-id="3ac6a-103">获取客户</span><span class="sxs-lookup"><span data-stu-id="3ac6a-103">Get customers</span></span>
<span data-ttu-id="3ac6a-104">检索 Dynamics 365 Business Central 的 customer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-104">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ac6a-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ac6a-105">Permissions</span></span>
<span data-ttu-id="3ac6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ac6a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ac6a-108">Permission type</span></span> |<span data-ttu-id="3ac6a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ac6a-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3ac6a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ac6a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3ac6a-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ac6a-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3ac6a-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="3ac6a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3ac6a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-113">Not supported.</span></span>|
|<span data-ttu-id="3ac6a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ac6a-114">Application</span></span>|<span data-ttu-id="3ac6a-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ac6a-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ac6a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ac6a-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/customers('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ac6a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3ac6a-117">Optional query parameters</span></span>
<span data-ttu-id="3ac6a-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ac6a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ac6a-119">Request headers</span></span>
|<span data-ttu-id="3ac6a-120">标头</span><span class="sxs-lookup"><span data-stu-id="3ac6a-120">Header</span></span>|<span data-ttu-id="3ac6a-121">值</span><span class="sxs-lookup"><span data-stu-id="3ac6a-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="3ac6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ac6a-122">Authorization</span></span>  |<span data-ttu-id="3ac6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ac6a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ac6a-125">Request body</span></span>
<span data-ttu-id="3ac6a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ac6a-127">响应</span><span class="sxs-lookup"><span data-stu-id="3ac6a-127">Response</span></span>
<span data-ttu-id="3ac6a-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**customers**对象。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-128">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="3ac6a-129">**请求**</span><span class="sxs-lookup"><span data-stu-id="3ac6a-129">**Request**</span></span>

<span data-ttu-id="3ac6a-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/customers('{id}')
```

<span data-ttu-id="3ac6a-131">**响应**</span><span class="sxs-lookup"><span data-stu-id="3ac6a-131">**Response**</span></span>

<span data-ttu-id="3ac6a-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="3ac6a-133">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ac6a-134">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ac6a-134">All the properties will be returned from an actual call.</span></span>

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

