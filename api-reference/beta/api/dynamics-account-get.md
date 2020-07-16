---
title: 获取帐户
description: 获取 Dynamics 365 Business Central 中的 account 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 19ef71bd9103ffe257d5a0201e1fde322a78dd0c
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142209"
---
# <a name="get-accounts"></a><span data-ttu-id="2de5c-103">获取帐户</span><span class="sxs-lookup"><span data-stu-id="2de5c-103">Get accounts</span></span>

<span data-ttu-id="2de5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2de5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2de5c-105">检索 Dynamics 365 Business Central 的 account 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2de5c-105">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2de5c-106">权限</span><span class="sxs-lookup"><span data-stu-id="2de5c-106">Permissions</span></span>
<span data-ttu-id="2de5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2de5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2de5c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2de5c-109">Permission type</span></span> |<span data-ttu-id="2de5c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2de5c-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2de5c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2de5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2de5c-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de5c-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2de5c-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="2de5c-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2de5c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2de5c-114">Not supported.</span></span>|
|<span data-ttu-id="2de5c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2de5c-115">Application</span></span>|<span data-ttu-id="2de5c-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de5c-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="2de5c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2de5c-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2de5c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2de5c-118">Optional query parameters</span></span>
<span data-ttu-id="2de5c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2de5c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2de5c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2de5c-120">Request headers</span></span>
|<span data-ttu-id="2de5c-121">标头</span><span class="sxs-lookup"><span data-stu-id="2de5c-121">Header</span></span>|<span data-ttu-id="2de5c-122">值</span><span class="sxs-lookup"><span data-stu-id="2de5c-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="2de5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2de5c-123">Authorization</span></span>  |<span data-ttu-id="2de5c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2de5c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2de5c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2de5c-126">Request body</span></span>
<span data-ttu-id="2de5c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2de5c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2de5c-128">响应</span><span class="sxs-lookup"><span data-stu-id="2de5c-128">Response</span></span>
<span data-ttu-id="2de5c-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**accounts**对象。</span><span class="sxs-lookup"><span data-stu-id="2de5c-129">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2de5c-130">示例</span><span class="sxs-lookup"><span data-stu-id="2de5c-130">Example</span></span>

<span data-ttu-id="2de5c-131">**请求**下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2de5c-131">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/accounts/{id}
```

<span data-ttu-id="2de5c-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="2de5c-132">**Response**</span></span>

<span data-ttu-id="2de5c-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2de5c-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="2de5c-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2de5c-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2de5c-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2de5c-135">All the properties will be returned from an actual call.</span></span>

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
