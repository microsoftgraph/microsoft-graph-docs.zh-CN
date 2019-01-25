---
title: 获取 impossibleTravelRiskEvent
description: 检索的属性和 impossibletravelriskevent 对象的关系。
localization_priority: Normal
ms.openlocfilehash: e5f1d7a47c261a9524225a1308531de8cd8de27c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520716"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="9791b-103">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9791b-103">Get impossibleTravelRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9791b-104">检索的属性和 impossibletravelriskevent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9791b-104">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9791b-105">权限</span><span class="sxs-lookup"><span data-stu-id="9791b-105">Permissions</span></span>
<span data-ttu-id="9791b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9791b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9791b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9791b-108">Permission type</span></span>      | <span data-ttu-id="9791b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9791b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9791b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9791b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9791b-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9791b-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="9791b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9791b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9791b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9791b-113">Not supported.</span></span>    |
|<span data-ttu-id="9791b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9791b-114">Application</span></span> | <span data-ttu-id="9791b-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9791b-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9791b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9791b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9791b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9791b-117">Request headers</span></span>
| <span data-ttu-id="9791b-118">名称</span><span class="sxs-lookup"><span data-stu-id="9791b-118">Name</span></span>      |<span data-ttu-id="9791b-119">说明</span><span class="sxs-lookup"><span data-stu-id="9791b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9791b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9791b-120">Authorization</span></span>  | <span data-ttu-id="9791b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9791b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9791b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9791b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9791b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9791b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9791b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9791b-126">Request body</span></span>
<span data-ttu-id="9791b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9791b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9791b-128">响应</span><span class="sxs-lookup"><span data-stu-id="9791b-128">Response</span></span>

<span data-ttu-id="9791b-129">如果成功，此方法返回`200 OK`响应正文中的响应代码和[impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9791b-129">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9791b-130">示例</span><span class="sxs-lookup"><span data-stu-id="9791b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9791b-131">请求</span><span class="sxs-lookup"><span data-stu-id="9791b-131">Request</span></span>
<span data-ttu-id="9791b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9791b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="9791b-133">响应</span><span class="sxs-lookup"><span data-stu-id="9791b-133">Response</span></span>
<span data-ttu-id="9791b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9791b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab",
  "ipAddress": "176.10.104.240",
  "isAtypicalLocation": true,
  "location": "Bern, CH",
  "previousIPAddress": "95.31.18.119",
  "previousLocation": "Moskva, Russia, RU",
  "previousSigninDateTime": "2016-01-29T00:00:55.3859274Z",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "ImpossibleTravelRiskEvent",
  "userAgent": "Firefox 42.0.0.1",
  "userDisplayName": "Jon Doe",
  "userId": "0bfdc7a8-6a16-c33e-7de9-a60a28ae533b",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get impossibleTravelRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/impossibletravelriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
