---
title: 删除供应商
description: 删除 Dynamics 365 Business Central 中的供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8de331472d60c64ac753243f3bbcba18d23b3a24
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474097"
---
# <a name="delete-vendors"></a><span data-ttu-id="5a90f-103">删除供应商</span><span class="sxs-lookup"><span data-stu-id="5a90f-103">Delete vendors</span></span>

<span data-ttu-id="5a90f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a90f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a90f-105">从 Dynamics 365 Business Central 中删除供应商对象。</span><span class="sxs-lookup"><span data-stu-id="5a90f-105">Delete a vendor object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a90f-106">权限</span><span class="sxs-lookup"><span data-stu-id="5a90f-106">Permissions</span></span>
<span data-ttu-id="5a90f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a90f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a90f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a90f-109">Permission type</span></span> |<span data-ttu-id="5a90f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a90f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5a90f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a90f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a90f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a90f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5a90f-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5a90f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5a90f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a90f-114">Not supported.</span></span>|
|<span data-ttu-id="5a90f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a90f-115">Application</span></span>|<span data-ttu-id="5a90f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a90f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a90f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a90f-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a90f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a90f-118">Optional query parameters</span></span>
<span data-ttu-id="5a90f-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5a90f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a90f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a90f-120">Request headers</span></span>
|<span data-ttu-id="5a90f-121">标头</span><span class="sxs-lookup"><span data-stu-id="5a90f-121">Header</span></span>|<span data-ttu-id="5a90f-122">值</span><span class="sxs-lookup"><span data-stu-id="5a90f-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="5a90f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a90f-123">Authorization</span></span>  |<span data-ttu-id="5a90f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a90f-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="5a90f-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="5a90f-126">If-Match</span></span>       |<span data-ttu-id="5a90f-127">必填。</span><span class="sxs-lookup"><span data-stu-id="5a90f-127">Required.</span></span> <span data-ttu-id="5a90f-128">如果包含此请求标头且提供的 eTag 与供应商上的当前标记不匹配，则将不会更新供应商。</span><span class="sxs-lookup"><span data-stu-id="5a90f-128">When this request header is included and the eTag provided does not match the current tag on the **vendors**, the **vendors** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a90f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a90f-129">Request body</span></span>
<span data-ttu-id="5a90f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a90f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a90f-131">响应</span><span class="sxs-lookup"><span data-stu-id="5a90f-131">Response</span></span>
<span data-ttu-id="5a90f-p104">如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5a90f-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a90f-134">示例</span><span class="sxs-lookup"><span data-stu-id="5a90f-134">Example</span></span>

<span data-ttu-id="5a90f-135">**请求**</span><span class="sxs-lookup"><span data-stu-id="5a90f-135">**Request**</span></span>

<span data-ttu-id="5a90f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a90f-136">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="5a90f-137">**响应**</span><span class="sxs-lookup"><span data-stu-id="5a90f-137">**Response**</span></span> 

<span data-ttu-id="5a90f-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5a90f-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```


