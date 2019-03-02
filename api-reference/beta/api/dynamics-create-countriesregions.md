---
title: 创建 countriesRegions
description: 在 Dynamics 365 Business Central 中创建国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a78ba9ce04dc1b9a5a39cf9e742de7503afc9c3f
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365407"
---
# <a name="create-countriesregions"></a><span data-ttu-id="2ea1e-103">创建 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="2ea1e-103">Create countriesRegions</span></span>
<span data-ttu-id="2ea1e-104">在 Dynamics 365 Business Central 中创建一个 countriesRegions 对象。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-104">Create a countriesRegions object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ea1e-105">权限</span><span class="sxs-lookup"><span data-stu-id="2ea1e-105">Permissions</span></span>
<span data-ttu-id="2ea1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ea1e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ea1e-108">Permission type</span></span> |<span data-ttu-id="2ea1e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ea1e-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2ea1e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ea1e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2ea1e-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ea1e-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2ea1e-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="2ea1e-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2ea1e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-113">Not supported.</span></span>|
|<span data-ttu-id="2ea1e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ea1e-114">Application</span></span>|<span data-ttu-id="2ea1e-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ea1e-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ea1e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ea1e-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/countriesRegions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ea1e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ea1e-117">Optional query parameters</span></span>
<span data-ttu-id="2ea1e-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ea1e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ea1e-119">Request headers</span></span>
|<span data-ttu-id="2ea1e-120">标头</span><span class="sxs-lookup"><span data-stu-id="2ea1e-120">Header</span></span>|<span data-ttu-id="2ea1e-121">值</span><span class="sxs-lookup"><span data-stu-id="2ea1e-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="2ea1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ea1e-122">Authorization</span></span>  |<span data-ttu-id="2ea1e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="2ea1e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ea1e-125">Content-Type</span></span>  |<span data-ttu-id="2ea1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ea1e-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="2ea1e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ea1e-127">Request body</span></span>
<span data-ttu-id="2ea1e-128">在请求正文中, 提供**countriesRegions**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-128">In the request body, supply a JSON representation of **countriesRegions** object.</span></span>

## <a name="response"></a><span data-ttu-id="2ea1e-129">响应</span><span class="sxs-lookup"><span data-stu-id="2ea1e-129">Response</span></span>
<span data-ttu-id="2ea1e-130">如果成功, 此方法在```201 Created```响应正文中返回响应代码和**countriesRegions**对象。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-130">If successful, this method returns ```201 Created``` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ea1e-131">示例</span><span class="sxs-lookup"><span data-stu-id="2ea1e-131">Example</span></span>

<span data-ttu-id="2ea1e-132">**请求**</span><span class="sxs-lookup"><span data-stu-id="2ea1e-132">**Request**</span></span>

<span data-ttu-id="2ea1e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/countriesRegions
Content-type: application/json

{
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code"
}
```

<span data-ttu-id="2ea1e-134">**响应**</span><span class="sxs-lookup"><span data-stu-id="2ea1e-134">**Response**</span></span>

<span data-ttu-id="2ea1e-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="2ea1e-136">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2ea1e-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2ea1e-137">All the properties will be returned from an actual call.</span></span>

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

