---
title: 获取 leakedCredentialsRiskEvent
description: 检索 leakedcredentialsriskevent 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: identity-and-sign-in
ms.openlocfilehash: 63abf3f0f1fa4ec1ca7c63f9a8a6169b0c61a821
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049322"
---
# <a name="get-leakedcredentialsriskevent-deprecated"></a><span data-ttu-id="e52ea-103">获取已弃 (的 leakedCredentialsRiskEvent) </span><span class="sxs-lookup"><span data-stu-id="e52ea-103">Get leakedCredentialsRiskEvent (deprecated)</span></span>

<span data-ttu-id="e52ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e52ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="e52ea-105">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="e52ea-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="e52ea-106">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="e52ea-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="e52ea-107">检索 leakedcredentialsriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e52ea-107">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e52ea-108">权限</span><span class="sxs-lookup"><span data-stu-id="e52ea-108">Permissions</span></span>
<span data-ttu-id="e52ea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e52ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e52ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e52ea-111">Permission type</span></span>      | <span data-ttu-id="e52ea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e52ea-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e52ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e52ea-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e52ea-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e52ea-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e52ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e52ea-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e52ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e52ea-116">Not supported.</span></span>    |
|<span data-ttu-id="e52ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e52ea-117">Application</span></span> | <span data-ttu-id="e52ea-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e52ea-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e52ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e52ea-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e52ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e52ea-120">Request headers</span></span>
| <span data-ttu-id="e52ea-121">名称</span><span class="sxs-lookup"><span data-stu-id="e52ea-121">Name</span></span>      |<span data-ttu-id="e52ea-122">说明</span><span class="sxs-lookup"><span data-stu-id="e52ea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e52ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e52ea-123">Authorization</span></span>  | <span data-ttu-id="e52ea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e52ea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e52ea-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e52ea-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e52ea-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e52ea-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e52ea-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e52ea-129">Request body</span></span>
<span data-ttu-id="e52ea-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e52ea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e52ea-131">响应</span><span class="sxs-lookup"><span data-stu-id="e52ea-131">Response</span></span>

<span data-ttu-id="e52ea-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e52ea-132">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e52ea-133">示例</span><span class="sxs-lookup"><span data-stu-id="e52ea-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e52ea-134">请求</span><span class="sxs-lookup"><span data-stu-id="e52ea-134">Request</span></span>
<span data-ttu-id="e52ea-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e52ea-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="e52ea-136">响应</span><span class="sxs-lookup"><span data-stu-id="e52ea-136">Response</span></span>
<span data-ttu-id="e52ea-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e52ea-137">Here is an example of the response.</span></span> <span data-ttu-id="e52ea-138">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e52ea-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "closedDateTime": null,
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "active",
  "riskLevel": "high",
  "riskType": "LeakedCredentialsRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


