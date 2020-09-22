---
title: 创建货币
description: 在 Dynamics 365 Business Central 中创建货币对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: eb78fef62cb2d17e622c11cbd575905b60656f79
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981728"
---
# <a name="create-currencies"></a><span data-ttu-id="b6268-103">创建货币</span><span class="sxs-lookup"><span data-stu-id="b6268-103">Create currencies</span></span>

<span data-ttu-id="b6268-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6268-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6268-105">在 Dynamics 365 Business Central 中创建货币对象。</span><span class="sxs-lookup"><span data-stu-id="b6268-105">Create a currency object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6268-106">权限</span><span class="sxs-lookup"><span data-stu-id="b6268-106">Permissions</span></span>
<span data-ttu-id="b6268-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6268-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6268-109">Permission type</span></span> |<span data-ttu-id="b6268-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6268-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b6268-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6268-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6268-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6268-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b6268-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="b6268-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b6268-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6268-114">Not supported.</span></span>|
|<span data-ttu-id="b6268-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6268-115">Application</span></span>|<span data-ttu-id="b6268-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6268-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6268-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6268-117">HTTP request</span></span>
```
POST /financials/companies/{id}/currencies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6268-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b6268-118">Optional query parameters</span></span>
<span data-ttu-id="b6268-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b6268-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6268-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6268-120">Request headers</span></span>
|<span data-ttu-id="b6268-121">标头</span><span class="sxs-lookup"><span data-stu-id="b6268-121">Header</span></span>         |<span data-ttu-id="b6268-122">值</span><span class="sxs-lookup"><span data-stu-id="b6268-122">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="b6268-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6268-123">Authorization</span></span>  |<span data-ttu-id="b6268-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6268-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b6268-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6268-126">Content-Type</span></span>   |<span data-ttu-id="b6268-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b6268-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="b6268-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6268-128">Request body</span></span>
<span data-ttu-id="b6268-129">在请求正文中，提供 **货币** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6268-129">In the request body, supply a JSON representation of **currencies** object.</span></span>

## <a name="response"></a><span data-ttu-id="b6268-130">响应</span><span class="sxs-lookup"><span data-stu-id="b6268-130">Response</span></span>
<span data-ttu-id="b6268-131">如果成功，此方法 ```201 Created``` 在响应正文中返回响应代码和 **货币** 对象。</span><span class="sxs-lookup"><span data-stu-id="b6268-131">If successful, this method returns ```201 Created``` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6268-132">示例</span><span class="sxs-lookup"><span data-stu-id="b6268-132">Example</span></span>

<span data-ttu-id="b6268-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="b6268-133">**Request**</span></span>

<span data-ttu-id="b6268-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6268-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/currencies
Content-type: application/json

{
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01
}
```

<span data-ttu-id="b6268-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="b6268-135">**Response**</span></span>

<span data-ttu-id="b6268-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b6268-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="b6268-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b6268-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6268-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b6268-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.002Z"
}

```


