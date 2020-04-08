---
title: 获取 anonymousIpRiskEvent
description: 检索 anonymousipriskevent 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 2fb493c35d6d26f3b1a7b4212cbe242da0062ba3
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178952"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="9f9d2-103">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9f9d2-103">Get anonymousIpRiskEvent</span></span>

<span data-ttu-id="9f9d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f9d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="9f9d2-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="9f9d2-106">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="9f9d2-107">检索 anonymousipriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-107">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f9d2-108">权限</span><span class="sxs-lookup"><span data-stu-id="9f9d2-108">Permissions</span></span>
<span data-ttu-id="9f9d2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f9d2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f9d2-111">Permission type</span></span>      | <span data-ttu-id="9f9d2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f9d2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f9d2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9d2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9f9d2-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f9d2-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="9f9d2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f9d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-116">Not supported.</span></span>    |
|<span data-ttu-id="9f9d2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f9d2-117">Application</span></span> | <span data-ttu-id="9f9d2-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f9d2-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f9d2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f9d2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f9d2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f9d2-120">Request headers</span></span>
| <span data-ttu-id="9f9d2-121">名称</span><span class="sxs-lookup"><span data-stu-id="9f9d2-121">Name</span></span>      |<span data-ttu-id="9f9d2-122">说明</span><span class="sxs-lookup"><span data-stu-id="9f9d2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f9d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f9d2-123">Authorization</span></span>  | <span data-ttu-id="9f9d2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f9d2-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f9d2-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f9d2-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f9d2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f9d2-129">Request body</span></span>
<span data-ttu-id="9f9d2-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f9d2-131">响应</span><span class="sxs-lookup"><span data-stu-id="9f9d2-131">Response</span></span>

<span data-ttu-id="9f9d2-132">如果成功，此方法在响应`200 OK`正文的值中返回响应代码和[anonymousIpRiskEvent](../resources/anonymousipriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-132">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f9d2-133">示例</span><span class="sxs-lookup"><span data-stu-id="9f9d2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f9d2-134">请求</span><span class="sxs-lookup"><span data-stu-id="9f9d2-134">Request</span></span>
<span data-ttu-id="9f9d2-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="9f9d2-136">响应</span><span class="sxs-lookup"><span data-stu-id="9f9d2-136">Response</span></span>
<span data-ttu-id="9f9d2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f9d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
