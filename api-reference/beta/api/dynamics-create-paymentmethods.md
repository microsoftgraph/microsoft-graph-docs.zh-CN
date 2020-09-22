---
title: 创建 paymentMethods
description: 在 Dynamics 365 Business Central 中创建付款方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f4e23fd95c4550c43ce78aa0a1c15771afe7672a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981644"
---
# <a name="create-paymentmethods"></a><span data-ttu-id="f57b3-103">创建 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="f57b3-103">Create paymentMethods</span></span>

<span data-ttu-id="f57b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f57b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f57b3-105">在 DDynamics 365 Business Central 中创建付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="f57b3-105">Create a payment method object in DDynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f57b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="f57b3-106">Permissions</span></span>
<span data-ttu-id="f57b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f57b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f57b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f57b3-109">Permission type</span></span> |<span data-ttu-id="f57b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f57b3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f57b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f57b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f57b3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f57b3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f57b3-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="f57b3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f57b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f57b3-114">Not supported.</span></span>|
|<span data-ttu-id="f57b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f57b3-115">Application</span></span>|<span data-ttu-id="f57b3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f57b3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f57b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f57b3-117">HTTP request</span></span>
```
POST /financials/companies/{id}/paymentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f57b3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f57b3-118">Optional query parameters</span></span>
<span data-ttu-id="f57b3-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f57b3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f57b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f57b3-120">Request headers</span></span>
|<span data-ttu-id="f57b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="f57b3-121">Header</span></span>         |<span data-ttu-id="f57b3-122">值</span><span class="sxs-lookup"><span data-stu-id="f57b3-122">Value</span></span>                        |
|---------------|-----------------------------|
|<span data-ttu-id="f57b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f57b3-123">Authorization</span></span>  |<span data-ttu-id="f57b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f57b3-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="f57b3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f57b3-126">Content-Type</span></span>   |<span data-ttu-id="f57b3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f57b3-127">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="f57b3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f57b3-128">Request body</span></span>
<span data-ttu-id="f57b3-129">在请求正文中，提供 **paymentMethods** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f57b3-129">In the request body, supply a JSON representation of a **paymentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="f57b3-130">响应</span><span class="sxs-lookup"><span data-stu-id="f57b3-130">Response</span></span>
<span data-ttu-id="f57b3-131">如果成功，此方法 ```201 Created``` 在响应正文中返回响应代码和 **paymentMethods** 对象。</span><span class="sxs-lookup"><span data-stu-id="f57b3-131">If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f57b3-132">示例</span><span class="sxs-lookup"><span data-stu-id="f57b3-132">Example</span></span>

<span data-ttu-id="f57b3-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="f57b3-133">**Request**</span></span>

<span data-ttu-id="f57b3-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f57b3-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

<span data-ttu-id="f57b3-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="f57b3-135">**Response**</span></span>

<span data-ttu-id="f57b3-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f57b3-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="f57b3-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f57b3-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f57b3-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f57b3-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```



