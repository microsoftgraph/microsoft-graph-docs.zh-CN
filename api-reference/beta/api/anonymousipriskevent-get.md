---
title: 获取 anonymousIpRiskEvent
description: 检索 anonymousipriskevent 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: dd89350360f045659697da747525bf0bfa6ec96a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945583"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="152ef-103">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="152ef-103">Get anonymousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="152ef-104">检索 anonymousipriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="152ef-104">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="152ef-105">权限</span><span class="sxs-lookup"><span data-stu-id="152ef-105">Permissions</span></span>
<span data-ttu-id="152ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="152ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="152ef-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="152ef-108">Permission type</span></span>      | <span data-ttu-id="152ef-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="152ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="152ef-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="152ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="152ef-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="152ef-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="152ef-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="152ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="152ef-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="152ef-113">Not supported.</span></span>    |
|<span data-ttu-id="152ef-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="152ef-114">Application</span></span> | <span data-ttu-id="152ef-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="152ef-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="152ef-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="152ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="152ef-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="152ef-117">Request headers</span></span>
| <span data-ttu-id="152ef-118">名称</span><span class="sxs-lookup"><span data-stu-id="152ef-118">Name</span></span>      |<span data-ttu-id="152ef-119">说明</span><span class="sxs-lookup"><span data-stu-id="152ef-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="152ef-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="152ef-120">Authorization</span></span>  | <span data-ttu-id="152ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="152ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="152ef-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="152ef-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="152ef-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="152ef-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="152ef-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="152ef-126">Request body</span></span>
<span data-ttu-id="152ef-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="152ef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="152ef-128">响应</span><span class="sxs-lookup"><span data-stu-id="152ef-128">Response</span></span>

<span data-ttu-id="152ef-129">如果成功, 此方法在响应`200 OK`正文的值中返回响应代码和[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="152ef-129">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="152ef-130">示例</span><span class="sxs-lookup"><span data-stu-id="152ef-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="152ef-131">请求</span><span class="sxs-lookup"><span data-stu-id="152ef-131">Request</span></span>
<span data-ttu-id="152ef-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="152ef-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="152ef-133">响应</span><span class="sxs-lookup"><span data-stu-id="152ef-133">Response</span></span>
<span data-ttu-id="152ef-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
