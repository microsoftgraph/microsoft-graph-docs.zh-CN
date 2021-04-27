---
title: 获取 unitsOfMeasure
description: 获取 Dynamics 365 Business Central 中的度量单位对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f374de8c500660ed423bc7a264cb37dd9f5c690f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044842"
---
# <a name="get-unitsofmeasure"></a><span data-ttu-id="f1536-103">获取 unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="f1536-103">Get unitsOfMeasure</span></span>

<span data-ttu-id="f1536-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1536-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1536-105">检索 Dynamics 365 Business Central 的度量对象单元的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1536-105">Retrieve the properties and relationships of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1536-106">权限</span><span class="sxs-lookup"><span data-stu-id="f1536-106">Permissions</span></span>
<span data-ttu-id="f1536-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1536-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1536-109">Permission type</span></span> |<span data-ttu-id="f1536-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1536-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f1536-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1536-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1536-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1536-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f1536-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="f1536-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f1536-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1536-114">Not supported.</span></span>|
|<span data-ttu-id="f1536-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1536-115">Application</span></span>|<span data-ttu-id="f1536-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1536-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1536-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1536-117">HTTP request</span></span>

```
GET /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1536-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f1536-118">Optional query parameters</span></span>
<span data-ttu-id="f1536-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f1536-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1536-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1536-120">Request headers</span></span>
|<span data-ttu-id="f1536-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1536-121">Header</span></span>|<span data-ttu-id="f1536-122">值</span><span class="sxs-lookup"><span data-stu-id="f1536-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="f1536-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1536-123">Authorization</span></span>  |<span data-ttu-id="f1536-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1536-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1536-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1536-126">Request body</span></span>
<span data-ttu-id="f1536-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1536-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1536-128">响应</span><span class="sxs-lookup"><span data-stu-id="f1536-128">Response</span></span>
<span data-ttu-id="f1536-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **unitsOfMeasure** 对象。</span><span class="sxs-lookup"><span data-stu-id="f1536-129">If successful, this method returns a `200 OK` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1536-130">示例</span><span class="sxs-lookup"><span data-stu-id="f1536-130">Example</span></span>

<span data-ttu-id="f1536-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="f1536-131">**Request**</span></span>

<span data-ttu-id="f1536-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1536-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
```

<span data-ttu-id="f1536-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="f1536-133">**Response**</span></span>

<span data-ttu-id="f1536-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f1536-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="f1536-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f1536-135">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```


