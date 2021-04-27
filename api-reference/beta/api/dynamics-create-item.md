---
title: 创建项目
description: 在 Dynamics 365 Business Central 创建项目对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 544155babf455cf013ca3bd2979f64ba8cb37d8c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045934"
---
# <a name="create-items"></a><span data-ttu-id="55f70-103">创建项目</span><span class="sxs-lookup"><span data-stu-id="55f70-103">Create items</span></span>

<span data-ttu-id="55f70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55f70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55f70-105">在 Dynamics 365 Business Central 创建用于发票、报价等的项目。</span><span class="sxs-lookup"><span data-stu-id="55f70-105">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="55f70-106">权限</span><span class="sxs-lookup"><span data-stu-id="55f70-106">Permissions</span></span>
<span data-ttu-id="55f70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55f70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55f70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="55f70-109">Permission type</span></span> |<span data-ttu-id="55f70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55f70-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="55f70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55f70-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55f70-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55f70-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="55f70-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="55f70-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="55f70-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="55f70-114">Not supported.</span></span>|
|<span data-ttu-id="55f70-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="55f70-115">Application</span></span>|<span data-ttu-id="55f70-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55f70-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55f70-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55f70-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55f70-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="55f70-118">Optional query parameters</span></span>
<span data-ttu-id="55f70-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="55f70-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55f70-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="55f70-120">Request headers</span></span>
|<span data-ttu-id="55f70-121">标头</span><span class="sxs-lookup"><span data-stu-id="55f70-121">Header</span></span>       |<span data-ttu-id="55f70-122">值</span><span class="sxs-lookup"><span data-stu-id="55f70-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="55f70-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55f70-123">Authorization</span></span>|<span data-ttu-id="55f70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55f70-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="55f70-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55f70-126">Content-Type</span></span> |<span data-ttu-id="55f70-127">application/json</span><span class="sxs-lookup"><span data-stu-id="55f70-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="55f70-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="55f70-128">Request body</span></span>
<span data-ttu-id="55f70-129">在请求正文中，提供 items 对象的 JSON **表示** 形式。</span><span class="sxs-lookup"><span data-stu-id="55f70-129">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="55f70-130">响应</span><span class="sxs-lookup"><span data-stu-id="55f70-130">Response</span></span>
<span data-ttu-id="55f70-131">如果成功，此方法在 ```201 Created``` 响应正文中返回 响应代码和 **items** 对象。</span><span class="sxs-lookup"><span data-stu-id="55f70-131">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55f70-132">示例</span><span class="sxs-lookup"><span data-stu-id="55f70-132">Example</span></span>
<span data-ttu-id="55f70-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="55f70-133">**Request**</span></span>

<span data-ttu-id="55f70-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55f70-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/items
Content-type: application/json

{
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "65bdbd3a-39f1-49f4-bf24-598cbac36230",
  "gtin": "",
  "itemCategoryId": "5b0b9c1c-312d-4809-96b2-056690a11057",
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupCode": "FURNITURE"
} 

```

<span data-ttu-id="55f70-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="55f70-135">**Response**</span></span>

<span data-ttu-id="55f70-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55f70-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="55f70-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="55f70-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```



