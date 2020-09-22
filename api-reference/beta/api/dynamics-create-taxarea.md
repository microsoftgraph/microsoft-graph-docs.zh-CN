---
title: 创建 taxAreas
description: 在 Dynamics 中创建金融的税务区域对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7f2da2cc9540b1dc3d884fffe3a89fc50dbf32c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981607"
---
# <a name="create-taxareas"></a><span data-ttu-id="d07ab-103">创建 taxAreas</span><span class="sxs-lookup"><span data-stu-id="d07ab-103">Create taxAreas</span></span>

<span data-ttu-id="d07ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d07ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d07ab-105">在 Dynamics 365 Business Central 中创建税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="d07ab-105">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d07ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="d07ab-106">Permissions</span></span>
<span data-ttu-id="d07ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d07ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d07ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d07ab-109">Permission type</span></span> |<span data-ttu-id="d07ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d07ab-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d07ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d07ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d07ab-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d07ab-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d07ab-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="d07ab-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d07ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d07ab-114">Not supported.</span></span>|
|<span data-ttu-id="d07ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d07ab-115">Application</span></span>|<span data-ttu-id="d07ab-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d07ab-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d07ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d07ab-117">HTTP request</span></span>

```
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d07ab-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d07ab-118">Optional query parameters</span></span>
<span data-ttu-id="d07ab-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d07ab-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d07ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d07ab-120">Request headers</span></span>
|<span data-ttu-id="d07ab-121">标头</span><span class="sxs-lookup"><span data-stu-id="d07ab-121">Header</span></span>|<span data-ttu-id="d07ab-122">值</span><span class="sxs-lookup"><span data-stu-id="d07ab-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="d07ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d07ab-123">Authorization</span></span>  |<span data-ttu-id="d07ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d07ab-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="d07ab-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d07ab-126">Content-Type</span></span>  |<span data-ttu-id="d07ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d07ab-127">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="d07ab-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d07ab-128">Request body</span></span>
<span data-ttu-id="d07ab-129">在请求正文中，提供 **taxAreas** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d07ab-129">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="d07ab-130">响应</span><span class="sxs-lookup"><span data-stu-id="d07ab-130">Response</span></span>
<span data-ttu-id="d07ab-131">如果成功，此方法 ```201 Created``` 在响应正文中返回响应代码和 **taxAreas** 对象。</span><span class="sxs-lookup"><span data-stu-id="d07ab-131">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d07ab-132">示例</span><span class="sxs-lookup"><span data-stu-id="d07ab-132">Example</span></span>

<span data-ttu-id="d07ab-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="d07ab-133">**Request**</span></span>

<span data-ttu-id="d07ab-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d07ab-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

```json
{
  "code": "44442001T"
}
```

<span data-ttu-id="d07ab-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="d07ab-135">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "44442001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


