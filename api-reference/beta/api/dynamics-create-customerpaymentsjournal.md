---
title: 创建 customerPaymentJournals
description: 在 Dynamics 365 Business Central 中创建客户付款日记对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3f1bcae115bd1d5e9c117b6bc90981402397ab0e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956693"
---
# <a name="create-customerpaymentjournals"></a><span data-ttu-id="10f74-103">创建 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="10f74-103">Create customerPaymentJournals</span></span>
<span data-ttu-id="10f74-104">在 Dynamics 365 Business Central 中创建客户付款日记对象。</span><span class="sxs-lookup"><span data-stu-id="10f74-104">Creates a customer payment journal object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="10f74-105">权限</span><span class="sxs-lookup"><span data-stu-id="10f74-105">Permissions</span></span>
<span data-ttu-id="10f74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f74-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="10f74-108">Permission type</span></span> |<span data-ttu-id="10f74-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10f74-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="10f74-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10f74-110">Delegated (work or school account)</span></span>|<span data-ttu-id="10f74-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f74-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="10f74-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="10f74-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="10f74-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="10f74-113">Not supported.</span></span>|
|<span data-ttu-id="10f74-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="10f74-114">Application</span></span>|<span data-ttu-id="10f74-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f74-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10f74-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10f74-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10f74-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10f74-117">Optional query parameters</span></span>
<span data-ttu-id="10f74-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10f74-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10f74-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="10f74-119">Request headers</span></span>
|<span data-ttu-id="10f74-120">标头</span><span class="sxs-lookup"><span data-stu-id="10f74-120">Header</span></span>        |<span data-ttu-id="10f74-121">值</span><span class="sxs-lookup"><span data-stu-id="10f74-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="10f74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10f74-122">Authorization</span></span> |<span data-ttu-id="10f74-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10f74-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="10f74-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10f74-125">Content-Type</span></span>  |<span data-ttu-id="10f74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10f74-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="10f74-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10f74-127">Request body</span></span>
<span data-ttu-id="10f74-128">在请求正文中, 提供**customerPaymentJournals**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10f74-128">In the request body, supply a JSON representation of **customerPaymentJournals** object.</span></span>

## <a name="response"></a><span data-ttu-id="10f74-129">响应</span><span class="sxs-lookup"><span data-stu-id="10f74-129">Response</span></span>
<span data-ttu-id="10f74-130">如果成功, 此方法在```201 Created```响应正文中返回响应代码和**customerPaymentJournals**对象。</span><span class="sxs-lookup"><span data-stu-id="10f74-130">If successful, this method returns ```201 Created``` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f74-131">示例</span><span class="sxs-lookup"><span data-stu-id="10f74-131">Example</span></span>

<span data-ttu-id="10f74-132">**请求**</span><span class="sxs-lookup"><span data-stu-id="10f74-132">**Request**</span></span>

<span data-ttu-id="10f74-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10f74-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="10f74-134">**响应**</span><span class="sxs-lookup"><span data-stu-id="10f74-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


