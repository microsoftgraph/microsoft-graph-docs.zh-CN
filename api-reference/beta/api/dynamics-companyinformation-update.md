---
title: 更新 companyInformation
description: 更新 Dynamics 365 Business Central 中的公司信息对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: eb94bf97caa58724286f464416884a179a1e1023
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473411"
---
# <a name="update-companyinformation"></a><span data-ttu-id="7c8be-103">更新 companyInformation</span><span class="sxs-lookup"><span data-stu-id="7c8be-103">Update companyInformation</span></span>

<span data-ttu-id="7c8be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c8be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c8be-105">更新 Dynamics 365 Business Central 的公司信息对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7c8be-105">Update the properties of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c8be-106">权限</span><span class="sxs-lookup"><span data-stu-id="7c8be-106">Permissions</span></span>
<span data-ttu-id="7c8be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c8be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c8be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c8be-109">Permission type</span></span> |<span data-ttu-id="7c8be-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c8be-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7c8be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c8be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c8be-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c8be-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7c8be-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="7c8be-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7c8be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c8be-114">Not supported.</span></span>|
|<span data-ttu-id="7c8be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c8be-115">Application</span></span>|<span data-ttu-id="7c8be-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c8be-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c8be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c8be-117">HTTP request</span></span>
```http
PATCH /financials/companies/{id}/companyInformation/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c8be-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7c8be-118">Optional query parameters</span></span>
<span data-ttu-id="7c8be-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7c8be-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c8be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c8be-120">Request headers</span></span>
|<span data-ttu-id="7c8be-121">标头</span><span class="sxs-lookup"><span data-stu-id="7c8be-121">Header</span></span>        |<span data-ttu-id="7c8be-122">值</span><span class="sxs-lookup"><span data-stu-id="7c8be-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="7c8be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c8be-123">Authorization</span></span> |<span data-ttu-id="7c8be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c8be-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7c8be-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c8be-126">Content-Type</span></span>  |<span data-ttu-id="7c8be-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c8be-127">application/json</span></span>         |
|<span data-ttu-id="7c8be-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="7c8be-128">If-Match</span></span>      |<span data-ttu-id="7c8be-129">必填。</span><span class="sxs-lookup"><span data-stu-id="7c8be-129">Required.</span></span> <span data-ttu-id="7c8be-130">如果包含此请求标头，并且提供的 eTag 与 **companyInformation** 上的当前标记不匹配，将不会更新 **companyInformation。**</span><span class="sxs-lookup"><span data-stu-id="7c8be-130">When this request header is included and the eTag provided does not match the current tag on the **companyInformation**, the **companyInformation** will not be updated.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c8be-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c8be-131">Request body</span></span>
<span data-ttu-id="7c8be-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7c8be-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="7c8be-135">响应</span><span class="sxs-lookup"><span data-stu-id="7c8be-135">Response</span></span>
<span data-ttu-id="7c8be-136">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` **companyInformation** 对象。</span><span class="sxs-lookup"><span data-stu-id="7c8be-136">If successful, this method returns a `200 OK` response code and an updated an **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c8be-137">示例</span><span class="sxs-lookup"><span data-stu-id="7c8be-137">Example</span></span>

<span data-ttu-id="7c8be-138">**请求**</span><span class="sxs-lookup"><span data-stu-id="7c8be-138">**Request**</span></span>

<span data-ttu-id="7c8be-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c8be-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/companyInformation/{id}
Content-type: application/json

{
  "displayName": "CRONUS USA, LTD.",
  "website": "www.cronuscorp.net"
}
```

<span data-ttu-id="7c8be-140">**响应**</span><span class="sxs-lookup"><span data-stu-id="7c8be-140">**Response**</span></span>

<span data-ttu-id="7c8be-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7c8be-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="7c8be-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7c8be-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7c8be-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7c8be-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "displayName": "CRONUS USA, LTD.",
  "address": {
    "street": "7122 South Ashford Street\r\nWestminster",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "+1 425 555 0100",
  "faxNumber": "+1 425 555 0101",
  "email": "",
  "website": "www.cronuscorp.net",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/companyInformation/{id}/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
  }
```


