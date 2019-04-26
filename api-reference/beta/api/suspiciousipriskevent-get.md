---
title: 获取 suspiciousIpRiskEvent
description: 检索 suspiciousipriskevent 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 8e3e069f18553575a5d69a5fb17c2c289f44fe82
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335731"
---
# <a name="get-suspiciousipriskevent"></a><span data-ttu-id="a0836-103">获取 suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a0836-103">Get suspiciousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0836-104">检索 suspiciousipriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0836-104">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0836-105">权限</span><span class="sxs-lookup"><span data-stu-id="a0836-105">Permissions</span></span>
<span data-ttu-id="a0836-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0836-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0836-108">Permission type</span></span>      | <span data-ttu-id="a0836-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0836-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0836-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0836-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0836-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0836-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="a0836-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0836-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0836-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0836-113">Not supported.</span></span>    |
|<span data-ttu-id="a0836-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0836-114">Application</span></span> | <span data-ttu-id="a0836-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0836-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0836-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0836-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a0836-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0836-117">Request headers</span></span>
| <span data-ttu-id="a0836-118">名称</span><span class="sxs-lookup"><span data-stu-id="a0836-118">Name</span></span>      |<span data-ttu-id="a0836-119">说明</span><span class="sxs-lookup"><span data-stu-id="a0836-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0836-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0836-120">Authorization</span></span>  | <span data-ttu-id="a0836-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0836-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0836-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a0836-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a0836-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a0836-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0836-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0836-126">Request body</span></span>
<span data-ttu-id="a0836-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0836-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0836-128">响应</span><span class="sxs-lookup"><span data-stu-id="a0836-128">Response</span></span>

<span data-ttu-id="a0836-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0836-129">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0836-130">示例</span><span class="sxs-lookup"><span data-stu-id="a0836-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0836-131">请求</span><span class="sxs-lookup"><span data-stu-id="a0836-131">Request</span></span>
<span data-ttu-id="a0836-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0836-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="a0836-133">响应</span><span class="sxs-lookup"><span data-stu-id="a0836-133">Response</span></span>
<span data-ttu-id="a0836-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0836-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": null,
  "createdDateTime": "2016-02-03T06:08:35.123512Z",
  "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
  "ipAddress": "95.31.18.119",
  "location": "Moskva, Russia, RU",
  "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
  "riskEventStatus": "active",
  "riskLevel": "low",
  "riskType": "SuspiciousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get suspiciousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
