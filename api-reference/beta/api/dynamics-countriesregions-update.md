---
title: 更新 countriesRegions
description: 在 Dynamics 365 Business Central 中更新国家/地区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a1425ac005b214167fe63323a63eaaa40d2c9d92
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473607"
---
# <a name="update-countriesregions"></a><span data-ttu-id="310e0-103">更新 countriesRegions</span><span class="sxs-lookup"><span data-stu-id="310e0-103">Update countriesRegions</span></span>

<span data-ttu-id="310e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="310e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="310e0-105">更新 Dynamics 365 Business Central 的国家/地区对象的属性。</span><span class="sxs-lookup"><span data-stu-id="310e0-105">Update the properties of a country/region object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="310e0-106">权限</span><span class="sxs-lookup"><span data-stu-id="310e0-106">Permissions</span></span>
<span data-ttu-id="310e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="310e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="310e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="310e0-109">Permission type</span></span> |<span data-ttu-id="310e0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="310e0-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="310e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="310e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="310e0-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310e0-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="310e0-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="310e0-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="310e0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="310e0-114">Not supported.</span></span>|
|<span data-ttu-id="310e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="310e0-115">Application</span></span>|<span data-ttu-id="310e0-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310e0-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="310e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="310e0-117">HTTP request</span></span>
```http
PATCH /financials/companies/{id}/countriesRegions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="310e0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="310e0-118">Optional query parameters</span></span>
<span data-ttu-id="310e0-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="310e0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="310e0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="310e0-120">Request headers</span></span>
|<span data-ttu-id="310e0-121">标头</span><span class="sxs-lookup"><span data-stu-id="310e0-121">Header</span></span>|<span data-ttu-id="310e0-122">值</span><span class="sxs-lookup"><span data-stu-id="310e0-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="310e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="310e0-123">Authorization</span></span> |<span data-ttu-id="310e0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="310e0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="310e0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="310e0-126">Content-Type</span></span>  |<span data-ttu-id="310e0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="310e0-127">application/json</span></span>|
|<span data-ttu-id="310e0-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="310e0-128">If-Match</span></span>      |<span data-ttu-id="310e0-129">必填。</span><span class="sxs-lookup"><span data-stu-id="310e0-129">Required.</span></span> <span data-ttu-id="310e0-130">如果包含此请求标头且提供的 eTag 与 **countriesRegions** 上的当前标记不匹配，则 **countriesRegions** 将不会更新。</span><span class="sxs-lookup"><span data-stu-id="310e0-130">When this request header is included and the eTag provided does not match the current tag on the **countriesRegions**, the **countriesRegions** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="310e0-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="310e0-131">Request body</span></span>
<span data-ttu-id="310e0-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="310e0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="310e0-135">响应</span><span class="sxs-lookup"><span data-stu-id="310e0-135">Response</span></span>
<span data-ttu-id="310e0-136">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` **countriesRegions** 对象。</span><span class="sxs-lookup"><span data-stu-id="310e0-136">If successful, this method returns a `200 OK` response code and an updated **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="310e0-137">示例</span><span class="sxs-lookup"><span data-stu-id="310e0-137">Example</span></span>

<span data-ttu-id="310e0-138">**请求**</span><span class="sxs-lookup"><span data-stu-id="310e0-138">**Request**</span></span>

<span data-ttu-id="310e0-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="310e0-139">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
Content-type: application/json

{
  "displayName": "United States of America"
}
```

<span data-ttu-id="310e0-140">**响应**</span><span class="sxs-lookup"><span data-stu-id="310e0-140">**Response**</span></span>

<span data-ttu-id="310e0-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="310e0-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="310e0-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="310e0-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="310e0-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="310e0-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "United States of America",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-16T15:22:31.753Z"
}
```


