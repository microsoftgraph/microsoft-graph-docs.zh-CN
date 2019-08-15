---
title: 获取 identityRiskEvent
description: 检索 identityriskevent 对象的属性和关系。
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0df9e818a880516980f034449ceb140f244cc255
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419533"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="27666-103">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="27666-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27666-104">检索 identityriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27666-104">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="27666-105">权限</span><span class="sxs-lookup"><span data-stu-id="27666-105">Permissions</span></span>
<span data-ttu-id="27666-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27666-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="27666-108">Permission type</span></span>      | <span data-ttu-id="27666-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27666-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27666-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27666-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27666-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="27666-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="27666-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27666-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27666-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="27666-113">Not supported.</span></span>    |
|<span data-ttu-id="27666-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="27666-114">Application</span></span> | <span data-ttu-id="27666-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="27666-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27666-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27666-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="27666-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="27666-117">Request headers</span></span>
| <span data-ttu-id="27666-118">名称</span><span class="sxs-lookup"><span data-stu-id="27666-118">Name</span></span>      |<span data-ttu-id="27666-119">说明</span><span class="sxs-lookup"><span data-stu-id="27666-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27666-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="27666-120">Authorization</span></span>  | <span data-ttu-id="27666-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27666-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27666-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="27666-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="27666-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="27666-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27666-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="27666-126">Request body</span></span>
<span data-ttu-id="27666-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="27666-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27666-128">响应</span><span class="sxs-lookup"><span data-stu-id="27666-128">Response</span></span>

<span data-ttu-id="27666-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[identityRiskEvent](../resources/identityriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27666-129">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27666-130">示例</span><span class="sxs-lookup"><span data-stu-id="27666-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27666-131">请求</span><span class="sxs-lookup"><span data-stu-id="27666-131">Request</span></span>
<span data-ttu-id="27666-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27666-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27666-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="27666-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27666-134">C#</span><span class="sxs-lookup"><span data-stu-id="27666-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27666-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27666-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27666-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="27666-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27666-137">响应</span><span class="sxs-lookup"><span data-stu-id="27666-137">Response</span></span>
<span data-ttu-id="27666-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27666-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
