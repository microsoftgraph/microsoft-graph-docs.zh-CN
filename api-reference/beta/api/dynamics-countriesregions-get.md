---
title: 获取 countriesRegions
description: 获取 Dynamics 365 Business Central 中的国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0dd701cfff4b730c97d5c92ce2ed2134fced81fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454144"
---
# <a name="get-countriesregions"></a><span data-ttu-id="12322-103">获取 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="12322-103">Get countriesRegions</span></span>
<span data-ttu-id="12322-104">检索 countriesRegions 对象的属性和关系, 以实现 Dynamics 365 Business Central。</span><span class="sxs-lookup"><span data-stu-id="12322-104">Retrieve the properties and relationships of a countriesRegions object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="12322-105">权限</span><span class="sxs-lookup"><span data-stu-id="12322-105">Permissions</span></span>
<span data-ttu-id="12322-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12322-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="12322-108">Permission type</span></span> |<span data-ttu-id="12322-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12322-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="12322-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12322-110">Delegated (work or school account)</span></span>|<span data-ttu-id="12322-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12322-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="12322-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="12322-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="12322-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="12322-113">Not supported.</span></span>|
|<span data-ttu-id="12322-114">Application</span><span class="sxs-lookup"><span data-stu-id="12322-114">Application</span></span>|<span data-ttu-id="12322-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12322-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12322-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12322-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/countriesRegions('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12322-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="12322-117">Optional query parameters</span></span>
<span data-ttu-id="12322-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="12322-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12322-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12322-119">Request headers</span></span>
|<span data-ttu-id="12322-120">标头</span><span class="sxs-lookup"><span data-stu-id="12322-120">Header</span></span>|<span data-ttu-id="12322-121">值</span><span class="sxs-lookup"><span data-stu-id="12322-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="12322-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12322-122">Authorization</span></span>  |<span data-ttu-id="12322-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12322-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12322-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="12322-125">Request body</span></span>
<span data-ttu-id="12322-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12322-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12322-127">响应</span><span class="sxs-lookup"><span data-stu-id="12322-127">Response</span></span>
<span data-ttu-id="12322-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**countriesRegions**对象。</span><span class="sxs-lookup"><span data-stu-id="12322-128">If successful, this method returns a `200 OK` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12322-129">示例</span><span class="sxs-lookup"><span data-stu-id="12322-129">Example</span></span>

<span data-ttu-id="12322-130">**请求**</span><span class="sxs-lookup"><span data-stu-id="12322-130">**Request**</span></span>

<span data-ttu-id="12322-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12322-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/countriesRegions('{id}')
```

<span data-ttu-id="12322-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="12322-132">**Response**</span></span>

<span data-ttu-id="12322-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="12322-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="12322-134">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="12322-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="12322-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="12322-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}
```
