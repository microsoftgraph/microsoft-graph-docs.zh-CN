---
title: 更新 journalLines
description: 更新 Dynamics 365 Business Central 中的日记行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 9b7a60418d1a322b3d2997c1889f7280acd7810d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791419"
---
# <a name="update-journallines"></a><span data-ttu-id="107c6-103">更新 journalLines</span><span class="sxs-lookup"><span data-stu-id="107c6-103">Update journalLines</span></span>
<span data-ttu-id="107c6-104">更新 Dynamics 365 Business Central 的日记行对象的属性。</span><span class="sxs-lookup"><span data-stu-id="107c6-104">Update the properties of a journal lines object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="107c6-105">权限</span><span class="sxs-lookup"><span data-stu-id="107c6-105">Permissions</span></span>
<span data-ttu-id="107c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="107c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="107c6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="107c6-108">Permission type</span></span> |<span data-ttu-id="107c6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="107c6-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="107c6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="107c6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="107c6-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="107c6-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="107c6-112">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="107c6-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="107c6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="107c6-113">Not supported.</span></span>|
|<span data-ttu-id="107c6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="107c6-114">Application</span></span>|<span data-ttu-id="107c6-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="107c6-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="107c6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="107c6-116">HTTP request</span></span>

```
PATCH /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="107c6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="107c6-117">Optional query parameters</span></span>
<span data-ttu-id="107c6-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="107c6-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="107c6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="107c6-119">Request headers</span></span>
| <span data-ttu-id="107c6-120">标头</span><span class="sxs-lookup"><span data-stu-id="107c6-120">Header</span></span>       | <span data-ttu-id="107c6-121">值</span><span class="sxs-lookup"><span data-stu-id="107c6-121">Value</span></span>                    |
|--------------|--------------------------|
|<span data-ttu-id="107c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="107c6-122">Authorization</span></span> |<span data-ttu-id="107c6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="107c6-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="107c6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="107c6-125">Content-Type</span></span>  |<span data-ttu-id="107c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="107c6-126">application/json</span></span>          |
|<span data-ttu-id="107c6-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="107c6-127">If-Match</span></span>      |<span data-ttu-id="107c6-128">必需。</span><span class="sxs-lookup"><span data-stu-id="107c6-128">Required.</span></span> <span data-ttu-id="107c6-129">如果包含此请求标头，且提供的 eTag 与**journalLines**上的当前标记不匹配，则不会更新**journalLines** 。</span><span class="sxs-lookup"><span data-stu-id="107c6-129">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="107c6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="107c6-130">Request body</span></span>
<span data-ttu-id="107c6-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="107c6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="107c6-134">响应</span><span class="sxs-lookup"><span data-stu-id="107c6-134">Response</span></span>
<span data-ttu-id="107c6-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的**journalLines**对象。</span><span class="sxs-lookup"><span data-stu-id="107c6-135">If successful, this method returns a `200 OK` response code and an updated **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="107c6-136">示例</span><span class="sxs-lookup"><span data-stu-id="107c6-136">Example</span></span>

<span data-ttu-id="107c6-137">**请求**</span><span class="sxs-lookup"><span data-stu-id="107c6-137">**Request**</span></span>

<span data-ttu-id="107c6-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="107c6-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines/{id}
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="107c6-139">**响应**</span><span class="sxs-lookup"><span data-stu-id="107c6-139">**Response**</span></span>

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


