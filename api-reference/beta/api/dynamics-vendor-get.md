---
title: 获取供应商
description: 获取 Dynamics 365 Business Central 中的供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6d701590a8a0d571075eca114930d0bfbdf5a50b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044814"
---
# <a name="get-vendors"></a><span data-ttu-id="1e9e2-103">获取供应商</span><span class="sxs-lookup"><span data-stu-id="1e9e2-103">Get vendors</span></span>

<span data-ttu-id="1e9e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e9e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e9e2-105">检索 Dynamics 365 Business Central 的供应商对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-105">Retrieve the properties and relationships of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e9e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="1e9e2-106">Permissions</span></span>
<span data-ttu-id="1e9e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e9e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e9e2-109">Permission type</span></span> |<span data-ttu-id="1e9e2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e9e2-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="1e9e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e9e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e9e2-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e9e2-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="1e9e2-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="1e9e2-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1e9e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-114">Not supported.</span></span>|
|<span data-ttu-id="1e9e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e9e2-115">Application</span></span>|<span data-ttu-id="1e9e2-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e9e2-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e9e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e9e2-117">HTTP request</span></span>

```http
GET /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e9e2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e9e2-118">Optional query parameters</span></span>
<span data-ttu-id="1e9e2-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e9e2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e9e2-120">Request headers</span></span>
|<span data-ttu-id="1e9e2-121">标头</span><span class="sxs-lookup"><span data-stu-id="1e9e2-121">Header</span></span>|<span data-ttu-id="1e9e2-122">值</span><span class="sxs-lookup"><span data-stu-id="1e9e2-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="1e9e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e9e2-123">Authorization</span></span>  |<span data-ttu-id="1e9e2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e9e2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e9e2-126">Request body</span></span>
<span data-ttu-id="1e9e2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e9e2-128">响应</span><span class="sxs-lookup"><span data-stu-id="1e9e2-128">Response</span></span>
<span data-ttu-id="1e9e2-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和供应商对象。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-129">If successful, this method returns a `200 OK` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e9e2-130">示例</span><span class="sxs-lookup"><span data-stu-id="1e9e2-130">Example</span></span>

<span data-ttu-id="1e9e2-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="1e9e2-131">**Request**</span></span>

<span data-ttu-id="1e9e2-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="1e9e2-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="1e9e2-133">**Response**</span></span>

<span data-ttu-id="1e9e2-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="1e9e2-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-135">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyId": "id-value",
  "currencyCode": "USD",
  "irs1099Code": "",
  "paymentTermsId": "id-value",
  "paymentMethodId": "id-value",
  "taxLiable": true,
  "blocked": " ",
  "balance": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:29.667Z"
}
```




