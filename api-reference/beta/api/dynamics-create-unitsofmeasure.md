---
title: 创建 unitsOfMeasure
description: 在 Dynamics 365 Business Central 中创建度量单位对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f0538fcaee242c0105200b191f9c3c9441fb2538
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431139"
---
# <a name="create-unitsofmeasure"></a><span data-ttu-id="8830b-103">创建 unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="8830b-103">Create unitsOfMeasure</span></span>

<span data-ttu-id="8830b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8830b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8830b-105">在 Dynamics 365 Business Central 中创建度量单位对象。</span><span class="sxs-lookup"><span data-stu-id="8830b-105">Create a units of measure object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="8830b-106">权限</span><span class="sxs-lookup"><span data-stu-id="8830b-106">Permissions</span></span>
<span data-ttu-id="8830b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8830b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8830b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8830b-109">Permission type</span></span> |<span data-ttu-id="8830b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8830b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="8830b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8830b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8830b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8830b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="8830b-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="8830b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8830b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8830b-114">Not supported.</span></span>|
|<span data-ttu-id="8830b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8830b-115">Application</span></span>|<span data-ttu-id="8830b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8830b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8830b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8830b-117">HTTP request</span></span>
```
POST /financials/companies/{id}/unitsOfMeasure
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8830b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8830b-118">Optional query parameters</span></span>
<span data-ttu-id="8830b-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8830b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8830b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8830b-120">Request headers</span></span>
|<span data-ttu-id="8830b-121">标头</span><span class="sxs-lookup"><span data-stu-id="8830b-121">Header</span></span>|<span data-ttu-id="8830b-122">值</span><span class="sxs-lookup"><span data-stu-id="8830b-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="8830b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8830b-123">Authorization</span></span>  |<span data-ttu-id="8830b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8830b-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8830b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8830b-126">Content-Type</span></span>  |<span data-ttu-id="8830b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8830b-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="8830b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8830b-128">Request body</span></span>
<span data-ttu-id="8830b-129">在请求正文中，提供**unitsOfMeasure**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8830b-129">In the request body, supply a JSON representation of a **unitsOfMeasure** object.</span></span>

## <a name="response"></a><span data-ttu-id="8830b-130">响应</span><span class="sxs-lookup"><span data-stu-id="8830b-130">Response</span></span>
<span data-ttu-id="8830b-131">如果成功，此方法在```201 Created```响应正文中返回响应代码和**unitsOfMeasure**对象。</span><span class="sxs-lookup"><span data-stu-id="8830b-131">If successful, this method returns ```201 Created``` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8830b-132">示例</span><span class="sxs-lookup"><span data-stu-id="8830b-132">Example</span></span>

<span data-ttu-id="8830b-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="8830b-133">**Request**</span></span>

<span data-ttu-id="8830b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8830b-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure
Content-type: application/json

{
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA"
}
```

<span data-ttu-id="8830b-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="8830b-135">**Response**</span></span>

<span data-ttu-id="8830b-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8830b-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="8830b-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8830b-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8830b-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8830b-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}

```

