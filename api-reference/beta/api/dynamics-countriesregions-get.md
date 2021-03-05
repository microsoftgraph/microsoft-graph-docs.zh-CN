---
title: 获取 countriesRegions
description: 获取 Dynamics 365 Business Central 中的国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 678151c8c03de09a1e72d7ce15bb1e8e7bf82b60
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473383"
---
# <a name="get-countriesregions"></a><span data-ttu-id="e0030-103">获取 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="e0030-103">Get countriesRegions</span></span>

<span data-ttu-id="e0030-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0030-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0030-105">检索 Dynamics 365 Business Central 的 CountriesRegions 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0030-105">Retrieve the properties and relationships of a countriesRegions object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0030-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0030-106">Permissions</span></span>
<span data-ttu-id="e0030-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0030-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0030-109">Permission type</span></span> |<span data-ttu-id="e0030-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0030-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e0030-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0030-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0030-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0030-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e0030-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e0030-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e0030-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0030-114">Not supported.</span></span>|
|<span data-ttu-id="e0030-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0030-115">Application</span></span>|<span data-ttu-id="e0030-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0030-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0030-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0030-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/countriesRegions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0030-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e0030-118">Optional query parameters</span></span>
<span data-ttu-id="e0030-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e0030-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0030-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0030-120">Request headers</span></span>
|<span data-ttu-id="e0030-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0030-121">Header</span></span>|<span data-ttu-id="e0030-122">值</span><span class="sxs-lookup"><span data-stu-id="e0030-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="e0030-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0030-123">Authorization</span></span>  |<span data-ttu-id="e0030-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0030-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0030-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0030-126">Request body</span></span>
<span data-ttu-id="e0030-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0030-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0030-128">响应</span><span class="sxs-lookup"><span data-stu-id="e0030-128">Response</span></span>
<span data-ttu-id="e0030-129">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 **countriesRegions** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0030-129">If successful, this method returns a `200 OK` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0030-130">示例</span><span class="sxs-lookup"><span data-stu-id="e0030-130">Example</span></span>

<span data-ttu-id="e0030-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="e0030-131">**Request**</span></span>

<span data-ttu-id="e0030-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0030-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
```

<span data-ttu-id="e0030-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="e0030-133">**Response**</span></span>

<span data-ttu-id="e0030-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0030-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="e0030-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0030-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e0030-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0030-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}
```


