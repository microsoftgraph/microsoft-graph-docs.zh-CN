---
title: 获取 leakedCredentialsRiskEvent
description: 检索 leakedcredentialsriskevent 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: ae53a9ee3f9687a9bc4f248804c2e4c9060953f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979097"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="f2a3b-103">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f2a3b-103">Get leakedCredentialsRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2a3b-104">检索 leakedcredentialsriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-104">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2a3b-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2a3b-105">Permissions</span></span>
<span data-ttu-id="f2a3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2a3b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2a3b-108">Permission type</span></span>      | <span data-ttu-id="f2a3b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2a3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2a3b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2a3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2a3b-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2a3b-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="f2a3b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2a3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2a3b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-113">Not supported.</span></span>    |
|<span data-ttu-id="f2a3b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2a3b-114">Application</span></span> | <span data-ttu-id="f2a3b-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2a3b-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2a3b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2a3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f2a3b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2a3b-117">Request headers</span></span>
| <span data-ttu-id="f2a3b-118">名称</span><span class="sxs-lookup"><span data-stu-id="f2a3b-118">Name</span></span>      |<span data-ttu-id="f2a3b-119">说明</span><span class="sxs-lookup"><span data-stu-id="f2a3b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2a3b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2a3b-120">Authorization</span></span>  | <span data-ttu-id="f2a3b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2a3b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f2a3b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f2a3b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a3b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2a3b-126">Request body</span></span>
<span data-ttu-id="f2a3b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2a3b-128">响应</span><span class="sxs-lookup"><span data-stu-id="f2a3b-128">Response</span></span>

<span data-ttu-id="f2a3b-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-129">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2a3b-130">示例</span><span class="sxs-lookup"><span data-stu-id="f2a3b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2a3b-131">请求</span><span class="sxs-lookup"><span data-stu-id="f2a3b-131">Request</span></span>
<span data-ttu-id="f2a3b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="f2a3b-133">响应</span><span class="sxs-lookup"><span data-stu-id="f2a3b-133">Response</span></span>
<span data-ttu-id="f2a3b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2a3b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
