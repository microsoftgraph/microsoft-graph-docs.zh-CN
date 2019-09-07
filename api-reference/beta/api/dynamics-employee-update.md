---
title: 更新员工
description: 更新 Dynamics 365 Business Central 中的 employee 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ac17678b5cc75d8416918b6f39583d27f9d5dea7
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791657"
---
# <a name="update-employees"></a><span data-ttu-id="c8e01-103">更新员工</span><span class="sxs-lookup"><span data-stu-id="c8e01-103">Update employees</span></span>
<span data-ttu-id="c8e01-104">为 Dynamics 365 Business Central 更新 employee 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8e01-104">Update the properties of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e01-105">权限</span><span class="sxs-lookup"><span data-stu-id="c8e01-105">Permissions</span></span>
<span data-ttu-id="c8e01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e01-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8e01-108">Permission type</span></span> |<span data-ttu-id="c8e01-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8e01-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c8e01-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8e01-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c8e01-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e01-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c8e01-112">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="c8e01-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c8e01-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8e01-113">Not supported.</span></span>|
|<span data-ttu-id="c8e01-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8e01-114">Application</span></span>|<span data-ttu-id="c8e01-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e01-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8e01-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8e01-116">HTTP request</span></span>

```
PATCH /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8e01-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c8e01-117">Optional query parameters</span></span>
<span data-ttu-id="c8e01-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c8e01-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8e01-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8e01-119">Request headers</span></span>
|<span data-ttu-id="c8e01-120">标头</span><span class="sxs-lookup"><span data-stu-id="c8e01-120">Header</span></span>         |<span data-ttu-id="c8e01-121">值</span><span class="sxs-lookup"><span data-stu-id="c8e01-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="c8e01-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8e01-122">Authorization</span></span>  |<span data-ttu-id="c8e01-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8e01-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c8e01-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8e01-125">Content-Type</span></span>   |<span data-ttu-id="c8e01-126">application/json.</span><span class="sxs-lookup"><span data-stu-id="c8e01-126">application/json.</span></span>         |
|<span data-ttu-id="c8e01-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="c8e01-127">If-Match</span></span>       |<span data-ttu-id="c8e01-128">必需。</span><span class="sxs-lookup"><span data-stu-id="c8e01-128">Required.</span></span> <span data-ttu-id="c8e01-129">如果包含此请求标头，且提供的 eTag 与**员工**的当前标记不匹配，则不会更新**员工**。</span><span class="sxs-lookup"><span data-stu-id="c8e01-129">When this request header is included and the eTag provided does not match the current tag on the **employees**, the **employees** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8e01-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8e01-130">Request body</span></span>
<span data-ttu-id="c8e01-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c8e01-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="c8e01-134">响应</span><span class="sxs-lookup"><span data-stu-id="c8e01-134">Response</span></span>
<span data-ttu-id="c8e01-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的**employees**对象。</span><span class="sxs-lookup"><span data-stu-id="c8e01-135">If successful, this method returns a `200 OK` response code and an updated **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8e01-136">示例</span><span class="sxs-lookup"><span data-stu-id="c8e01-136">Example</span></span>

<span data-ttu-id="c8e01-137">**请求**</span><span class="sxs-lookup"><span data-stu-id="c8e01-137">**Request**</span></span>

<span data-ttu-id="c8e01-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8e01-138">Here is an example of the request.</span></span>

```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
Content-type: application/json

{
  "givenName": "Anthony",
  "phoneNumber": "0678-8712-3455"
}
```

<span data-ttu-id="c8e01-139">**响应**</span><span class="sxs-lookup"><span data-stu-id="c8e01-139">**Response**</span></span>

<span data-ttu-id="c8e01-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c8e01-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="c8e01-141">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c8e01-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c8e01-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c8e01-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "displayName": "Anthony Hill",
  "givenName": "Anthony",
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
  "phoneNumber": "0678-8712-3455",
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
  
