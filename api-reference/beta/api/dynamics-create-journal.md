---
title: 创建日记
description: 在 Dynamics 365 Business Central 中创建日记对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e67c1692ce6a0e6579070f0c8d420798e67c4e61
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473285"
---
# <a name="create-journals"></a><span data-ttu-id="d0be9-103">创建日记</span><span class="sxs-lookup"><span data-stu-id="d0be9-103">Create journals</span></span>

<span data-ttu-id="d0be9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0be9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0be9-105">在 Dynamics 365 商业中心创建日记。</span><span class="sxs-lookup"><span data-stu-id="d0be9-105">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d0be9-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0be9-106">Permissions</span></span>
<span data-ttu-id="d0be9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0be9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0be9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0be9-109">Permission type</span></span> |<span data-ttu-id="d0be9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0be9-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d0be9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0be9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0be9-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0be9-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d0be9-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="d0be9-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d0be9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0be9-114">Not supported.</span></span>|
|<span data-ttu-id="d0be9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0be9-115">Application</span></span>|<span data-ttu-id="d0be9-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0be9-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0be9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0be9-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0be9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d0be9-118">Optional query parameters</span></span>
<span data-ttu-id="d0be9-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d0be9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0be9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0be9-120">Request headers</span></span>
|<span data-ttu-id="d0be9-121">标头</span><span class="sxs-lookup"><span data-stu-id="d0be9-121">Header</span></span>        |<span data-ttu-id="d0be9-122">值</span><span class="sxs-lookup"><span data-stu-id="d0be9-122">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="d0be9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0be9-123">Authorization</span></span> |<span data-ttu-id="d0be9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0be9-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d0be9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0be9-126">Content-Type</span></span>  |<span data-ttu-id="d0be9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d0be9-127">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="d0be9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0be9-128">Request body</span></span>
<span data-ttu-id="d0be9-129">在请求正文中，提供日记对象的 JSON **表示** 形式。</span><span class="sxs-lookup"><span data-stu-id="d0be9-129">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="d0be9-130">响应</span><span class="sxs-lookup"><span data-stu-id="d0be9-130">Response</span></span>
<span data-ttu-id="d0be9-131">如果成功，此方法在响应正文中返回响应代码 ```201 Created``` 和日记对象。 </span><span class="sxs-lookup"><span data-stu-id="d0be9-131">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0be9-132">示例</span><span class="sxs-lookup"><span data-stu-id="d0be9-132">Example</span></span>

<span data-ttu-id="d0be9-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="d0be9-133">**Request**</span></span>

<span data-ttu-id="d0be9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0be9-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals
Content-type: application/json

{
  "code": "DEFAULT"
}
```

<span data-ttu-id="d0be9-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="d0be9-135">**Response**</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



