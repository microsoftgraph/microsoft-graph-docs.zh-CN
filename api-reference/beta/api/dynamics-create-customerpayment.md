---
title: 创建 customerPayments
description: 在 Dynamics 365 Business Central 中创建客户付款对象。
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: da711f4e7ce186814d5e5c33870ed908a853a5c6
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792070"
---
# <a name="create-customerpayments"></a><span data-ttu-id="31a3d-103">创建 customerPayments</span><span class="sxs-lookup"><span data-stu-id="31a3d-103">Create customerPayments</span></span>
<span data-ttu-id="31a3d-104">在 Dynamics 365 Business Central 中创建客户付款对象。</span><span class="sxs-lookup"><span data-stu-id="31a3d-104">Creates a customer payment object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="31a3d-105">权限</span><span class="sxs-lookup"><span data-stu-id="31a3d-105">Permissions</span></span>
<span data-ttu-id="31a3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31a3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31a3d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="31a3d-108">Permission type</span></span> |<span data-ttu-id="31a3d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31a3d-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="31a3d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31a3d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="31a3d-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31a3d-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="31a3d-112">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="31a3d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="31a3d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="31a3d-113">Not supported.</span></span>|
|<span data-ttu-id="31a3d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="31a3d-114">Application</span></span>|<span data-ttu-id="31a3d-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31a3d-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31a3d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31a3d-116">HTTP request</span></span>
```
POST /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31a3d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31a3d-117">Optional query parameters</span></span>
<span data-ttu-id="31a3d-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31a3d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31a3d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="31a3d-119">Request headers</span></span>
|<span data-ttu-id="31a3d-120">标头</span><span class="sxs-lookup"><span data-stu-id="31a3d-120">Header</span></span>        |<span data-ttu-id="31a3d-121">值</span><span class="sxs-lookup"><span data-stu-id="31a3d-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="31a3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31a3d-122">Authorization</span></span> |<span data-ttu-id="31a3d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31a3d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="31a3d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31a3d-125">Content-Type</span></span>  |<span data-ttu-id="31a3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31a3d-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="31a3d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31a3d-127">Request body</span></span>
<span data-ttu-id="31a3d-128">在请求正文中，提供**customerPayments**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31a3d-128">In the request body, supply a JSON representation of **customerPayments** object.</span></span>

## <a name="response"></a><span data-ttu-id="31a3d-129">响应</span><span class="sxs-lookup"><span data-stu-id="31a3d-129">Response</span></span>
<span data-ttu-id="31a3d-130">如果成功，此方法在```201 Created```响应正文中返回响应代码和**customerPayments**对象。</span><span class="sxs-lookup"><span data-stu-id="31a3d-130">If successful, this method returns ```201 Created``` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31a3d-131">示例</span><span class="sxs-lookup"><span data-stu-id="31a3d-131">Example</span></span>

<span data-ttu-id="31a3d-132">**请求**</span><span class="sxs-lookup"><span data-stu-id="31a3d-132">**Request**</span></span>

<span data-ttu-id="31a3d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31a3d-133">Here is an example of a request.</span></span>

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
<span data-ttu-id="31a3d-134">**响应**</span><span class="sxs-lookup"><span data-stu-id="31a3d-134">**Response**</span></span>

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

