---
title: 获取 generalLedgerEntries
description: 获取 Dynamics 365 Business Central 中的总帐条目对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 08246b246bda49700e4efd7d84073a3ea1113c5c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045381"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="99447-103">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="99447-103">Get generalLedgerEntries</span></span>

<span data-ttu-id="99447-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99447-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99447-105">检索 Dynamics 365 Business Central 总帐条目对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99447-105">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="99447-106">权限</span><span class="sxs-lookup"><span data-stu-id="99447-106">Permissions</span></span>
<span data-ttu-id="99447-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99447-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99447-109">Permission type</span></span> |<span data-ttu-id="99447-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99447-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="99447-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99447-111">Delegated (work or school account)</span></span>|<span data-ttu-id="99447-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99447-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="99447-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="99447-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="99447-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99447-114">Not supported.</span></span>|
|<span data-ttu-id="99447-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99447-115">Application</span></span>|<span data-ttu-id="99447-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99447-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="99447-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99447-117">HTTP request</span></span>
```
GET /financials/companies/{id}/generalLedgerEntries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99447-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="99447-118">Optional query parameters</span></span>
<span data-ttu-id="99447-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="99447-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99447-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99447-120">Request headers</span></span>
|<span data-ttu-id="99447-121">标头</span><span class="sxs-lookup"><span data-stu-id="99447-121">Header</span></span>       |<span data-ttu-id="99447-122">值</span><span class="sxs-lookup"><span data-stu-id="99447-122">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="99447-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99447-123">Authorization</span></span>|<span data-ttu-id="99447-124">Bearer。</span><span class="sxs-lookup"><span data-stu-id="99447-124">Bearer.</span></span> <span data-ttu-id="99447-125">必需。</span><span class="sxs-lookup"><span data-stu-id="99447-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99447-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99447-126">Request body</span></span>
<span data-ttu-id="99447-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99447-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99447-128">响应</span><span class="sxs-lookup"><span data-stu-id="99447-128">Response</span></span>
<span data-ttu-id="99447-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **generalLedgerEntries** 对象。</span><span class="sxs-lookup"><span data-stu-id="99447-129">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99447-130">示例</span><span class="sxs-lookup"><span data-stu-id="99447-130">Example</span></span>

<span data-ttu-id="99447-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="99447-131">**Request**</span></span>

<span data-ttu-id="99447-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99447-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/generalLedgerEntries/{id}
```

<span data-ttu-id="99447-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="99447-133">**Response**</span></span>

<span data-ttu-id="99447-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99447-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="99447-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="99447-135">**Note**: The response object shown here might be shortened for readability.</span></span>

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



