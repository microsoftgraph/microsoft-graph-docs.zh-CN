---
title: 获取 customerPaymentJournals
description: 获取 Dynamics 365 Business Central 中的客户付款日志。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 63844cd7b18201c47a2ed27480fe9db2bc5bc107
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430544"
---
# <a name="get-customerpaymentjournals"></a><span data-ttu-id="d202c-103">获取 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="d202c-103">Get customerPaymentJournals</span></span>

<span data-ttu-id="d202c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d202c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d202c-105">检索 Dynamics 365 Business Central 的客户付款日记对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d202c-105">Retrieve the properties and relationships of a customer payment journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d202c-106">权限</span><span class="sxs-lookup"><span data-stu-id="d202c-106">Permissions</span></span>
<span data-ttu-id="d202c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d202c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d202c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d202c-109">Permission type</span></span> |<span data-ttu-id="d202c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d202c-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d202c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d202c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d202c-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d202c-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d202c-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="d202c-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d202c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d202c-114">Not supported.</span></span>|
|<span data-ttu-id="d202c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d202c-115">Application</span></span>|<span data-ttu-id="d202c-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d202c-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d202c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d202c-117">HTTP request</span></span>

```
GET /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d202c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d202c-118">Optional query parameters</span></span>
<span data-ttu-id="d202c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d202c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d202c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d202c-120">Request headers</span></span>
|<span data-ttu-id="d202c-121">标头</span><span class="sxs-lookup"><span data-stu-id="d202c-121">Header</span></span>       |<span data-ttu-id="d202c-122">值</span><span class="sxs-lookup"><span data-stu-id="d202c-122">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="d202c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d202c-123">Authorization</span></span>|<span data-ttu-id="d202c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d202c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d202c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d202c-126">Request body</span></span>
<span data-ttu-id="d202c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d202c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d202c-128">响应</span><span class="sxs-lookup"><span data-stu-id="d202c-128">Response</span></span>
<span data-ttu-id="d202c-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和**customerPaymentJournals**对象。</span><span class="sxs-lookup"><span data-stu-id="d202c-129">If successful, this method returns a `200 OK` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d202c-130">示例</span><span class="sxs-lookup"><span data-stu-id="d202c-130">Example</span></span>

<span data-ttu-id="d202c-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="d202c-131">**Request**</span></span>

<span data-ttu-id="d202c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d202c-132">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}
```

<span data-ttu-id="d202c-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="d202c-133">**Response**</span></span>

<span data-ttu-id="d202c-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d202c-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="d202c-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d202c-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d202c-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d202c-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```
