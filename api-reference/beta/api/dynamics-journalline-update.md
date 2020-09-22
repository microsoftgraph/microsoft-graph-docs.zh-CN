---
title: 更新 journalLines
description: 更新 Dynamics 365 Business Central 中的日记行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7f011b816fbd5c217a41faed82d836947ef1e817
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008222"
---
# <a name="update-journallines"></a><span data-ttu-id="ea156-103">更新 journalLines</span><span class="sxs-lookup"><span data-stu-id="ea156-103">Update journalLines</span></span>

<span data-ttu-id="ea156-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea156-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea156-105">更新 Dynamics 365 Business Central 的日记行对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ea156-105">Update the properties of a journal lines object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea156-106">权限</span><span class="sxs-lookup"><span data-stu-id="ea156-106">Permissions</span></span>
<span data-ttu-id="ea156-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea156-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea156-109">Permission type</span></span> |<span data-ttu-id="ea156-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea156-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ea156-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea156-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea156-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea156-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ea156-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ea156-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ea156-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea156-114">Not supported.</span></span>|
|<span data-ttu-id="ea156-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea156-115">Application</span></span>|<span data-ttu-id="ea156-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea156-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea156-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea156-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea156-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ea156-118">Optional query parameters</span></span>
<span data-ttu-id="ea156-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ea156-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea156-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea156-120">Request headers</span></span>
| <span data-ttu-id="ea156-121">标头</span><span class="sxs-lookup"><span data-stu-id="ea156-121">Header</span></span>       | <span data-ttu-id="ea156-122">值</span><span class="sxs-lookup"><span data-stu-id="ea156-122">Value</span></span>                    |
|--------------|--------------------------|
|<span data-ttu-id="ea156-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea156-123">Authorization</span></span> |<span data-ttu-id="ea156-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea156-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="ea156-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea156-126">Content-Type</span></span>  |<span data-ttu-id="ea156-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ea156-127">application/json</span></span>          |
|<span data-ttu-id="ea156-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="ea156-128">If-Match</span></span>      |<span data-ttu-id="ea156-129">必需。</span><span class="sxs-lookup"><span data-stu-id="ea156-129">Required.</span></span> <span data-ttu-id="ea156-130">如果包含此请求标头，且提供的 eTag 与 **journalLines**上的当前标记不匹配，则不会更新 **journalLines** 。</span><span class="sxs-lookup"><span data-stu-id="ea156-130">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea156-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea156-131">Request body</span></span>
<span data-ttu-id="ea156-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ea156-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="ea156-135">响应</span><span class="sxs-lookup"><span data-stu-id="ea156-135">Response</span></span>
<span data-ttu-id="ea156-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 **journalLines** 对象。</span><span class="sxs-lookup"><span data-stu-id="ea156-136">If successful, this method returns a `200 OK` response code and an updated **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea156-137">示例</span><span class="sxs-lookup"><span data-stu-id="ea156-137">Example</span></span>

<span data-ttu-id="ea156-138">**请求**</span><span class="sxs-lookup"><span data-stu-id="ea156-138">**Request**</span></span>

<span data-ttu-id="ea156-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea156-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines/{id}
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="ea156-140">**响应**</span><span class="sxs-lookup"><span data-stu-id="ea156-140">**Response**</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "",
  "accountNumber": "",
  "postingDate": "2015-12-31",
  "documentNumber": "D00001",
  "externalDocumentNumber": "",
  "amount": 2000,
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```




