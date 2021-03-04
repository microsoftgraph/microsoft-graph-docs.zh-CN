---
title: 获取 unfamiliarLocationRiskEvent
description: 检索 unfamiliarlocationriskevent 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: 7107c46fc18f3586e7aababbfc2fbea1e285e98a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444881"
---
# <a name="get-unfamiliarlocationriskevent-deprecated"></a><span data-ttu-id="a1a3c-103">获取已弃 (的 unfamiliarLocationRiskEvent) </span><span class="sxs-lookup"><span data-stu-id="a1a3c-103">Get unfamiliarLocationRiskEvent (deprecated)</span></span>

<span data-ttu-id="a1a3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1a3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="a1a3c-105">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="a1a3c-106">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="a1a3c-107">检索 unfamiliarlocationriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-107">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1a3c-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="a1a3c-108">Permissions</span></span>
<span data-ttu-id="a1a3c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a3c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1a3c-111">Permission type</span></span>      | <span data-ttu-id="a1a3c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1a3c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1a3c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1a3c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a1a3c-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a3c-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="a1a3c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1a3c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1a3c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-116">Not supported.</span></span>    |
|<span data-ttu-id="a1a3c-117">Application</span><span class="sxs-lookup"><span data-stu-id="a1a3c-117">Application</span></span> | <span data-ttu-id="a1a3c-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a3c-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1a3c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1a3c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a1a3c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1a3c-120">Request headers</span></span>
| <span data-ttu-id="a1a3c-121">名称</span><span class="sxs-lookup"><span data-stu-id="a1a3c-121">Name</span></span>      |<span data-ttu-id="a1a3c-122">说明</span><span class="sxs-lookup"><span data-stu-id="a1a3c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a1a3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1a3c-123">Authorization</span></span>  | <span data-ttu-id="a1a3c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1a3c-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a1a3c-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="a1a3c-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a3c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1a3c-129">Request body</span></span>
<span data-ttu-id="a1a3c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1a3c-131">响应</span><span class="sxs-lookup"><span data-stu-id="a1a3c-131">Response</span></span>

<span data-ttu-id="a1a3c-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-132">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1a3c-133">示例</span><span class="sxs-lookup"><span data-stu-id="a1a3c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1a3c-134">请求</span><span class="sxs-lookup"><span data-stu-id="a1a3c-134">Request</span></span>
<span data-ttu-id="a1a3c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="a1a3c-136">响应</span><span class="sxs-lookup"><span data-stu-id="a1a3c-136">Response</span></span>
<span data-ttu-id="a1a3c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1a3c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


