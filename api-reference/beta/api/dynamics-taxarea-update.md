---
title: 更新 taxAreas
description: 更新 Dynamics 365 Business Central 中的税务区域对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a2f8a3321b1143d367ce4c256e97cf42af77b100
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474167"
---
# <a name="update-taxareas"></a><span data-ttu-id="31c3f-103">更新 taxAreas</span><span class="sxs-lookup"><span data-stu-id="31c3f-103">Update taxAreas</span></span>

<span data-ttu-id="31c3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31c3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31c3f-105">更新 Dynamics 365 商业中心税区对象的属性。</span><span class="sxs-lookup"><span data-stu-id="31c3f-105">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="31c3f-106">权限</span><span class="sxs-lookup"><span data-stu-id="31c3f-106">Permissions</span></span>
<span data-ttu-id="31c3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31c3f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31c3f-109">Permission type</span></span> |<span data-ttu-id="31c3f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31c3f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="31c3f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31c3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31c3f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c3f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="31c3f-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="31c3f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="31c3f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31c3f-114">Not supported.</span></span>|
|<span data-ttu-id="31c3f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31c3f-115">Application</span></span>|<span data-ttu-id="31c3f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c3f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31c3f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31c3f-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31c3f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31c3f-118">Optional query parameters</span></span>
<span data-ttu-id="31c3f-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31c3f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31c3f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="31c3f-120">Request headers</span></span>
|<span data-ttu-id="31c3f-121">标头</span><span class="sxs-lookup"><span data-stu-id="31c3f-121">Header</span></span>|<span data-ttu-id="31c3f-122">值</span><span class="sxs-lookup"><span data-stu-id="31c3f-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="31c3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31c3f-123">Authorization</span></span> |<span data-ttu-id="31c3f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31c3f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="31c3f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31c3f-126">Content-Type</span></span>  |<span data-ttu-id="31c3f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="31c3f-127">application/json</span></span>|
|<span data-ttu-id="31c3f-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="31c3f-128">If-Match</span></span>      |<span data-ttu-id="31c3f-129">必填。</span><span class="sxs-lookup"><span data-stu-id="31c3f-129">Required.</span></span> <span data-ttu-id="31c3f-130">如果包含此请求标头且提供的 eTag 与 **taxAreas** 上的当前标记不匹配，则 **taxAreas** 将不会更新。</span><span class="sxs-lookup"><span data-stu-id="31c3f-130">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31c3f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="31c3f-131">Request body</span></span>
<span data-ttu-id="31c3f-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="31c3f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="31c3f-135">响应</span><span class="sxs-lookup"><span data-stu-id="31c3f-135">Response</span></span>
<span data-ttu-id="31c3f-136">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` **taxAreas** 对象。</span><span class="sxs-lookup"><span data-stu-id="31c3f-136">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31c3f-137">示例</span><span class="sxs-lookup"><span data-stu-id="31c3f-137">Example</span></span>

<span data-ttu-id="31c3f-138">**请求**</span><span class="sxs-lookup"><span data-stu-id="31c3f-138">**Request**</span></span>

<span data-ttu-id="31c3f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31c3f-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="31c3f-140">**响应**</span><span class="sxs-lookup"><span data-stu-id="31c3f-140">**Response**</span></span>

<span data-ttu-id="31c3f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="31c3f-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="31c3f-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="31c3f-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31c3f-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="31c3f-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



