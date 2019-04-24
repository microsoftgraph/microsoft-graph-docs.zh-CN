---
title: 创建供应商
description: 在 Dynamics 365 Business Central 中创建一个供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 90c2c8a25602ac2a2c4197c916b9ce14e03b8e6d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458612"
---
# <a name="create-vendors"></a><span data-ttu-id="3330d-103">创建供应商</span><span class="sxs-lookup"><span data-stu-id="3330d-103">Create vendors</span></span>
<span data-ttu-id="3330d-104">在 Dynamics 365 Business Central 中创建一个供应商对象。</span><span class="sxs-lookup"><span data-stu-id="3330d-104">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3330d-105">权限</span><span class="sxs-lookup"><span data-stu-id="3330d-105">Permissions</span></span>
<span data-ttu-id="3330d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3330d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3330d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3330d-108">Permission type</span></span> |<span data-ttu-id="3330d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3330d-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3330d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3330d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3330d-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3330d-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3330d-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="3330d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3330d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3330d-113">Not supported.</span></span>|
|<span data-ttu-id="3330d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3330d-114">Application</span></span>|<span data-ttu-id="3330d-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3330d-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3330d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3330d-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3330d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3330d-117">Optional query parameters</span></span>
<span data-ttu-id="3330d-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3330d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3330d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3330d-119">Request headers</span></span>
|<span data-ttu-id="3330d-120">标头</span><span class="sxs-lookup"><span data-stu-id="3330d-120">Header</span></span>|<span data-ttu-id="3330d-121">值</span><span class="sxs-lookup"><span data-stu-id="3330d-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="3330d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3330d-122">Authorization</span></span>  |<span data-ttu-id="3330d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3330d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="3330d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3330d-125">Content-Type</span></span>  |<span data-ttu-id="3330d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3330d-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="3330d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3330d-127">Request body</span></span>
<span data-ttu-id="3330d-128">在请求正文中, 提供 "**供应商**" 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3330d-128">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="3330d-129">响应</span><span class="sxs-lookup"><span data-stu-id="3330d-129">Response</span></span>
<span data-ttu-id="3330d-130">如果成功, 此方法在```201 Created```响应正文中返回响应代码和**供应商**对象。</span><span class="sxs-lookup"><span data-stu-id="3330d-130">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3330d-131">示例</span><span class="sxs-lookup"><span data-stu-id="3330d-131">Example</span></span>

<span data-ttu-id="3330d-132">**请求**</span><span class="sxs-lookup"><span data-stu-id="3330d-132">**Request**</span></span>

<span data-ttu-id="3330d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3330d-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/vendors
Content-type: application/json

{
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": " "
}
```

<span data-ttu-id="3330d-134">**响应**</span><span class="sxs-lookup"><span data-stu-id="3330d-134">**Response**</span></span>

<span data-ttu-id="3330d-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3330d-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="3330d-136">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3330d-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3330d-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3330d-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}

```

