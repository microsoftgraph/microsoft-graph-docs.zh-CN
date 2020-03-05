---
title: 删除日记
description: 删除 Dynamics 365 Business Central 中的日记对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ff9b50f7e0b1a4b6580cc2ba328d98a9dcd8b132
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42429347"
---
# <a name="delete-journals"></a><span data-ttu-id="50bb3-103">删除日记</span><span class="sxs-lookup"><span data-stu-id="50bb3-103">Delete journals</span></span>

<span data-ttu-id="50bb3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="50bb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50bb3-105">从 Dynamics 365 Business Central 中删除日记。</span><span class="sxs-lookup"><span data-stu-id="50bb3-105">Delete a journal from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="50bb3-106">权限</span><span class="sxs-lookup"><span data-stu-id="50bb3-106">Permissions</span></span>
<span data-ttu-id="50bb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50bb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50bb3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="50bb3-109">Permission type</span></span> |<span data-ttu-id="50bb3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50bb3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="50bb3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50bb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50bb3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50bb3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="50bb3-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="50bb3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="50bb3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="50bb3-114">Not supported.</span></span>|
|<span data-ttu-id="50bb3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="50bb3-115">Application</span></span>|<span data-ttu-id="50bb3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50bb3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50bb3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50bb3-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50bb3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50bb3-118">Optional query parameters</span></span>
<span data-ttu-id="50bb3-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="50bb3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50bb3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="50bb3-120">Request headers</span></span>
|<span data-ttu-id="50bb3-121">标头</span><span class="sxs-lookup"><span data-stu-id="50bb3-121">Header</span></span>         |<span data-ttu-id="50bb3-122">值</span><span class="sxs-lookup"><span data-stu-id="50bb3-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="50bb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50bb3-123">Authorization</span></span>  |<span data-ttu-id="50bb3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50bb3-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="50bb3-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="50bb3-126">If-Match</span></span>       |<span data-ttu-id="50bb3-127">必填。</span><span class="sxs-lookup"><span data-stu-id="50bb3-127">Required.</span></span> <span data-ttu-id="50bb3-128">如果包含此请求标头，且提供的 eTag 与**日记**中的当前标记不匹配，则不会更新**日记**。</span><span class="sxs-lookup"><span data-stu-id="50bb3-128">When this request header is included and the eTag provided does not match the current tag on the **journals**, the **journals** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50bb3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="50bb3-129">Request body</span></span>

<span data-ttu-id="50bb3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50bb3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50bb3-131">响应</span><span class="sxs-lookup"><span data-stu-id="50bb3-131">Response</span></span>

<span data-ttu-id="50bb3-p104">如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="50bb3-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50bb3-134">示例</span><span class="sxs-lookup"><span data-stu-id="50bb3-134">Example</span></span>

<span data-ttu-id="50bb3-135">**请求**</span><span class="sxs-lookup"><span data-stu-id="50bb3-135">**Request**</span></span>

<span data-ttu-id="50bb3-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50bb3-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}
```

<span data-ttu-id="50bb3-137">**响应**</span><span class="sxs-lookup"><span data-stu-id="50bb3-137">**Response**</span></span> 

<span data-ttu-id="50bb3-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="50bb3-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
