---
title: 获取 anonymousIpRiskEvent
description: 检索 anonymousipriskevent 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: c306593d55792035377d18ad1888f5a4ca707aa6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459519"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="ec8b0-103">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ec8b0-103">Get anonymousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec8b0-104">检索 anonymousipriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-104">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec8b0-105">权限</span><span class="sxs-lookup"><span data-stu-id="ec8b0-105">Permissions</span></span>
<span data-ttu-id="ec8b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec8b0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec8b0-108">Permission type</span></span>      | <span data-ttu-id="ec8b0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec8b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec8b0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec8b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec8b0-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec8b0-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="ec8b0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec8b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec8b0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-113">Not supported.</span></span>    |
|<span data-ttu-id="ec8b0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec8b0-114">Application</span></span> | <span data-ttu-id="ec8b0-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec8b0-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec8b0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec8b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ec8b0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec8b0-117">Request headers</span></span>
| <span data-ttu-id="ec8b0-118">名称</span><span class="sxs-lookup"><span data-stu-id="ec8b0-118">Name</span></span>      |<span data-ttu-id="ec8b0-119">说明</span><span class="sxs-lookup"><span data-stu-id="ec8b0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec8b0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec8b0-120">Authorization</span></span>  | <span data-ttu-id="ec8b0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec8b0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec8b0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec8b0-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec8b0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec8b0-126">Request body</span></span>
<span data-ttu-id="ec8b0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec8b0-128">响应</span><span class="sxs-lookup"><span data-stu-id="ec8b0-128">Response</span></span>

<span data-ttu-id="ec8b0-129">如果成功, 此方法在响应`200 OK`正文的值中返回响应代码和[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-129">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec8b0-130">示例</span><span class="sxs-lookup"><span data-stu-id="ec8b0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec8b0-131">请求</span><span class="sxs-lookup"><span data-stu-id="ec8b0-131">Request</span></span>
<span data-ttu-id="ec8b0-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="ec8b0-133">响应</span><span class="sxs-lookup"><span data-stu-id="ec8b0-133">Response</span></span>
<span data-ttu-id="ec8b0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec8b0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get anonymousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/anonymousipriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
