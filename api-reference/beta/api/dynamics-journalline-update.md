---
title: 更新 journalLines
description: 更新 Dynamics 365 Business Central 中的日记行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 58932fcc23eb78c2715b79e57f100508f50b66a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428759"
---
# <a name="update-journallines"></a><span data-ttu-id="5b7d3-103">更新 journalLines</span><span class="sxs-lookup"><span data-stu-id="5b7d3-103">Update journalLines</span></span>

<span data-ttu-id="5b7d3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5b7d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b7d3-105">更新 Dynamics 365 Business Central 的日记行对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-105">Update the properties of a journal lines object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b7d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="5b7d3-106">Permissions</span></span>
<span data-ttu-id="5b7d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b7d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b7d3-109">Permission type</span></span> |<span data-ttu-id="5b7d3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b7d3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5b7d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b7d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b7d3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b7d3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5b7d3-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5b7d3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5b7d3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-114">Not supported.</span></span>|
|<span data-ttu-id="5b7d3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b7d3-115">Application</span></span>|<span data-ttu-id="5b7d3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b7d3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b7d3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b7d3-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b7d3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5b7d3-118">Optional query parameters</span></span>
<span data-ttu-id="5b7d3-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b7d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b7d3-120">Request headers</span></span>
| <span data-ttu-id="5b7d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="5b7d3-121">Header</span></span>       | <span data-ttu-id="5b7d3-122">值</span><span class="sxs-lookup"><span data-stu-id="5b7d3-122">Value</span></span>                    |
|--------------|--------------------------|
|<span data-ttu-id="5b7d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b7d3-123">Authorization</span></span> |<span data-ttu-id="5b7d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="5b7d3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b7d3-126">Content-Type</span></span>  |<span data-ttu-id="5b7d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5b7d3-127">application/json</span></span>          |
|<span data-ttu-id="5b7d3-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="5b7d3-128">If-Match</span></span>      |<span data-ttu-id="5b7d3-129">必填。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-129">Required.</span></span> <span data-ttu-id="5b7d3-130">如果包含此请求标头，且提供的 eTag 与**journalLines**上的当前标记不匹配，则不会更新**journalLines** 。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-130">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b7d3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b7d3-131">Request body</span></span>
<span data-ttu-id="5b7d3-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="5b7d3-135">响应</span><span class="sxs-lookup"><span data-stu-id="5b7d3-135">Response</span></span>
<span data-ttu-id="5b7d3-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的**journalLines**对象。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-136">If successful, this method returns a `200 OK` response code and an updated **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b7d3-137">示例</span><span class="sxs-lookup"><span data-stu-id="5b7d3-137">Example</span></span>

<span data-ttu-id="5b7d3-138">**请求**</span><span class="sxs-lookup"><span data-stu-id="5b7d3-138">**Request**</span></span>

<span data-ttu-id="5b7d3-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b7d3-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines/{id}
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="5b7d3-140">**响应**</span><span class="sxs-lookup"><span data-stu-id="5b7d3-140">**Response**</span></span>

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


