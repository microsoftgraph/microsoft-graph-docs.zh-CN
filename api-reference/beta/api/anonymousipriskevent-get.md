---
title: 获取 anonymousIpRiskEvent
description: 检索的属性和 anonymousipriskevent 对象的关系。
localization_priority: Normal
ms.openlocfilehash: a4a1483dd3b4bc984a418f1ff03083bf2977b5a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859925"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="36ff6-103">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="36ff6-103">Get anonymousIpRiskEvent</span></span>

> <span data-ttu-id="36ff6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="36ff6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36ff6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36ff6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36ff6-106">检索的属性和 anonymousipriskevent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="36ff6-106">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36ff6-107">权限</span><span class="sxs-lookup"><span data-stu-id="36ff6-107">Permissions</span></span>
<span data-ttu-id="36ff6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36ff6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36ff6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36ff6-110">Permission type</span></span>      | <span data-ttu-id="36ff6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36ff6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36ff6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36ff6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="36ff6-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="36ff6-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="36ff6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36ff6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36ff6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36ff6-115">Not supported.</span></span>    |
|<span data-ttu-id="36ff6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36ff6-116">Application</span></span> | <span data-ttu-id="36ff6-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="36ff6-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36ff6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36ff6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="36ff6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="36ff6-119">Request headers</span></span>
| <span data-ttu-id="36ff6-120">名称</span><span class="sxs-lookup"><span data-stu-id="36ff6-120">Name</span></span>      |<span data-ttu-id="36ff6-121">说明</span><span class="sxs-lookup"><span data-stu-id="36ff6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36ff6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36ff6-122">Authorization</span></span>  | <span data-ttu-id="36ff6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36ff6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36ff6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36ff6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="36ff6-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="36ff6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36ff6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="36ff6-128">Request body</span></span>
<span data-ttu-id="36ff6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36ff6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36ff6-130">响应</span><span class="sxs-lookup"><span data-stu-id="36ff6-130">Response</span></span>

<span data-ttu-id="36ff6-131">如果成功，此方法返回`200 OK`的响应正文值中的响应代码和[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36ff6-131">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="36ff6-132">示例</span><span class="sxs-lookup"><span data-stu-id="36ff6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36ff6-133">请求</span><span class="sxs-lookup"><span data-stu-id="36ff6-133">Request</span></span>
<span data-ttu-id="36ff6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36ff6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="36ff6-135">响应</span><span class="sxs-lookup"><span data-stu-id="36ff6-135">Response</span></span>
<span data-ttu-id="36ff6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36ff6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "ipAddress": null,
  "location": null,
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "AnonymousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get anonymousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
