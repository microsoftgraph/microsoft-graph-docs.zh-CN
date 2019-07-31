---
title: 创建项目
description: 在 Dynamics 365 Business Central 中创建 item 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: db6622a6f58bb4fb84a19b56b62f20d305fc74f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956665"
---
# <a name="create-items"></a><span data-ttu-id="77877-103">创建项目</span><span class="sxs-lookup"><span data-stu-id="77877-103">Create items</span></span>
<span data-ttu-id="77877-104">在 Dynamics 365 Business Central 中创建一个项目, 以便在发票、报价等上使用。</span><span class="sxs-lookup"><span data-stu-id="77877-104">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="77877-105">权限</span><span class="sxs-lookup"><span data-stu-id="77877-105">Permissions</span></span>
<span data-ttu-id="77877-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77877-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77877-108">Permission type</span></span> |<span data-ttu-id="77877-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77877-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="77877-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77877-110">Delegated (work or school account)</span></span>|<span data-ttu-id="77877-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77877-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="77877-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="77877-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="77877-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="77877-113">Not supported.</span></span>|
|<span data-ttu-id="77877-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77877-114">Application</span></span>|<span data-ttu-id="77877-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77877-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77877-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77877-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77877-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77877-117">Optional query parameters</span></span>
<span data-ttu-id="77877-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="77877-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77877-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="77877-119">Request headers</span></span>
|<span data-ttu-id="77877-120">标头</span><span class="sxs-lookup"><span data-stu-id="77877-120">Header</span></span>       |<span data-ttu-id="77877-121">值</span><span class="sxs-lookup"><span data-stu-id="77877-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="77877-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77877-122">Authorization</span></span>|<span data-ttu-id="77877-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77877-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="77877-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77877-125">Content-Type</span></span> |<span data-ttu-id="77877-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77877-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="77877-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77877-127">Request body</span></span>
<span data-ttu-id="77877-128">在请求正文中, 提供**items**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77877-128">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="77877-129">响应</span><span class="sxs-lookup"><span data-stu-id="77877-129">Response</span></span>
<span data-ttu-id="77877-130">如果成功, 此方法在```201 Created```响应正文中返回响应代码和**items**对象。</span><span class="sxs-lookup"><span data-stu-id="77877-130">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77877-131">示例</span><span class="sxs-lookup"><span data-stu-id="77877-131">Example</span></span>
<span data-ttu-id="77877-132">**请求**</span><span class="sxs-lookup"><span data-stu-id="77877-132">**Request**</span></span>

<span data-ttu-id="77877-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77877-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/items
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

<span data-ttu-id="77877-134">**响应**</span><span class="sxs-lookup"><span data-stu-id="77877-134">**Response**</span></span>

<span data-ttu-id="77877-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77877-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="77877-136">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77877-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77877-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="77877-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```

