---
title: 创建供应商
description: 在 Dynamics 365 Business Central 中创建一个供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2bf393a954078585cc89a073947c636a233a2a00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431083"
---
# <a name="create-vendors"></a><span data-ttu-id="83038-103">创建供应商</span><span class="sxs-lookup"><span data-stu-id="83038-103">Create vendors</span></span>

<span data-ttu-id="83038-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="83038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83038-105">在 Dynamics 365 Business Central 中创建一个供应商对象。</span><span class="sxs-lookup"><span data-stu-id="83038-105">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="83038-106">权限</span><span class="sxs-lookup"><span data-stu-id="83038-106">Permissions</span></span>
<span data-ttu-id="83038-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83038-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83038-109">Permission type</span></span> |<span data-ttu-id="83038-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83038-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="83038-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83038-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83038-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83038-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="83038-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="83038-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="83038-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83038-114">Not supported.</span></span>|
|<span data-ttu-id="83038-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83038-115">Application</span></span>|<span data-ttu-id="83038-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83038-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83038-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83038-117">HTTP request</span></span>
```
POST /financials/companies/{id}/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83038-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="83038-118">Optional query parameters</span></span>
<span data-ttu-id="83038-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="83038-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83038-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83038-120">Request headers</span></span>
|<span data-ttu-id="83038-121">标头</span><span class="sxs-lookup"><span data-stu-id="83038-121">Header</span></span>|<span data-ttu-id="83038-122">值</span><span class="sxs-lookup"><span data-stu-id="83038-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="83038-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83038-123">Authorization</span></span>  |<span data-ttu-id="83038-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83038-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="83038-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83038-126">Content-Type</span></span>  |<span data-ttu-id="83038-127">application/json</span><span class="sxs-lookup"><span data-stu-id="83038-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="83038-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="83038-128">Request body</span></span>
<span data-ttu-id="83038-129">在请求正文中，提供 "**供应商**" 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83038-129">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="83038-130">响应</span><span class="sxs-lookup"><span data-stu-id="83038-130">Response</span></span>
<span data-ttu-id="83038-131">如果成功，此方法在```201 Created```响应正文中返回响应代码和**供应商**对象。</span><span class="sxs-lookup"><span data-stu-id="83038-131">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83038-132">示例</span><span class="sxs-lookup"><span data-stu-id="83038-132">Example</span></span>

<span data-ttu-id="83038-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="83038-133">**Request**</span></span>

<span data-ttu-id="83038-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83038-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/vendors
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

<span data-ttu-id="83038-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="83038-135">**Response**</span></span>

<span data-ttu-id="83038-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="83038-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="83038-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="83038-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="83038-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="83038-138">All the properties will be returned from an actual call.</span></span>

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

