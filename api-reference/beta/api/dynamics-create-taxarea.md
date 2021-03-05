---
title: 创建 taxAreas
description: 在 Dynamics for Financials 中创建一个税区对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e30275efd4205b776593b5d515b2032654506a90
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473236"
---
# <a name="create-taxareas"></a><span data-ttu-id="a18f7-103">创建 taxAreas</span><span class="sxs-lookup"><span data-stu-id="a18f7-103">Create taxAreas</span></span>

<span data-ttu-id="a18f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a18f7-105">在 Dynamics 365 商业中心创建税区对象。</span><span class="sxs-lookup"><span data-stu-id="a18f7-105">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a18f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="a18f7-106">Permissions</span></span>
<span data-ttu-id="a18f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a18f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a18f7-109">Permission type</span></span> |<span data-ttu-id="a18f7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a18f7-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a18f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a18f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a18f7-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18f7-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a18f7-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="a18f7-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a18f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a18f7-114">Not supported.</span></span>|
|<span data-ttu-id="a18f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a18f7-115">Application</span></span>|<span data-ttu-id="a18f7-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18f7-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a18f7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a18f7-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a18f7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a18f7-118">Optional query parameters</span></span>
<span data-ttu-id="a18f7-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a18f7-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a18f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a18f7-120">Request headers</span></span>
|<span data-ttu-id="a18f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="a18f7-121">Header</span></span>|<span data-ttu-id="a18f7-122">值</span><span class="sxs-lookup"><span data-stu-id="a18f7-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="a18f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a18f7-123">Authorization</span></span>  |<span data-ttu-id="a18f7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a18f7-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="a18f7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a18f7-126">Content-Type</span></span>  |<span data-ttu-id="a18f7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a18f7-127">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="a18f7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a18f7-128">Request body</span></span>
<span data-ttu-id="a18f7-129">在请求正文中，提供 **taxAreas** 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a18f7-129">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="a18f7-130">响应</span><span class="sxs-lookup"><span data-stu-id="a18f7-130">Response</span></span>
<span data-ttu-id="a18f7-131">如果成功，此方法在响应正文中返回响应 ```201 Created``` 代码和 **taxAreas** 对象。</span><span class="sxs-lookup"><span data-stu-id="a18f7-131">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a18f7-132">示例</span><span class="sxs-lookup"><span data-stu-id="a18f7-132">Example</span></span>

<span data-ttu-id="a18f7-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="a18f7-133">**Request**</span></span>

<span data-ttu-id="a18f7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a18f7-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

{
  "code": "44442001T"
}
```

<span data-ttu-id="a18f7-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="a18f7-135">**Response**</span></span>

```http
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


