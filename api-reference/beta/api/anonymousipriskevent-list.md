---
title: 列表 anonymousIpRiskEvents
description: 检索 anonymousipriskevent 对象的列表。
ms.openlocfilehash: aa5845d37f36dd59727083650c1737ecedc46187
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042413"
---
# <a name="list-anonymousipriskevents"></a><span data-ttu-id="50ecc-103">列表 anonymousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="50ecc-103">List anonymousIpRiskEvents</span></span>

> <span data-ttu-id="50ecc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="50ecc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50ecc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="50ecc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50ecc-106">检索 anonymousipriskevent 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="50ecc-106">Retrieve a list of anonymousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="50ecc-107">权限</span><span class="sxs-lookup"><span data-stu-id="50ecc-107">Permissions</span></span>
<span data-ttu-id="50ecc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50ecc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ecc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="50ecc-110">Permission type</span></span>      | <span data-ttu-id="50ecc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50ecc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50ecc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50ecc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50ecc-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="50ecc-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="50ecc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50ecc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50ecc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="50ecc-115">Not supported.</span></span>    |
|<span data-ttu-id="50ecc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="50ecc-116">Application</span></span> | <span data-ttu-id="50ecc-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="50ecc-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50ecc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50ecc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents
```

## <a name="request-headers"></a><span data-ttu-id="50ecc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50ecc-119">Request headers</span></span>
| <span data-ttu-id="50ecc-120">名称</span><span class="sxs-lookup"><span data-stu-id="50ecc-120">Name</span></span>      |<span data-ttu-id="50ecc-121">说明</span><span class="sxs-lookup"><span data-stu-id="50ecc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50ecc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50ecc-122">Authorization</span></span>  | <span data-ttu-id="50ecc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50ecc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50ecc-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="50ecc-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="50ecc-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="50ecc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50ecc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="50ecc-128">Request body</span></span>
<span data-ttu-id="50ecc-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50ecc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50ecc-130">响应</span><span class="sxs-lookup"><span data-stu-id="50ecc-130">Response</span></span>

<span data-ttu-id="50ecc-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="50ecc-131">If successful, this method returns a `200 OK` response code and collection of [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50ecc-132">示例</span><span class="sxs-lookup"><span data-stu-id="50ecc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50ecc-133">请求</span><span class="sxs-lookup"><span data-stu-id="50ecc-133">Request</span></span>
<span data-ttu-id="50ecc-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50ecc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="50ecc-135">响应</span><span class="sxs-lookup"><span data-stu-id="50ecc-135">Response</span></span>
<span data-ttu-id="50ecc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50ecc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List anonymousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
