---
title: 获取 identityRiskEvent
description: 检索的属性和 identityriskevent 对象的关系。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 54bb5a43971fd4108178a7cace6821e4369ec6a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510727"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="2b311-103">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2b311-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b311-104">检索的属性和 identityriskevent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2b311-104">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b311-105">权限</span><span class="sxs-lookup"><span data-stu-id="2b311-105">Permissions</span></span>
<span data-ttu-id="2b311-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b311-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b311-108">Permission type</span></span>      | <span data-ttu-id="2b311-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b311-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b311-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b311-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b311-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b311-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="2b311-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b311-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b311-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b311-113">Not supported.</span></span>    |
|<span data-ttu-id="2b311-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b311-114">Application</span></span> | <span data-ttu-id="2b311-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b311-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b311-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b311-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2b311-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b311-117">Request headers</span></span>
| <span data-ttu-id="2b311-118">名称</span><span class="sxs-lookup"><span data-stu-id="2b311-118">Name</span></span>      |<span data-ttu-id="2b311-119">说明</span><span class="sxs-lookup"><span data-stu-id="2b311-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b311-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b311-120">Authorization</span></span>  | <span data-ttu-id="2b311-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b311-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b311-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2b311-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b311-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2b311-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b311-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b311-126">Request body</span></span>
<span data-ttu-id="2b311-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b311-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b311-128">响应</span><span class="sxs-lookup"><span data-stu-id="2b311-128">Response</span></span>

<span data-ttu-id="2b311-129">如果成功，此方法返回`200 OK`响应正文中的响应代码和[identityRiskEvent](../resources/identityriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b311-129">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b311-130">示例</span><span class="sxs-lookup"><span data-stu-id="2b311-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b311-131">请求</span><span class="sxs-lookup"><span data-stu-id="2b311-131">Request</span></span>
<span data-ttu-id="2b311-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b311-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="2b311-133">响应</span><span class="sxs-lookup"><span data-stu-id="2b311-133">Response</span></span>
<span data-ttu-id="2b311-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b311-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
