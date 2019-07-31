---
title: 获取 trialBalance
description: 获取 Dynamics 365 Business Central 中的试算平衡表对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b3e5881964d49fa1a42cf1aa4f9da8fba818d6e5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955867"
---
# <a name="get-trialbalance"></a><span data-ttu-id="ac9b5-103">获取 trialBalance</span><span class="sxs-lookup"><span data-stu-id="ac9b5-103">Get trialBalance</span></span>
<span data-ttu-id="ac9b5-104">检索 Dynamics 365 Business Central 的试用余额报告对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-104">Retrieve the properties and relationships of a trial balance report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac9b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="ac9b5-105">Permissions</span></span>
<span data-ttu-id="ac9b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac9b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac9b5-108">Permission type</span></span> |<span data-ttu-id="ac9b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac9b5-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ac9b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac9b5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ac9b5-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac9b5-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ac9b5-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ac9b5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ac9b5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-113">Not supported.</span></span>|
|<span data-ttu-id="ac9b5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac9b5-114">Application</span></span>|<span data-ttu-id="ac9b5-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac9b5-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac9b5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac9b5-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/trialBalance
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac9b5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ac9b5-117">Optional query parameters</span></span>
<span data-ttu-id="ac9b5-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac9b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac9b5-119">Request headers</span></span>
|<span data-ttu-id="ac9b5-120">标头</span><span class="sxs-lookup"><span data-stu-id="ac9b5-120">Header</span></span>|<span data-ttu-id="ac9b5-121">值</span><span class="sxs-lookup"><span data-stu-id="ac9b5-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="ac9b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac9b5-122">Authorization</span></span>  |<span data-ttu-id="ac9b5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac9b5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac9b5-125">Request body</span></span>
<span data-ttu-id="ac9b5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac9b5-127">响应</span><span class="sxs-lookup"><span data-stu-id="ac9b5-127">Response</span></span>
<span data-ttu-id="ac9b5-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**trialBalance**对象。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-128">If successful, this method returns a `200 OK` response code and a **trialBalance** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac9b5-129">示例</span><span class="sxs-lookup"><span data-stu-id="ac9b5-129">Example</span></span>

<span data-ttu-id="ac9b5-130">**请求**</span><span class="sxs-lookup"><span data-stu-id="ac9b5-130">**Request**</span></span>

<span data-ttu-id="ac9b5-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/trialBalance?$orderby number&$filter=dateFilter ge 2019-01-01 and dateFilter le 2019-12-31
```

<span data-ttu-id="ac9b5-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="ac9b5-132">**Response**</span></span>

<span data-ttu-id="ac9b5-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="ac9b5-134">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ac9b5-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ac9b5-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "number": "1110",
  "accountId": "id-value",
  "accountType": "Posting",
  "display": "Accounts Receivable",
  "totalDebit": "479.00",
  "totalCredit": "0.00",
  "balanceAtDateDebit": "72,893.84",
  "balanceAtDateCredit": "0.00",
  "dateFilter": "2019-12-31"    
}
```

