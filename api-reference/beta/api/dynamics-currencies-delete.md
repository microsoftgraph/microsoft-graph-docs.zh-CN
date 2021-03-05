---
title: 删除货币
description: 删除 Dynamics 365 Business Central 中的货币对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b9f6c729dc97d523952454978afc056c05c354c5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473152"
---
# <a name="delete-currencies"></a><span data-ttu-id="d79f9-103">删除货币</span><span class="sxs-lookup"><span data-stu-id="d79f9-103">Delete currencies</span></span>

<span data-ttu-id="d79f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d79f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d79f9-105">从 Dynamics 365 Business Central 中删除货币对象。</span><span class="sxs-lookup"><span data-stu-id="d79f9-105">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d79f9-106">权限</span><span class="sxs-lookup"><span data-stu-id="d79f9-106">Permissions</span></span>
<span data-ttu-id="d79f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d79f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d79f9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d79f9-109">Permission type</span></span> |<span data-ttu-id="d79f9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d79f9-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d79f9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d79f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d79f9-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79f9-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d79f9-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="d79f9-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d79f9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d79f9-114">Not supported.</span></span>|
|<span data-ttu-id="d79f9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d79f9-115">Application</span></span>|<span data-ttu-id="d79f9-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79f9-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d79f9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d79f9-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d79f9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d79f9-118">Optional query parameters</span></span>
<span data-ttu-id="d79f9-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d79f9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d79f9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d79f9-120">Request headers</span></span>

|<span data-ttu-id="d79f9-121">标头</span><span class="sxs-lookup"><span data-stu-id="d79f9-121">Header</span></span>|<span data-ttu-id="d79f9-122">值</span><span class="sxs-lookup"><span data-stu-id="d79f9-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="d79f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d79f9-123">Authorization</span></span>  |<span data-ttu-id="d79f9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d79f9-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d79f9-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="d79f9-126">If-Match</span></span>       |<span data-ttu-id="d79f9-127">必填。</span><span class="sxs-lookup"><span data-stu-id="d79f9-127">Required.</span></span> <span data-ttu-id="d79f9-128">如果包含此请求标头且提供的 eTag 与货币上的当前标记不匹配，**则货币** 不会</span><span class="sxs-lookup"><span data-stu-id="d79f9-128">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="d79f9-129">更新。</span><span class="sxs-lookup"><span data-stu-id="d79f9-129">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d79f9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d79f9-130">Request body</span></span>
<span data-ttu-id="d79f9-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d79f9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d79f9-132">响应</span><span class="sxs-lookup"><span data-stu-id="d79f9-132">Response</span></span>
<span data-ttu-id="d79f9-p104">如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d79f9-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d79f9-135">示例</span><span class="sxs-lookup"><span data-stu-id="d79f9-135">Example</span></span>

<span data-ttu-id="d79f9-136">**请求**</span><span class="sxs-lookup"><span data-stu-id="d79f9-136">**Request**</span></span>

<span data-ttu-id="d79f9-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d79f9-137">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="d79f9-138">**响应**</span><span class="sxs-lookup"><span data-stu-id="d79f9-138">**Response**</span></span> 

<span data-ttu-id="d79f9-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d79f9-139">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```


