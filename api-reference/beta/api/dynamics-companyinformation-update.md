---
title: 更新 companyInformation
description: 更新 Dynamics 365 Business Central 中的公司信息对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4be5d9a0ba74e6c875b7051085538a76b0bf4bf9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956805"
---
# <a name="update-companyinformation"></a><span data-ttu-id="8e3dd-103">更新 companyInformation</span><span class="sxs-lookup"><span data-stu-id="8e3dd-103">Update companyInformation</span></span>
<span data-ttu-id="8e3dd-104">更新 Dynamics 365 Business Central 的公司信息对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-104">Update the properties of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e3dd-105">权限</span><span class="sxs-lookup"><span data-stu-id="8e3dd-105">Permissions</span></span>
<span data-ttu-id="8e3dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e3dd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e3dd-108">Permission type</span></span> |<span data-ttu-id="8e3dd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e3dd-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="8e3dd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e3dd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8e3dd-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3dd-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="8e3dd-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="8e3dd-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8e3dd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-113">Not supported.</span></span>|
|<span data-ttu-id="8e3dd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e3dd-114">Application</span></span>|<span data-ttu-id="8e3dd-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3dd-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e3dd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e3dd-116">HTTP request</span></span>
```
PATCH /financials/companies('{id}')/companyInformation('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e3dd-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8e3dd-117">Optional query parameters</span></span>
<span data-ttu-id="8e3dd-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e3dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e3dd-119">Request headers</span></span>
|<span data-ttu-id="8e3dd-120">标头</span><span class="sxs-lookup"><span data-stu-id="8e3dd-120">Header</span></span>        |<span data-ttu-id="8e3dd-121">值</span><span class="sxs-lookup"><span data-stu-id="8e3dd-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="8e3dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e3dd-122">Authorization</span></span> |<span data-ttu-id="8e3dd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8e3dd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e3dd-125">Content-Type</span></span>  |<span data-ttu-id="8e3dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e3dd-126">application/json</span></span>         |
|<span data-ttu-id="8e3dd-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="8e3dd-127">If-Match</span></span>      |<span data-ttu-id="8e3dd-128">必需。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-128">Required.</span></span> <span data-ttu-id="8e3dd-129">如果包含此请求标头, 且提供的 eTag 与**companyInformation**上的当前标记不匹配, 则不会更新**companyInformation** 。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-129">When this request header is included and the eTag provided does not match the current tag on the **companyInformation**, the **companyInformation** will not be updated.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e3dd-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e3dd-130">Request body</span></span>
<span data-ttu-id="8e3dd-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="8e3dd-134">响应</span><span class="sxs-lookup"><span data-stu-id="8e3dd-134">Response</span></span>
<span data-ttu-id="8e3dd-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的**companyInformation**对象。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-135">If successful, this method returns a `200 OK` response code and an updated an **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e3dd-136">示例</span><span class="sxs-lookup"><span data-stu-id="8e3dd-136">Example</span></span>

<span data-ttu-id="8e3dd-137">**请求**</span><span class="sxs-lookup"><span data-stu-id="8e3dd-137">**Request**</span></span>

<span data-ttu-id="8e3dd-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/companyInformation('{id}')
Content-type: application/json

{
  "displayName": "CRONUS USA, LTD.",
  "website": "www.cronuscorp.net"
}
```

<span data-ttu-id="8e3dd-139">**响应**</span><span class="sxs-lookup"><span data-stu-id="8e3dd-139">**Response**</span></span>

<span data-ttu-id="8e3dd-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="8e3dd-141">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e3dd-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e3dd-142">All the properties will be returned from an actual call.</span></span>

```json
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
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/companyInformation('{id}')/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
  }
```
