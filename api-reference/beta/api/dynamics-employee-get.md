---
title: 获取员工
description: 获取 Dynamics 365 Business Central 中的 employee 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8ad066ad4eee33f8a5e73612fd401e030641d820
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42429991"
---
# <a name="get-employees"></a><span data-ttu-id="ead7d-103">获取员工</span><span class="sxs-lookup"><span data-stu-id="ead7d-103">Get employees</span></span>

<span data-ttu-id="ead7d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ead7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ead7d-105">检索 Dynamics 365 Business Central 的 employee 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ead7d-105">Retrieve the properties and relationships of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ead7d-106">权限</span><span class="sxs-lookup"><span data-stu-id="ead7d-106">Permissions</span></span>
<span data-ttu-id="ead7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ead7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ead7d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ead7d-109">Permission type</span></span> |<span data-ttu-id="ead7d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ead7d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ead7d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ead7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ead7d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ead7d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ead7d-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ead7d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ead7d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ead7d-114">Not supported.</span></span>|
|<span data-ttu-id="ead7d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ead7d-115">Application</span></span>|<span data-ttu-id="ead7d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ead7d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ead7d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ead7d-117">HTTP request</span></span>
```
GET /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ead7d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ead7d-118">Optional query parameters</span></span>
<span data-ttu-id="ead7d-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ead7d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ead7d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ead7d-120">Request headers</span></span>
|<span data-ttu-id="ead7d-121">标头</span><span class="sxs-lookup"><span data-stu-id="ead7d-121">Header</span></span>       |<span data-ttu-id="ead7d-122">值</span><span class="sxs-lookup"><span data-stu-id="ead7d-122">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="ead7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ead7d-123">Authorization</span></span>|<span data-ttu-id="ead7d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ead7d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ead7d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ead7d-126">Request body</span></span>
<span data-ttu-id="ead7d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ead7d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ead7d-128">响应</span><span class="sxs-lookup"><span data-stu-id="ead7d-128">Response</span></span>
<span data-ttu-id="ead7d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和**employees**对象。</span><span class="sxs-lookup"><span data-stu-id="ead7d-129">If successful, this method returns a `200 OK` response code and an **employees** object in the response body.</span></span>

<span data-ttu-id="ead7d-130">**请求**</span><span class="sxs-lookup"><span data-stu-id="ead7d-130">**Request**</span></span>

<span data-ttu-id="ead7d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ead7d-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
```

<span data-ttu-id="ead7d-132">**响应**</span><span class="sxs-lookup"><span data-stu-id="ead7d-132">**Response**</span></span>

<span data-ttu-id="ead7d-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ead7d-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="ead7d-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ead7d-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ead7d-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ead7d-135">All the properties will be returned from an actual call.</span></span>

```json
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


