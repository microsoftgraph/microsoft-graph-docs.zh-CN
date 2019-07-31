---
title: 创建 taxAreas
description: 在 Dynamics 中创建金融的税务区域对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e2e8138a89f25abafe0a5333136d5aef45014f10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956567"
---
# <a name="create-taxareas"></a><span data-ttu-id="6ceea-103">创建 taxAreas</span><span class="sxs-lookup"><span data-stu-id="6ceea-103">Create taxAreas</span></span>
<span data-ttu-id="6ceea-104">在 Dynamics 365 Business Central 中创建税务区域对象。</span><span class="sxs-lookup"><span data-stu-id="6ceea-104">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ceea-105">权限</span><span class="sxs-lookup"><span data-stu-id="6ceea-105">Permissions</span></span>
<span data-ttu-id="6ceea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ceea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ceea-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ceea-108">Permission type</span></span> |<span data-ttu-id="6ceea-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ceea-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6ceea-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ceea-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6ceea-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ceea-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6ceea-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="6ceea-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6ceea-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ceea-113">Not supported.</span></span>|
|<span data-ttu-id="6ceea-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ceea-114">Application</span></span>|<span data-ttu-id="6ceea-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ceea-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ceea-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ceea-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ceea-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6ceea-117">Optional query parameters</span></span>
<span data-ttu-id="6ceea-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6ceea-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ceea-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ceea-119">Request headers</span></span>
|<span data-ttu-id="6ceea-120">标头</span><span class="sxs-lookup"><span data-stu-id="6ceea-120">Header</span></span>|<span data-ttu-id="6ceea-121">值</span><span class="sxs-lookup"><span data-stu-id="6ceea-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="6ceea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ceea-122">Authorization</span></span>  |<span data-ttu-id="6ceea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ceea-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="6ceea-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ceea-125">Content-Type</span></span>  |<span data-ttu-id="6ceea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ceea-126">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="6ceea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ceea-127">Request body</span></span>
<span data-ttu-id="6ceea-128">在请求正文中, 提供**taxAreas**对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ceea-128">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="6ceea-129">响应</span><span class="sxs-lookup"><span data-stu-id="6ceea-129">Response</span></span>
<span data-ttu-id="6ceea-130">如果成功, 此方法在```201 Created```响应正文中返回响应代码和**taxAreas**对象。</span><span class="sxs-lookup"><span data-stu-id="6ceea-130">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ceea-131">示例</span><span class="sxs-lookup"><span data-stu-id="6ceea-131">Example</span></span>

<span data-ttu-id="6ceea-132">**请求**</span><span class="sxs-lookup"><span data-stu-id="6ceea-132">**Request**</span></span>

<span data-ttu-id="6ceea-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ceea-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas
Content-type: application/json

```json
{
  "code": "44442001T"
}
```

<span data-ttu-id="6ceea-134">**响应**</span><span class="sxs-lookup"><span data-stu-id="6ceea-134">**Response**</span></span>

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
