---
title: 获取 countriesRegions
description: 获取 Dynamics 365 Business Central 中的国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 30916ec2fd6bd00f92a5ad96be05400d7ec4c92f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008368"
---
# <a name="get-countriesregions"></a><span data-ttu-id="c3e5e-103">获取 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="c3e5e-103">Get countriesRegions</span></span>

<span data-ttu-id="c3e5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e5e-105">检索 countriesRegions 对象的属性和关系，以实现 Dynamics 365 Business Central。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-105">Retrieve the properties and relationships of a countriesRegions object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3e5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="c3e5e-106">Permissions</span></span>
<span data-ttu-id="c3e5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3e5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3e5e-109">Permission type</span></span> |<span data-ttu-id="c3e5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3e5e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c3e5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3e5e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3e5e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3e5e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c3e5e-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="c3e5e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c3e5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-114">Not supported.</span></span>|
|<span data-ttu-id="c3e5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3e5e-115">Application</span></span>|<span data-ttu-id="c3e5e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3e5e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3e5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3e5e-117">HTTP request</span></span>
```
GET /financials/companies/{id}/countriesRegions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3e5e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c3e5e-118">Optional query parameters</span></span>
<span data-ttu-id="c3e5e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3e5e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3e5e-120">Request headers</span></span>
|<span data-ttu-id="c3e5e-121">标头</span><span class="sxs-lookup"><span data-stu-id="c3e5e-121">Header</span></span>|<span data-ttu-id="c3e5e-122">值</span><span class="sxs-lookup"><span data-stu-id="c3e5e-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="c3e5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3e5e-123">Authorization</span></span>  |<span data-ttu-id="c3e5e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3e5e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3e5e-126">Request body</span></span>
<span data-ttu-id="c3e5e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3e5e-128">响应</span><span class="sxs-lookup"><span data-stu-id="c3e5e-128">Response</span></span>
<span data-ttu-id="c3e5e-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **countriesRegions** 对象。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-129">If successful, this method returns a `200 OK` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3e5e-130">示例</span><span class="sxs-lookup"><span data-stu-id="c3e5e-130">Example</span></span>

<span data-ttu-id="c3e5e-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="c3e5e-131">**Request**</span></span>

<span data-ttu-id="c3e5e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
```

<span data-ttu-id="c3e5e-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="c3e5e-133">**Response**</span></span>

<span data-ttu-id="c3e5e-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="c3e5e-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c3e5e-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c3e5e-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}
```


