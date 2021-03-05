---
title: 获取 generalLedgerEntries
description: 获取 Dynamics 365 Business Central 中的总帐条目对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: d3862417cd75e2a6adb55c1c9660b8b1c2ddabc4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473005"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="e9e39-103">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="e9e39-103">Get generalLedgerEntries</span></span>

<span data-ttu-id="e9e39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e39-105">检索 Dynamics 365 Business Central 的一般分类帐条目对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e9e39-105">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9e39-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9e39-106">Permissions</span></span>
<span data-ttu-id="e9e39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9e39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9e39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9e39-109">Permission type</span></span> |<span data-ttu-id="e9e39-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9e39-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e9e39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9e39-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9e39-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9e39-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e9e39-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e9e39-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e9e39-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9e39-114">Not supported.</span></span>|
|<span data-ttu-id="e9e39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9e39-115">Application</span></span>|<span data-ttu-id="e9e39-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9e39-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="e9e39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9e39-117">HTTP request</span></span>
```
GET /financials/companies/{id}/generalLedgerEntries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9e39-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e9e39-118">Optional query parameters</span></span>
<span data-ttu-id="e9e39-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e9e39-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9e39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9e39-120">Request headers</span></span>
|<span data-ttu-id="e9e39-121">标头</span><span class="sxs-lookup"><span data-stu-id="e9e39-121">Header</span></span>       |<span data-ttu-id="e9e39-122">值</span><span class="sxs-lookup"><span data-stu-id="e9e39-122">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="e9e39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9e39-123">Authorization</span></span>|<span data-ttu-id="e9e39-124">Bearer。</span><span class="sxs-lookup"><span data-stu-id="e9e39-124">Bearer.</span></span> <span data-ttu-id="e9e39-125">必填。</span><span class="sxs-lookup"><span data-stu-id="e9e39-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9e39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9e39-126">Request body</span></span>
<span data-ttu-id="e9e39-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9e39-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9e39-128">响应</span><span class="sxs-lookup"><span data-stu-id="e9e39-128">Response</span></span>
<span data-ttu-id="e9e39-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` **generalLedgerEntries** 对象。</span><span class="sxs-lookup"><span data-stu-id="e9e39-129">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9e39-130">示例</span><span class="sxs-lookup"><span data-stu-id="e9e39-130">Example</span></span>

<span data-ttu-id="e9e39-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="e9e39-131">**Request**</span></span>

<span data-ttu-id="e9e39-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9e39-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/generalLedgerEntries/{id}
```

<span data-ttu-id="e9e39-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="e9e39-133">**Response**</span></span>

<span data-ttu-id="e9e39-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e9e39-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="e9e39-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9e39-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e9e39-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e9e39-136">All the properties will be returned from an actual call.</span></span>

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



