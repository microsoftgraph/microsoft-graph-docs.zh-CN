---
title: 获取 generalLedgerEntries
description: 获取 Dynamics 365 Business Central 中的总帐条目对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4aa22cf2a0634d9c54d6c9e12573730714be3ca4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981308"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="d92f9-103">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="d92f9-103">Get generalLedgerEntries</span></span>

<span data-ttu-id="d92f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d92f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d92f9-105">检索 Dynamics 365 Business Central 的总帐条目对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d92f9-105">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d92f9-106">权限</span><span class="sxs-lookup"><span data-stu-id="d92f9-106">Permissions</span></span>
<span data-ttu-id="d92f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d92f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d92f9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d92f9-109">Permission type</span></span> |<span data-ttu-id="d92f9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d92f9-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d92f9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d92f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d92f9-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d92f9-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d92f9-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="d92f9-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d92f9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d92f9-114">Not supported.</span></span>|
|<span data-ttu-id="d92f9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d92f9-115">Application</span></span>|<span data-ttu-id="d92f9-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d92f9-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="d92f9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d92f9-117">HTTP request</span></span>
```
GET /financials/companies/{id}/generalLedgerEntries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d92f9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d92f9-118">Optional query parameters</span></span>
<span data-ttu-id="d92f9-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d92f9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d92f9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d92f9-120">Request headers</span></span>
|<span data-ttu-id="d92f9-121">标头</span><span class="sxs-lookup"><span data-stu-id="d92f9-121">Header</span></span>       |<span data-ttu-id="d92f9-122">值</span><span class="sxs-lookup"><span data-stu-id="d92f9-122">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="d92f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d92f9-123">Authorization</span></span>|<span data-ttu-id="d92f9-124">负载.</span><span class="sxs-lookup"><span data-stu-id="d92f9-124">Bearer.</span></span> <span data-ttu-id="d92f9-125">必需。</span><span class="sxs-lookup"><span data-stu-id="d92f9-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d92f9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d92f9-126">Request body</span></span>
<span data-ttu-id="d92f9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d92f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d92f9-128">响应</span><span class="sxs-lookup"><span data-stu-id="d92f9-128">Response</span></span>
<span data-ttu-id="d92f9-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **generalLedgerEntries** 对象。</span><span class="sxs-lookup"><span data-stu-id="d92f9-129">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d92f9-130">示例</span><span class="sxs-lookup"><span data-stu-id="d92f9-130">Example</span></span>

<span data-ttu-id="d92f9-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="d92f9-131">**Request**</span></span>

<span data-ttu-id="d92f9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d92f9-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/generalLedgerEntries/{id}
```

<span data-ttu-id="d92f9-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="d92f9-133">**Response**</span></span>

<span data-ttu-id="d92f9-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d92f9-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="d92f9-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d92f9-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d92f9-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d92f9-136">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "10700",
    "postingDate": "2017-03-15",
    "documentNumber": "108027",
    "documentType": "Invoice",
    "accountId": "id-value",
    "accountNumber": "7210",
    "description": "Order 106003",
    "debitAmount": 6943.8,
    "creditAmount": 0,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```



