---
title: 列出 anonymousIpRiskEvents
description: 检索 anonymousipriskevent 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7935b5bcb98d5f7122f3967aeed1313315259a29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945566"
---
# <a name="list-anonymousipriskevents"></a><span data-ttu-id="45b9d-103">列出 anonymousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="45b9d-103">List anonymousIpRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45b9d-104">检索 anonymousipriskevent 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="45b9d-104">Retrieve a list of anonymousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="45b9d-105">权限</span><span class="sxs-lookup"><span data-stu-id="45b9d-105">Permissions</span></span>
<span data-ttu-id="45b9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45b9d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="45b9d-108">Permission type</span></span>      | <span data-ttu-id="45b9d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45b9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45b9d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45b9d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45b9d-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="45b9d-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="45b9d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45b9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45b9d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="45b9d-113">Not supported.</span></span>    |
|<span data-ttu-id="45b9d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="45b9d-114">Application</span></span> | <span data-ttu-id="45b9d-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="45b9d-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45b9d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45b9d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents
```

## <a name="request-headers"></a><span data-ttu-id="45b9d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="45b9d-117">Request headers</span></span>
| <span data-ttu-id="45b9d-118">名称</span><span class="sxs-lookup"><span data-stu-id="45b9d-118">Name</span></span>      |<span data-ttu-id="45b9d-119">说明</span><span class="sxs-lookup"><span data-stu-id="45b9d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45b9d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="45b9d-120">Authorization</span></span>  | <span data-ttu-id="45b9d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45b9d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45b9d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="45b9d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="45b9d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="45b9d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45b9d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="45b9d-126">Request body</span></span>
<span data-ttu-id="45b9d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45b9d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45b9d-128">响应</span><span class="sxs-lookup"><span data-stu-id="45b9d-128">Response</span></span>

<span data-ttu-id="45b9d-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="45b9d-129">If successful, this method returns a `200 OK` response code and collection of [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45b9d-130">示例</span><span class="sxs-lookup"><span data-stu-id="45b9d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45b9d-131">请求</span><span class="sxs-lookup"><span data-stu-id="45b9d-131">Request</span></span>
<span data-ttu-id="45b9d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45b9d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="45b9d-133">响应</span><span class="sxs-lookup"><span data-stu-id="45b9d-133">Response</span></span>
<span data-ttu-id="45b9d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45b9d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List anonymousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
