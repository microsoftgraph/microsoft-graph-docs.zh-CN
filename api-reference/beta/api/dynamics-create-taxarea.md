---
title: 创建 taxAreas
description: 在 Dynamics 中创建金融的税务区域对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c3d2061a4e1c3d78f6ee305bfe87ca82f992ac8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431209"
---
# <a name="create-taxareas"></a><span data-ttu-id="273dc-103">创建 taxAreas</span><span class="sxs-lookup"><span data-stu-id="273dc-103">Create taxAreas</span></span>

<span data-ttu-id="273dc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="273dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="273dc-105">在 Dynamics 365 Business Central 中创建税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="273dc-105">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="273dc-106">权限</span><span class="sxs-lookup"><span data-stu-id="273dc-106">Permissions</span></span>
<span data-ttu-id="273dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="273dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="273dc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="273dc-109">Permission type</span></span> |<span data-ttu-id="273dc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="273dc-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="273dc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="273dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="273dc-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="273dc-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="273dc-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="273dc-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="273dc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="273dc-114">Not supported.</span></span>|
|<span data-ttu-id="273dc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="273dc-115">Application</span></span>|<span data-ttu-id="273dc-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="273dc-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="273dc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="273dc-117">HTTP request</span></span>

```
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="273dc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="273dc-118">Optional query parameters</span></span>
<span data-ttu-id="273dc-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="273dc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="273dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="273dc-120">Request headers</span></span>
|<span data-ttu-id="273dc-121">标头</span><span class="sxs-lookup"><span data-stu-id="273dc-121">Header</span></span>|<span data-ttu-id="273dc-122">值</span><span class="sxs-lookup"><span data-stu-id="273dc-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="273dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="273dc-123">Authorization</span></span>  |<span data-ttu-id="273dc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="273dc-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="273dc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="273dc-126">Content-Type</span></span>  |<span data-ttu-id="273dc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="273dc-127">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="273dc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="273dc-128">Request body</span></span>
<span data-ttu-id="273dc-129">在请求正文中，提供**taxAreas**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="273dc-129">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="273dc-130">响应</span><span class="sxs-lookup"><span data-stu-id="273dc-130">Response</span></span>
<span data-ttu-id="273dc-131">如果成功，此方法在```201 Created```响应正文中返回响应代码和**taxAreas**对象。</span><span class="sxs-lookup"><span data-stu-id="273dc-131">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="273dc-132">示例</span><span class="sxs-lookup"><span data-stu-id="273dc-132">Example</span></span>

<span data-ttu-id="273dc-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="273dc-133">**Request**</span></span>

<span data-ttu-id="273dc-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="273dc-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

```json
{
  "code": "44442001T"
}
```

<span data-ttu-id="273dc-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="273dc-135">**Response**</span></span>

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
