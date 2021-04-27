---
title: 创建供应商
description: 在 Dynamics 365 Business Central 创建供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 24e058f673e499aa58bf2c52765dc0c391412c07
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045680"
---
# <a name="create-vendors"></a><span data-ttu-id="78b9d-103">创建供应商</span><span class="sxs-lookup"><span data-stu-id="78b9d-103">Create vendors</span></span>

<span data-ttu-id="78b9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78b9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78b9d-105">在 Dynamics 365 Business Central 创建供应商对象。</span><span class="sxs-lookup"><span data-stu-id="78b9d-105">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="78b9d-106">权限</span><span class="sxs-lookup"><span data-stu-id="78b9d-106">Permissions</span></span>
<span data-ttu-id="78b9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78b9d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="78b9d-109">Permission type</span></span> |<span data-ttu-id="78b9d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78b9d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="78b9d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78b9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="78b9d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78b9d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="78b9d-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="78b9d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="78b9d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="78b9d-114">Not supported.</span></span>|
|<span data-ttu-id="78b9d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="78b9d-115">Application</span></span>|<span data-ttu-id="78b9d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78b9d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78b9d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78b9d-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78b9d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="78b9d-118">Optional query parameters</span></span>
<span data-ttu-id="78b9d-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="78b9d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78b9d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="78b9d-120">Request headers</span></span>
|<span data-ttu-id="78b9d-121">标头</span><span class="sxs-lookup"><span data-stu-id="78b9d-121">Header</span></span>|<span data-ttu-id="78b9d-122">值</span><span class="sxs-lookup"><span data-stu-id="78b9d-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="78b9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78b9d-123">Authorization</span></span>  |<span data-ttu-id="78b9d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78b9d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="78b9d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78b9d-126">Content-Type</span></span>  |<span data-ttu-id="78b9d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="78b9d-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="78b9d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="78b9d-128">Request body</span></span>
<span data-ttu-id="78b9d-129">在请求正文中，提供供应商对象的 JSON **表示形式** 。</span><span class="sxs-lookup"><span data-stu-id="78b9d-129">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="78b9d-130">响应</span><span class="sxs-lookup"><span data-stu-id="78b9d-130">Response</span></span>
<span data-ttu-id="78b9d-131">如果成功，此方法在 ```201 Created``` 响应正文中返回响应代码和供应商对象。</span><span class="sxs-lookup"><span data-stu-id="78b9d-131">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78b9d-132">示例</span><span class="sxs-lookup"><span data-stu-id="78b9d-132">Example</span></span>

<span data-ttu-id="78b9d-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="78b9d-133">**Request**</span></span>

<span data-ttu-id="78b9d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78b9d-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/vendors
Content-type: application/json

{
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
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": " "
}
```

<span data-ttu-id="78b9d-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="78b9d-135">**Response**</span></span>

<span data-ttu-id="78b9d-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78b9d-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="78b9d-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="78b9d-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```



