---
title: 创建 shipmentMethods
description: 在 Dynamics 365 Business Central 中创建装运方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4c9ce592c2cc24aa9cac0731b678c473a9c18447
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791937"
---
# <a name="create-shipmentmethods"></a><span data-ttu-id="6d2ed-103">创建 shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="6d2ed-103">Create shipmentMethods</span></span>
<span data-ttu-id="6d2ed-104">在 Dynamics 365 Business Central 中创建装运方法对象。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-104">Create a shipment method object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d2ed-105">权限</span><span class="sxs-lookup"><span data-stu-id="6d2ed-105">Permissions</span></span>
<span data-ttu-id="6d2ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d2ed-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d2ed-108">Permission type</span></span> |<span data-ttu-id="6d2ed-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d2ed-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6d2ed-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d2ed-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6d2ed-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2ed-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6d2ed-112">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="6d2ed-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6d2ed-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-113">Not supported.</span></span>|
|<span data-ttu-id="6d2ed-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d2ed-114">Application</span></span>|<span data-ttu-id="6d2ed-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2ed-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d2ed-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d2ed-116">HTTP request</span></span>
```
POST /financials/companies/{id}/shipmentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d2ed-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d2ed-117">Optional query parameters</span></span>
<span data-ttu-id="6d2ed-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d2ed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d2ed-119">Request headers</span></span>

|<span data-ttu-id="6d2ed-120">标头</span><span class="sxs-lookup"><span data-stu-id="6d2ed-120">Header</span></span>         |<span data-ttu-id="6d2ed-121">值</span><span class="sxs-lookup"><span data-stu-id="6d2ed-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="6d2ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d2ed-122">Authorization</span></span>  |<span data-ttu-id="6d2ed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="6d2ed-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d2ed-125">Content-Type</span></span>   |<span data-ttu-id="6d2ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d2ed-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="6d2ed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d2ed-127">Request body</span></span>
<span data-ttu-id="6d2ed-128">在请求正文中，提供**shipmentMethods**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-128">In the request body, supply a JSON representation of a **shipmentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="6d2ed-129">响应</span><span class="sxs-lookup"><span data-stu-id="6d2ed-129">Response</span></span>
<span data-ttu-id="6d2ed-130">如果成功，此方法在```201 Created```响应正文中返回响应代码和**shipmentMethods**对象。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-130">If successful, this method returns ```201 Created``` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d2ed-131">示例</span><span class="sxs-lookup"><span data-stu-id="6d2ed-131">Example</span></span>

<span data-ttu-id="6d2ed-132">**请求**</span><span class="sxs-lookup"><span data-stu-id="6d2ed-132">**Request**</span></span>

<span data-ttu-id="6d2ed-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods
Content-type: application/json

{
  "code": "PICKUP",
  "displayName": "Pickup at Location"  
}
```

<span data-ttu-id="6d2ed-134">**响应**</span><span class="sxs-lookup"><span data-stu-id="6d2ed-134">**Response**</span></span>

<span data-ttu-id="6d2ed-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="6d2ed-136">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d2ed-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6d2ed-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}

```
