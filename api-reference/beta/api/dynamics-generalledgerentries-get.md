---
title: 获取 generalLedgerEntries
description: 获取 Dynamics 365 Business Central 中的总帐条目对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b75a8d70b2692fb5add39e12e388aa364e8ea585
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791622"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="5ceb8-103">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="5ceb8-103">Get generalLedgerEntries</span></span>
<span data-ttu-id="5ceb8-104">检索 Dynamics 365 Business Central 的总帐条目对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-104">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ceb8-105">权限</span><span class="sxs-lookup"><span data-stu-id="5ceb8-105">Permissions</span></span>
<span data-ttu-id="5ceb8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ceb8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ceb8-108">Permission type</span></span> |<span data-ttu-id="5ceb8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ceb8-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5ceb8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ceb8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5ceb8-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ceb8-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5ceb8-112">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5ceb8-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5ceb8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-113">Not supported.</span></span>|
|<span data-ttu-id="5ceb8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ceb8-114">Application</span></span>|<span data-ttu-id="5ceb8-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ceb8-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="5ceb8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ceb8-116">HTTP request</span></span>
```
GET /financials/companies/{id}/generalLedgerEntries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ceb8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5ceb8-117">Optional query parameters</span></span>
<span data-ttu-id="5ceb8-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ceb8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ceb8-119">Request headers</span></span>
|<span data-ttu-id="5ceb8-120">标头</span><span class="sxs-lookup"><span data-stu-id="5ceb8-120">Header</span></span>       |<span data-ttu-id="5ceb8-121">值</span><span class="sxs-lookup"><span data-stu-id="5ceb8-121">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="5ceb8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ceb8-122">Authorization</span></span>|<span data-ttu-id="5ceb8-123">负载.</span><span class="sxs-lookup"><span data-stu-id="5ceb8-123">Bearer.</span></span> <span data-ttu-id="5ceb8-124">必需。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ceb8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ceb8-125">Request body</span></span>
<span data-ttu-id="5ceb8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ceb8-127">响应</span><span class="sxs-lookup"><span data-stu-id="5ceb8-127">Response</span></span>
<span data-ttu-id="5ceb8-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和**generalLedgerEntries**对象。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-128">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ceb8-129">示例</span><span class="sxs-lookup"><span data-stu-id="5ceb8-129">Example</span></span>

<span data-ttu-id="5ceb8-130">**请求**</span><span class="sxs-lookup"><span data-stu-id="5ceb8-130">**Request**</span></span>

<span data-ttu-id="5ceb8-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/generalLedgerEntries/{id}
```

<span data-ttu-id="5ceb8-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="5ceb8-132">**Response**</span></span>

<span data-ttu-id="5ceb8-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="5ceb8-134">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5ceb8-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5ceb8-135">All the properties will be returned from an actual call.</span></span>

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

