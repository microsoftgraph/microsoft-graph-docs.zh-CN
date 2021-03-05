---
title: 获取 dimensionValues
description: 获取 Dynamics 365 Business Central 中的维度值对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 07ae48484d619c9bc883641066b978a6431ead16
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473131"
---
# <a name="get-dimensionvalues"></a><span data-ttu-id="18add-103">获取 dimensionValues</span><span class="sxs-lookup"><span data-stu-id="18add-103">Get dimensionValues</span></span>

<span data-ttu-id="18add-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18add-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18add-105">检索 Dynamics 365 Business Central 的维度值对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="18add-105">Retrieve the properties and relationships of a dimension value object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="18add-106">权限</span><span class="sxs-lookup"><span data-stu-id="18add-106">Permissions</span></span>
<span data-ttu-id="18add-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18add-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18add-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18add-109">Permission type</span></span> |<span data-ttu-id="18add-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18add-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="18add-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18add-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18add-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18add-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="18add-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="18add-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="18add-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18add-114">Not supported.</span></span>|
|<span data-ttu-id="18add-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18add-115">Application</span></span>|<span data-ttu-id="18add-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18add-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18add-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18add-117">HTTP request</span></span>

```
GET /financials/companies/{id}/dimensions/{id}/dimensionValues/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18add-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="18add-118">Optional query parameters</span></span>
<span data-ttu-id="18add-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="18add-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18add-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18add-120">Request headers</span></span>
|<span data-ttu-id="18add-121">标头</span><span class="sxs-lookup"><span data-stu-id="18add-121">Header</span></span>       |<span data-ttu-id="18add-122">值</span><span class="sxs-lookup"><span data-stu-id="18add-122">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="18add-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18add-123">Authorization</span></span>|<span data-ttu-id="18add-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18add-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18add-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="18add-126">Request body</span></span>
<span data-ttu-id="18add-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18add-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18add-128">响应</span><span class="sxs-lookup"><span data-stu-id="18add-128">Response</span></span>
<span data-ttu-id="18add-129">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 **dimensionValues** 对象。</span><span class="sxs-lookup"><span data-stu-id="18add-129">If successful, this method returns a `200 OK` response code and a **dimensionValues** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18add-130">示例</span><span class="sxs-lookup"><span data-stu-id="18add-130">Example</span></span>

<span data-ttu-id="18add-131">**请求**</span><span class="sxs-lookup"><span data-stu-id="18add-131">**Request**</span></span>

<span data-ttu-id="18add-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18add-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/dimensions/{id}/dimensionValues/{id}
```

<span data-ttu-id="18add-133">**响应**</span><span class="sxs-lookup"><span data-stu-id="18add-133">**Response**</span></span>

<span data-ttu-id="18add-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="18add-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="18add-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="18add-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18add-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18add-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "30",
  "displayName": "Europe North (EU)",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```



