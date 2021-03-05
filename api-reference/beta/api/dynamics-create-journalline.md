---
title: 创建 journalLines
description: 在 Dynamics 365 Business Central 中创建日记行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 38feb577f11f482fe00c5d44d883e1b0995ff562
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473264"
---
# <a name="create-journallines"></a><span data-ttu-id="accd6-103">创建 journalLines</span><span class="sxs-lookup"><span data-stu-id="accd6-103">Create journalLines</span></span>

<span data-ttu-id="accd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="accd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="accd6-105">在 Dynamics 365 Business Central 中创建日记行对象。</span><span class="sxs-lookup"><span data-stu-id="accd6-105">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="accd6-106">权限</span><span class="sxs-lookup"><span data-stu-id="accd6-106">Permissions</span></span>
<span data-ttu-id="accd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="accd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="accd6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="accd6-109">Permission type</span></span> |<span data-ttu-id="accd6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="accd6-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="accd6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="accd6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="accd6-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="accd6-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="accd6-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="accd6-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="accd6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="accd6-114">Not supported.</span></span>|
|<span data-ttu-id="accd6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="accd6-115">Application</span></span>|<span data-ttu-id="accd6-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="accd6-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="accd6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="accd6-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="accd6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="accd6-118">Optional query parameters</span></span>
<span data-ttu-id="accd6-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="accd6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="accd6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="accd6-120">Request headers</span></span>
|<span data-ttu-id="accd6-121">标头</span><span class="sxs-lookup"><span data-stu-id="accd6-121">Header</span></span>        |<span data-ttu-id="accd6-122">值</span><span class="sxs-lookup"><span data-stu-id="accd6-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="accd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="accd6-123">Authorization</span></span> |<span data-ttu-id="accd6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="accd6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="accd6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="accd6-126">Content-Type</span></span>  |<span data-ttu-id="accd6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="accd6-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="accd6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="accd6-128">Request body</span></span>
<span data-ttu-id="accd6-129">在请求正文中，提供 **journalLines** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="accd6-129">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="accd6-130">响应</span><span class="sxs-lookup"><span data-stu-id="accd6-130">Response</span></span>
<span data-ttu-id="accd6-131">如果成功，此方法在响应正文中返回响应代码 ```201 Created``` 和 **journalLines** 对象。</span><span class="sxs-lookup"><span data-stu-id="accd6-131">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="accd6-132">示例</span><span class="sxs-lookup"><span data-stu-id="accd6-132">Example</span></span>

<span data-ttu-id="accd6-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="accd6-133">**Request**</span></span>

<span data-ttu-id="accd6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="accd6-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines
Content-type: application/json

{
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": ""
}
```
<span data-ttu-id="accd6-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="accd6-135">**Response**</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```




