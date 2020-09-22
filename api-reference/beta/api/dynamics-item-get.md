---
title: 获取项目
description: 获取 Dynamics 365 Business Central 中的 item 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b73ecaa3b201143a61f1ea0cf514d848ffa46f37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981266"
---
# <a name="get-items"></a><span data-ttu-id="bb043-103">获取项目</span><span class="sxs-lookup"><span data-stu-id="bb043-103">Get items</span></span>

<span data-ttu-id="bb043-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb043-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb043-105">检索 Dynamics 365 Business Central 的 item 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb043-105">Retrieve the properties and relationships of an item object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb043-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb043-106">Permissions</span></span>
<span data-ttu-id="bb043-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb043-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb043-109">Permission type</span></span> |<span data-ttu-id="bb043-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb043-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="bb043-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb043-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb043-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb043-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="bb043-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="bb043-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bb043-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb043-114">Not supported.</span></span>|
|<span data-ttu-id="bb043-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb043-115">Application</span></span>|<span data-ttu-id="bb043-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb043-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb043-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb043-117">HTTP request</span></span>

```
GET /financials/companies/{id}/items/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb043-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb043-118">Optional query parameters</span></span>
<span data-ttu-id="bb043-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb043-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb043-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb043-120">Request headers</span></span>
|<span data-ttu-id="bb043-121">标头</span><span class="sxs-lookup"><span data-stu-id="bb043-121">Header</span></span>       |<span data-ttu-id="bb043-122">值</span><span class="sxs-lookup"><span data-stu-id="bb043-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="bb043-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb043-123">Authorization</span></span>|<span data-ttu-id="bb043-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb043-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb043-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb043-126">Request body</span></span>
<span data-ttu-id="bb043-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb043-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb043-128">响应</span><span class="sxs-lookup"><span data-stu-id="bb043-128">Response</span></span>
<span data-ttu-id="bb043-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **items** 对象。</span><span class="sxs-lookup"><span data-stu-id="bb043-129">If successful, this method returns a `200 OK` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb043-130">示例</span><span class="sxs-lookup"><span data-stu-id="bb043-130">Example</span></span>
<span data-ttu-id="bb043-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="bb043-131">**Request**</span></span>

<span data-ttu-id="bb043-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb043-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/items/{id}
```

<span data-ttu-id="bb043-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="bb043-133">**Response**</span></span>

<span data-ttu-id="bb043-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bb043-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="bb043-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bb043-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bb043-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bb043-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "id-value",
  "gtin": "",
  "itemCategoryId": "id-value"
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupId": "id-value",
  "taxGroupCode": "FURNITURE",
  "lastModifiedDateTime": "2017-03-07T00:35:30.073Z"
}

```



