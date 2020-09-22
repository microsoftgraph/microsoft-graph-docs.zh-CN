---
title: 创建 countriesRegions
description: 在 Dynamics 365 Business Central 中创建国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6d130b26205dc699b10cc93d504326b9f162b8ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008371"
---
# <a name="create-countriesregions"></a><span data-ttu-id="d8376-103">创建 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="d8376-103">Create countriesRegions</span></span>

<span data-ttu-id="d8376-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8376-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8376-105">在 Dynamics 365 Business Central 中创建一个 countriesRegions 对象。</span><span class="sxs-lookup"><span data-stu-id="d8376-105">Create a countriesRegions object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8376-106">权限</span><span class="sxs-lookup"><span data-stu-id="d8376-106">Permissions</span></span>
<span data-ttu-id="d8376-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8376-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8376-109">Permission type</span></span> |<span data-ttu-id="d8376-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8376-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d8376-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8376-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8376-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8376-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d8376-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="d8376-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d8376-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8376-114">Not supported.</span></span>|
|<span data-ttu-id="d8376-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8376-115">Application</span></span>|<span data-ttu-id="d8376-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8376-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8376-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8376-117">HTTP request</span></span>
```
POST /financials/companies/{id}/countriesRegions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8376-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d8376-118">Optional query parameters</span></span>
<span data-ttu-id="d8376-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d8376-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8376-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8376-120">Request headers</span></span>
|<span data-ttu-id="d8376-121">标头</span><span class="sxs-lookup"><span data-stu-id="d8376-121">Header</span></span>|<span data-ttu-id="d8376-122">值</span><span class="sxs-lookup"><span data-stu-id="d8376-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="d8376-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8376-123">Authorization</span></span>  |<span data-ttu-id="d8376-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8376-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d8376-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8376-126">Content-Type</span></span>  |<span data-ttu-id="d8376-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d8376-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="d8376-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8376-128">Request body</span></span>
<span data-ttu-id="d8376-129">在请求正文中，提供 **countriesRegions** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8376-129">In the request body, supply a JSON representation of **countriesRegions** object.</span></span>

## <a name="response"></a><span data-ttu-id="d8376-130">响应</span><span class="sxs-lookup"><span data-stu-id="d8376-130">Response</span></span>
<span data-ttu-id="d8376-131">如果成功，此方法 ```201 Created``` 在响应正文中返回响应代码和 **countriesRegions** 对象。</span><span class="sxs-lookup"><span data-stu-id="d8376-131">If successful, this method returns ```201 Created``` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8376-132">示例</span><span class="sxs-lookup"><span data-stu-id="d8376-132">Example</span></span>

<span data-ttu-id="d8376-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="d8376-133">**Request**</span></span>

<span data-ttu-id="d8376-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8376-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions
Content-type: application/json

{
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code"
}
```

<span data-ttu-id="d8376-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="d8376-135">**Response**</span></span>

<span data-ttu-id="d8376-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d8376-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="d8376-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d8376-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8376-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d8376-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}

```



