---
title: 获取 itemCategories
description: 获取 Dynamics 365 Business Central 中的项类别。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7e339b89f53b0f7c3cd8f5dfc7976ba931bcaffd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458374"
---
# <a name="get-itemcategories"></a><span data-ttu-id="1ff52-103">获取 itemCategories</span><span class="sxs-lookup"><span data-stu-id="1ff52-103">Get itemCategories</span></span>
<span data-ttu-id="1ff52-104">检索 Dynamics 365 Business Central 的 item category 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ff52-104">Retrieve the properties and relationships of an item category object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ff52-105">权限</span><span class="sxs-lookup"><span data-stu-id="1ff52-105">Permissions</span></span>
<span data-ttu-id="1ff52-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ff52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff52-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ff52-108">Permission type</span></span> |<span data-ttu-id="1ff52-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ff52-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="1ff52-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ff52-110">Delegated (work or school account)</span></span>|<span data-ttu-id="1ff52-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff52-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="1ff52-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="1ff52-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1ff52-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ff52-113">Not supported.</span></span>|
|<span data-ttu-id="1ff52-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ff52-114">Application</span></span>|<span data-ttu-id="1ff52-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff52-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ff52-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ff52-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/itemCategories('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ff52-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ff52-117">Optional query parameters</span></span>
<span data-ttu-id="1ff52-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ff52-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ff52-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ff52-119">Request headers</span></span>
|<span data-ttu-id="1ff52-120">标头</span><span class="sxs-lookup"><span data-stu-id="1ff52-120">Header</span></span>       |<span data-ttu-id="1ff52-121">值</span><span class="sxs-lookup"><span data-stu-id="1ff52-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="1ff52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ff52-122">Authorization</span></span>|<span data-ttu-id="1ff52-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ff52-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ff52-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ff52-125">Request body</span></span>
<span data-ttu-id="1ff52-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ff52-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff52-127">响应</span><span class="sxs-lookup"><span data-stu-id="1ff52-127">Response</span></span>
<span data-ttu-id="1ff52-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**itemCategories**对象。</span><span class="sxs-lookup"><span data-stu-id="1ff52-128">If successful, this method returns a `200 OK` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ff52-129">示例</span><span class="sxs-lookup"><span data-stu-id="1ff52-129">Example</span></span>

<span data-ttu-id="1ff52-130">**请求**</span><span class="sxs-lookup"><span data-stu-id="1ff52-130">**Request**</span></span>

<span data-ttu-id="1ff52-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ff52-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories('{id}')
```

<span data-ttu-id="1ff52-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="1ff52-132">**Response**</span></span>

<span data-ttu-id="1ff52-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1ff52-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="1ff52-134">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1ff52-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ff52-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ff52-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}
```

