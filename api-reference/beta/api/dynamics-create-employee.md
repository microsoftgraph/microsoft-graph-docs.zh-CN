---
title: 创建员工
description: 在 Dynamics 365 Business Central 中创建员工对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 79d6f242a7811570e9f4488f2f150205940a6eec
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473299"
---
# <a name="create-employees"></a><span data-ttu-id="e3dd2-103">创建员工</span><span class="sxs-lookup"><span data-stu-id="e3dd2-103">Create employees</span></span>

<span data-ttu-id="e3dd2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3dd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3dd2-105">在 Dynamics 365 Business Central 中创建员工对象。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-105">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3dd2-106">权限</span><span class="sxs-lookup"><span data-stu-id="e3dd2-106">Permissions</span></span>
<span data-ttu-id="e3dd2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3dd2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3dd2-109">Permission type</span></span> |<span data-ttu-id="e3dd2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3dd2-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e3dd2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3dd2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3dd2-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3dd2-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e3dd2-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e3dd2-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e3dd2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-114">Not supported.</span></span>|
|<span data-ttu-id="e3dd2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3dd2-115">Application</span></span>|<span data-ttu-id="e3dd2-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3dd2-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3dd2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3dd2-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3dd2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e3dd2-118">Optional query parameters</span></span>
<span data-ttu-id="e3dd2-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3dd2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3dd2-120">Request headers</span></span>
|<span data-ttu-id="e3dd2-121">标头</span><span class="sxs-lookup"><span data-stu-id="e3dd2-121">Header</span></span>        |<span data-ttu-id="e3dd2-122">值</span><span class="sxs-lookup"><span data-stu-id="e3dd2-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="e3dd2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3dd2-123">Authorization</span></span> |<span data-ttu-id="e3dd2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e3dd2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3dd2-126">Content-Type</span></span>  |<span data-ttu-id="e3dd2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e3dd2-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="e3dd2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3dd2-128">Request body</span></span>
<span data-ttu-id="e3dd2-129">在请求正文中，提供 employees 对象的 JSON **表示形式** 。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-129">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="e3dd2-130">响应</span><span class="sxs-lookup"><span data-stu-id="e3dd2-130">Response</span></span>
<span data-ttu-id="e3dd2-131">如果成功，此方法在 ```201 Created``` 响应正文中返回响应代码和 employees 对象。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-131">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3dd2-132">示例</span><span class="sxs-lookup"><span data-stu-id="e3dd2-132">Example</span></span>

<span data-ttu-id="e3dd2-133">**请求**</span><span class="sxs-lookup"><span data-stu-id="e3dd2-133">**Request**</span></span>

<span data-ttu-id="e3dd2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/employees
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "givenName": "Annette",
  "surname": "Hill",
  "jobTitle": "Production Assistant",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "birthDate": "1973-12-12"  
}

```

<span data-ttu-id="e3dd2-135">**响应**</span><span class="sxs-lookup"><span data-stu-id="e3dd2-135">**Response**</span></span>

<span data-ttu-id="e3dd2-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="e3dd2-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e3dd2-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e3dd2-138">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "displayName": "Annette Hill",
  "givenName": "Annette",
  "middleName": "",
  "surname": "Hill",
  "jobTitle": "Secretary",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "email": "",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "terminationDate": "0001-01-01",
  "status": "Active",
  "birthDate": "1973-12-12",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/employees/{id}/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z" 
}

```



