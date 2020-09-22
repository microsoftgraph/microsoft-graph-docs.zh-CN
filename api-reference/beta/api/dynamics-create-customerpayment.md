---
title: 创建 customerPayments
description: 在 Dynamics 365 Business Central 中创建客户付款对象。
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c5005a3fb97b44a173042d76088fb6fee0947a1f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008349"
---
# <a name="create-customerpayments"></a><span data-ttu-id="ece38-103">创建 customerPayments</span><span class="sxs-lookup"><span data-stu-id="ece38-103">Create customerPayments</span></span>

<span data-ttu-id="ece38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ece38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ece38-105">在 Dynamics 365 Business Central 中创建客户付款对象。</span><span class="sxs-lookup"><span data-stu-id="ece38-105">Creates a customer payment object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ece38-106">权限</span><span class="sxs-lookup"><span data-stu-id="ece38-106">Permissions</span></span>
<span data-ttu-id="ece38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ece38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ece38-109">Permission type</span></span> |<span data-ttu-id="ece38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ece38-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ece38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ece38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ece38-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece38-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ece38-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ece38-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ece38-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ece38-114">Not supported.</span></span>|
|<span data-ttu-id="ece38-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ece38-115">Application</span></span>|<span data-ttu-id="ece38-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece38-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ece38-117">HTTP request</span></span>
```
POST /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ece38-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ece38-118">Optional query parameters</span></span>
<span data-ttu-id="ece38-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ece38-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ece38-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ece38-120">Request headers</span></span>
|<span data-ttu-id="ece38-121">标头</span><span class="sxs-lookup"><span data-stu-id="ece38-121">Header</span></span>        |<span data-ttu-id="ece38-122">值</span><span class="sxs-lookup"><span data-stu-id="ece38-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="ece38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ece38-123">Authorization</span></span> |<span data-ttu-id="ece38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ece38-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ece38-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ece38-126">Content-Type</span></span>  |<span data-ttu-id="ece38-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ece38-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="ece38-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ece38-128">Request body</span></span>
<span data-ttu-id="ece38-129">在请求正文中，提供 **customerPayments** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ece38-129">In the request body, supply a JSON representation of **customerPayments** object.</span></span>

## <a name="response"></a><span data-ttu-id="ece38-130">响应</span><span class="sxs-lookup"><span data-stu-id="ece38-130">Response</span></span>
<span data-ttu-id="ece38-131">如果成功，此方法 ```201 Created``` 在响应正文中返回响应代码和 **customerPayments** 对象。</span><span class="sxs-lookup"><span data-stu-id="ece38-131">If successful, this method returns ```201 Created``` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece38-132">示例</span><span class="sxs-lookup"><span data-stu-id="ece38-132">Example</span></span>

<span data-ttu-id="ece38-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="ece38-133">**Request**</span></span>

<span data-ttu-id="ece38-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ece38-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournal/{id}/customerPayments
Content-type: application/json

{
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "contactId": "contactId-value",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": -1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
}
```
<span data-ttu-id="ece38-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="ece38-135">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```



