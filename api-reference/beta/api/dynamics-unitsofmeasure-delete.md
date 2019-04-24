---
title: 删除 unitsOfMeasure
description: 删除 Dynamics 365 Business Central 中的度量单位对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 571fc240ecaa244132278455ee64a8ad879ae030
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464374"
---
# <a name="delete-unitsofmeasure"></a><span data-ttu-id="e2d72-103">删除 unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="e2d72-103">Delete unitsOfMeasure</span></span>
<span data-ttu-id="e2d72-104">从 Dynamics 365 Business Central 中删除度量单位对象。</span><span class="sxs-lookup"><span data-stu-id="e2d72-104">Deletes a units of measure object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2d72-105">权限</span><span class="sxs-lookup"><span data-stu-id="e2d72-105">Permissions</span></span>
<span data-ttu-id="e2d72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2d72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2d72-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2d72-108">Permission type</span></span> |<span data-ttu-id="e2d72-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2d72-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e2d72-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2d72-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e2d72-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d72-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e2d72-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e2d72-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e2d72-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2d72-113">Not supported.</span></span>|
|<span data-ttu-id="e2d72-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2d72-114">Application</span></span>|<span data-ttu-id="e2d72-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d72-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2d72-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2d72-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/unitsOfMeasure('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2d72-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2d72-117">Optional query parameters</span></span>
<span data-ttu-id="e2d72-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2d72-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2d72-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2d72-119">Request headers</span></span>
|<span data-ttu-id="e2d72-120">标头</span><span class="sxs-lookup"><span data-stu-id="e2d72-120">Header</span></span>|<span data-ttu-id="e2d72-121">值</span><span class="sxs-lookup"><span data-stu-id="e2d72-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="e2d72-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2d72-122">Authorization</span></span>  |<span data-ttu-id="e2d72-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2d72-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e2d72-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="e2d72-125">If-Match</span></span>       |<span data-ttu-id="e2d72-126">必需。</span><span class="sxs-lookup"><span data-stu-id="e2d72-126">Required.</span></span> <span data-ttu-id="e2d72-127">如果包含此请求标头, 且提供的 eTag 与**unitsOfMeasure**上的当前标记不匹配, 则不会更新**unitsOfMeasure** 。</span><span class="sxs-lookup"><span data-stu-id="e2d72-127">When this request header is included and the eTag provided does not match the current tag on the **unitsOfMeasure**, the **unitsOfMeasure** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2d72-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2d72-128">Request body</span></span>
<span data-ttu-id="e2d72-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2d72-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2d72-130">响应</span><span class="sxs-lookup"><span data-stu-id="e2d72-130">Response</span></span>
<span data-ttu-id="e2d72-p104">如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e2d72-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2d72-133">示例</span><span class="sxs-lookup"><span data-stu-id="e2d72-133">Example</span></span>

<span data-ttu-id="e2d72-134">**请求**</span><span class="sxs-lookup"><span data-stu-id="e2d72-134">**Request**</span></span>

<span data-ttu-id="e2d72-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2d72-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/unitsOfMeasure('{id}')
```

<span data-ttu-id="e2d72-136">**响应**</span><span class="sxs-lookup"><span data-stu-id="e2d72-136">**Response**</span></span> 

<span data-ttu-id="e2d72-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2d72-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
