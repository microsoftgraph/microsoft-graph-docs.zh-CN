---
title: 获取 identityRiskEvent
description: 检索的属性和 identityriskevent 对象的关系。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 6b66352010a3f1455dd2598215039c24a2dc819e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935596"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="2ed43-103">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2ed43-103">Get identityRiskEvent</span></span>

> <span data-ttu-id="2ed43-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2ed43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ed43-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2ed43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ed43-106">检索的属性和 identityriskevent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2ed43-106">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ed43-107">权限</span><span class="sxs-lookup"><span data-stu-id="2ed43-107">Permissions</span></span>
<span data-ttu-id="2ed43-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ed43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ed43-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ed43-110">Permission type</span></span>      | <span data-ttu-id="2ed43-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ed43-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ed43-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed43-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ed43-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ed43-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="2ed43-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ed43-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed43-115">Not supported.</span></span>    |
|<span data-ttu-id="2ed43-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ed43-116">Application</span></span> | <span data-ttu-id="2ed43-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ed43-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ed43-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ed43-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2ed43-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ed43-119">Request headers</span></span>
| <span data-ttu-id="2ed43-120">名称</span><span class="sxs-lookup"><span data-stu-id="2ed43-120">Name</span></span>      |<span data-ttu-id="2ed43-121">说明</span><span class="sxs-lookup"><span data-stu-id="2ed43-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ed43-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ed43-122">Authorization</span></span>  | <span data-ttu-id="2ed43-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ed43-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ed43-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ed43-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ed43-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2ed43-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ed43-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ed43-128">Request body</span></span>
<span data-ttu-id="2ed43-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ed43-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed43-130">响应</span><span class="sxs-lookup"><span data-stu-id="2ed43-130">Response</span></span>

<span data-ttu-id="2ed43-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[identityRiskEvent](../resources/identityriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2ed43-131">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ed43-132">示例</span><span class="sxs-lookup"><span data-stu-id="2ed43-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ed43-133">请求</span><span class="sxs-lookup"><span data-stu-id="2ed43-133">Request</span></span>
<span data-ttu-id="2ed43-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ed43-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="2ed43-135">响应</span><span class="sxs-lookup"><span data-stu-id="2ed43-135">Response</span></span>
<span data-ttu-id="2ed43-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ed43-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
