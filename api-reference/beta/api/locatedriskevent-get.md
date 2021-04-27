---
title: 获取 locatedRiskEvent
description: 检索 locatedriskevent 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-access
author: cloudhandler
ms.openlocfilehash: b0a62ba83d65dec634399bb7780f150aef92c5a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049301"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="1f4c9-103">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1f4c9-103">Get locatedRiskEvent</span></span>

<span data-ttu-id="1f4c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f4c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f4c9-105">检索 locatedriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-105">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f4c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="1f4c9-106">Permissions</span></span>
<span data-ttu-id="1f4c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f4c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f4c9-109">Permission type</span></span>      | <span data-ttu-id="1f4c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f4c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f4c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f4c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f4c9-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f4c9-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="1f4c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f4c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f4c9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-114">Not supported.</span></span>    |
|<span data-ttu-id="1f4c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f4c9-115">Application</span></span> | <span data-ttu-id="1f4c9-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f4c9-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f4c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f4c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1f4c9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f4c9-118">Request headers</span></span>
| <span data-ttu-id="1f4c9-119">名称</span><span class="sxs-lookup"><span data-stu-id="1f4c9-119">Name</span></span>      |<span data-ttu-id="1f4c9-120">说明</span><span class="sxs-lookup"><span data-stu-id="1f4c9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f4c9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f4c9-121">Authorization</span></span>  | <span data-ttu-id="1f4c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f4c9-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1f4c9-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f4c9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f4c9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f4c9-127">Request body</span></span>
<span data-ttu-id="1f4c9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f4c9-129">响应</span><span class="sxs-lookup"><span data-stu-id="1f4c9-129">Response</span></span>

<span data-ttu-id="1f4c9-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [locatedRiskEvent](../resources/locatedriskevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-130">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f4c9-131">示例</span><span class="sxs-lookup"><span data-stu-id="1f4c9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f4c9-132">请求</span><span class="sxs-lookup"><span data-stu-id="1f4c9-132">Request</span></span>
<span data-ttu-id="1f4c9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="1f4c9-134">响应</span><span class="sxs-lookup"><span data-stu-id="1f4c9-134">Response</span></span>
<span data-ttu-id="1f4c9-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-135">Here is an example of the response.</span></span> <span data-ttu-id="1f4c9-136">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1f4c9-136">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.locatedRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "a6653179-3c7b-4e99-bb4c-dddeb18adfc1",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get locatedRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


