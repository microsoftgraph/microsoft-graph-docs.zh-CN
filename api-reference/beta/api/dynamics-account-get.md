---
title: 获取帐户
description: 获取 Dynamics 365 Business Central 中的 account 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f0441a3c2f9385378e767d721c09cb28e87a5682
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956875"
---
# <a name="get-accounts"></a><span data-ttu-id="eb9bf-103">获取帐户</span><span class="sxs-lookup"><span data-stu-id="eb9bf-103">Get accounts</span></span>
<span data-ttu-id="eb9bf-104">检索 Dynamics 365 Business Central 的 account 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-104">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb9bf-105">权限</span><span class="sxs-lookup"><span data-stu-id="eb9bf-105">Permissions</span></span>
<span data-ttu-id="eb9bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb9bf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb9bf-108">Permission type</span></span> |<span data-ttu-id="eb9bf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb9bf-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="eb9bf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb9bf-110">Delegated (work or school account)</span></span>|<span data-ttu-id="eb9bf-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb9bf-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="eb9bf-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="eb9bf-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eb9bf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-113">Not supported.</span></span>|
|<span data-ttu-id="eb9bf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb9bf-114">Application</span></span>|<span data-ttu-id="eb9bf-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb9bf-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="eb9bf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb9bf-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/accounts('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb9bf-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb9bf-117">Optional query parameters</span></span>
<span data-ttu-id="eb9bf-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb9bf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb9bf-119">Request headers</span></span>
|<span data-ttu-id="eb9bf-120">标头</span><span class="sxs-lookup"><span data-stu-id="eb9bf-120">Header</span></span>|<span data-ttu-id="eb9bf-121">值</span><span class="sxs-lookup"><span data-stu-id="eb9bf-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="eb9bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb9bf-122">Authorization</span></span>  |<span data-ttu-id="eb9bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb9bf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb9bf-125">Request body</span></span>
<span data-ttu-id="eb9bf-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb9bf-127">响应</span><span class="sxs-lookup"><span data-stu-id="eb9bf-127">Response</span></span>
<span data-ttu-id="eb9bf-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**accounts**对象。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-128">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb9bf-129">示例</span><span class="sxs-lookup"><span data-stu-id="eb9bf-129">Example</span></span>

<span data-ttu-id="eb9bf-130">**请求**下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-130">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/accounts('{id}')
```

<span data-ttu-id="eb9bf-131">**响应**</span><span class="sxs-lookup"><span data-stu-id="eb9bf-131">**Response**</span></span>

<span data-ttu-id="eb9bf-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="eb9bf-133">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb9bf-134">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb9bf-134">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "id-value",
    "number": "10700",
    "displayName": "Inventory",
    "category": "Assets",
    "subCategory": "Inventory",
    "blocked": false,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```