---
title: 获取尺寸
description: 获取 Dynamics 365 Business Central 中的 dimension 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 238b289679af5de7698801e763fbf54319e4c10f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464358"
---
# <a name="get-dimensions"></a><span data-ttu-id="723e9-103">获取尺寸</span><span class="sxs-lookup"><span data-stu-id="723e9-103">Get dimensions</span></span>
<span data-ttu-id="723e9-104">检索 Dynamics 365 Business Central 的**维度**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="723e9-104">Retrieve the properties and relationships of a **dimensions** object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="723e9-105">权限</span><span class="sxs-lookup"><span data-stu-id="723e9-105">Permissions</span></span>
<span data-ttu-id="723e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="723e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="723e9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="723e9-108">Permission type</span></span> |<span data-ttu-id="723e9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="723e9-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="723e9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="723e9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="723e9-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723e9-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="723e9-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="723e9-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="723e9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="723e9-113">Not supported.</span></span>|
|<span data-ttu-id="723e9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="723e9-114">Application</span></span>|<span data-ttu-id="723e9-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723e9-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="723e9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="723e9-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/dimensions('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="723e9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="723e9-117">Optional query parameters</span></span>
<span data-ttu-id="723e9-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="723e9-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="723e9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="723e9-119">Request headers</span></span>
|<span data-ttu-id="723e9-120">标头</span><span class="sxs-lookup"><span data-stu-id="723e9-120">Header</span></span>|<span data-ttu-id="723e9-121">值</span><span class="sxs-lookup"><span data-stu-id="723e9-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="723e9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="723e9-122">Authorization</span></span>  |<span data-ttu-id="723e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="723e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="723e9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="723e9-125">Request body</span></span>
<span data-ttu-id="723e9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="723e9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="723e9-127">响应</span><span class="sxs-lookup"><span data-stu-id="723e9-127">Response</span></span>
<span data-ttu-id="723e9-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**维度**对象。</span><span class="sxs-lookup"><span data-stu-id="723e9-128">If successful, this method returns a `200 OK` response code and a **dimensions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="723e9-129">示例</span><span class="sxs-lookup"><span data-stu-id="723e9-129">Example</span></span>

<span data-ttu-id="723e9-130">**请求**</span><span class="sxs-lookup"><span data-stu-id="723e9-130">**Request**</span></span>

<span data-ttu-id="723e9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="723e9-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/dimensions('{id}')
```

<span data-ttu-id="723e9-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="723e9-132">**Response**</span></span>

<span data-ttu-id="723e9-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="723e9-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="723e9-134">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="723e9-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="723e9-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="723e9-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "AREA",
  "displayName": "Area",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

