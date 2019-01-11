---
title: 获取 unfamiliarLocationRiskEvent
description: 检索的属性和 unfamiliarlocationriskevent 对象的关系。
localization_priority: Normal
ms.openlocfilehash: d58fc2c5b2c84ae0b43bbc2b83345d6bc6bff700
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827932"
---
# <a name="get-unfamiliarlocationriskevent"></a><span data-ttu-id="a5155-103">获取 unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a5155-103">Get unfamiliarLocationRiskEvent</span></span>

> <span data-ttu-id="a5155-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5155-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5155-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5155-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5155-106">检索的属性和 unfamiliarlocationriskevent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a5155-106">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5155-107">权限</span><span class="sxs-lookup"><span data-stu-id="a5155-107">Permissions</span></span>
<span data-ttu-id="a5155-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5155-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5155-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5155-110">Permission type</span></span>      | <span data-ttu-id="a5155-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5155-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5155-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5155-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5155-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5155-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="a5155-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5155-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5155-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5155-115">Not supported.</span></span>    |
|<span data-ttu-id="a5155-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5155-116">Application</span></span> | <span data-ttu-id="a5155-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5155-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5155-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5155-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a5155-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5155-119">Request headers</span></span>
| <span data-ttu-id="a5155-120">名称</span><span class="sxs-lookup"><span data-stu-id="a5155-120">Name</span></span>      |<span data-ttu-id="a5155-121">说明</span><span class="sxs-lookup"><span data-stu-id="a5155-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5155-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5155-122">Authorization</span></span>  | <span data-ttu-id="a5155-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5155-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5155-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a5155-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a5155-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a5155-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5155-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5155-128">Request body</span></span>
<span data-ttu-id="a5155-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5155-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5155-130">响应</span><span class="sxs-lookup"><span data-stu-id="a5155-130">Response</span></span>

<span data-ttu-id="a5155-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a5155-131">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5155-132">示例</span><span class="sxs-lookup"><span data-stu-id="a5155-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5155-133">请求</span><span class="sxs-lookup"><span data-stu-id="a5155-133">Request</span></span>
<span data-ttu-id="a5155-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5155-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="a5155-135">响应</span><span class="sxs-lookup"><span data-stu-id="a5155-135">Response</span></span>
<span data-ttu-id="a5155-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a5155-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
