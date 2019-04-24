---
title: 删除 paymentMethods
description: 删除 Dynamics 365 Business Central 中的付款方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7b418160573eb9acf2f0c9e9f2ab0d352b59d846
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458325"
---
# <a name="delete-paymentmethods"></a><span data-ttu-id="e5817-103">删除 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="e5817-103">Delete paymentMethods</span></span>
<span data-ttu-id="e5817-104">从 Dynamics 365 Business Central 中删除付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="e5817-104">Delete a payment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5817-105">权限</span><span class="sxs-lookup"><span data-stu-id="e5817-105">Permissions</span></span>
<span data-ttu-id="e5817-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5817-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5817-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5817-108">Permission type</span></span> |<span data-ttu-id="e5817-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5817-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e5817-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5817-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e5817-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5817-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e5817-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e5817-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e5817-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5817-113">Not supported.</span></span>|
|<span data-ttu-id="e5817-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5817-114">Application</span></span>|<span data-ttu-id="e5817-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5817-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5817-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5817-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/paymentMethods('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5817-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e5817-117">Optional query parameters</span></span>
<span data-ttu-id="e5817-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5817-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5817-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5817-119">Request headers</span></span>

|<span data-ttu-id="e5817-120">标头</span><span class="sxs-lookup"><span data-stu-id="e5817-120">Header</span></span>         |<span data-ttu-id="e5817-121">值</span><span class="sxs-lookup"><span data-stu-id="e5817-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="e5817-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5817-122">Authorization</span></span>  |<span data-ttu-id="e5817-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5817-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e5817-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="e5817-125">If-Match</span></span>       |<span data-ttu-id="e5817-126">必需。</span><span class="sxs-lookup"><span data-stu-id="e5817-126">Required.</span></span> <span data-ttu-id="e5817-127">如果包含此请求标头, 且提供的 eTag 与**paymentMethods**上的当前标记不匹配, 则不会更新**paymentMethods** 。</span><span class="sxs-lookup"><span data-stu-id="e5817-127">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5817-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5817-128">Request body</span></span>
<span data-ttu-id="e5817-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5817-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5817-130">响应</span><span class="sxs-lookup"><span data-stu-id="e5817-130">Response</span></span>
<span data-ttu-id="e5817-p104">如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e5817-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5817-133">示例</span><span class="sxs-lookup"><span data-stu-id="e5817-133">Example</span></span>

<span data-ttu-id="e5817-134">**请求**</span><span class="sxs-lookup"><span data-stu-id="e5817-134">**Request**</span></span>

<span data-ttu-id="e5817-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5817-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/paymentMethods('{id}')
```

<span data-ttu-id="e5817-136">**响应**</span><span class="sxs-lookup"><span data-stu-id="e5817-136">**Response**</span></span> 

<span data-ttu-id="e5817-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5817-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

