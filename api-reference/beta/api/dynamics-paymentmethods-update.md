---
title: 更新 paymentMethods
description: 更新 Dynamics 365 Business Central 中的付款方式对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7db0c249c272561e9276091c3f06db37c8644575
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045129"
---
# <a name="update-paymentmethods"></a><span data-ttu-id="7aa96-103">更新 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="7aa96-103">Update paymentMethods</span></span>

<span data-ttu-id="7aa96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aa96-105">更新 Dynamics 365 Business Central 的付款方式对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7aa96-105">Update the properties of a payment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa96-106">权限</span><span class="sxs-lookup"><span data-stu-id="7aa96-106">Permissions</span></span>
<span data-ttu-id="7aa96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7aa96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aa96-109">Permission type</span></span> |<span data-ttu-id="7aa96-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7aa96-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7aa96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aa96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7aa96-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa96-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7aa96-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="7aa96-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7aa96-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aa96-114">Not supported.</span></span>|
|<span data-ttu-id="7aa96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aa96-115">Application</span></span>|<span data-ttu-id="7aa96-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa96-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aa96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aa96-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7aa96-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7aa96-118">Optional query parameters</span></span>
<span data-ttu-id="7aa96-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7aa96-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aa96-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aa96-120">Request headers</span></span>
|<span data-ttu-id="7aa96-121">标头</span><span class="sxs-lookup"><span data-stu-id="7aa96-121">Header</span></span>        |<span data-ttu-id="7aa96-122">值</span><span class="sxs-lookup"><span data-stu-id="7aa96-122">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="7aa96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa96-123">Authorization</span></span> |<span data-ttu-id="7aa96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7aa96-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="7aa96-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aa96-126">Content-Type</span></span>  |<span data-ttu-id="7aa96-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7aa96-127">application/json</span></span>          |
|<span data-ttu-id="7aa96-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="7aa96-128">If-Match</span></span>      |<span data-ttu-id="7aa96-129">必需。</span><span class="sxs-lookup"><span data-stu-id="7aa96-129">Required.</span></span> <span data-ttu-id="7aa96-130">如果包含此请求标头且提供的 eTag 与 **paymentMethods** 上的当前标记不匹配，则 **paymentMethods** 将不会更新。</span><span class="sxs-lookup"><span data-stu-id="7aa96-130">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aa96-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aa96-131">Request body</span></span>
<span data-ttu-id="7aa96-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7aa96-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="7aa96-135">响应</span><span class="sxs-lookup"><span data-stu-id="7aa96-135">Response</span></span>
<span data-ttu-id="7aa96-136">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` **paymentMethods** 对象。</span><span class="sxs-lookup"><span data-stu-id="7aa96-136">If successful, this method returns a `200 OK` response code and an updated **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa96-137">示例</span><span class="sxs-lookup"><span data-stu-id="7aa96-137">Example</span></span>

<span data-ttu-id="7aa96-138">**请求**</span><span class="sxs-lookup"><span data-stu-id="7aa96-138">**Request**</span></span>

<span data-ttu-id="7aa96-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7aa96-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
Content-type: application/json

{
  "displayName": "Personal Check Payment",
}
```

<span data-ttu-id="7aa96-140">**响应**</span><span class="sxs-lookup"><span data-stu-id="7aa96-140">**Response**</span></span>

<span data-ttu-id="7aa96-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7aa96-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="7aa96-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7aa96-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Personal Check Payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}
```




