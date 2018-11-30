---
title: 获取 leakedCredentialsRiskEvent
description: 检索的属性和 leakedcredentialsriskevent 对象的关系。
ms.openlocfilehash: a3d259f785d2c8d6717f4dfe90ba04aeb454a1bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048853"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="f9ee1-103">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f9ee1-103">Get leakedCredentialsRiskEvent</span></span>

> <span data-ttu-id="f9ee1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9ee1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9ee1-106">检索的属性和 leakedcredentialsriskevent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-106">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9ee1-107">权限</span><span class="sxs-lookup"><span data-stu-id="f9ee1-107">Permissions</span></span>
<span data-ttu-id="f9ee1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ee1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9ee1-110">Permission type</span></span>      | <span data-ttu-id="f9ee1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9ee1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9ee1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9ee1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9ee1-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9ee1-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="f9ee1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9ee1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ee1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-115">Not supported.</span></span>    |
|<span data-ttu-id="f9ee1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9ee1-116">Application</span></span> | <span data-ttu-id="f9ee1-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9ee1-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ee1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9ee1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f9ee1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9ee1-119">Request headers</span></span>
| <span data-ttu-id="f9ee1-120">名称</span><span class="sxs-lookup"><span data-stu-id="f9ee1-120">Name</span></span>      |<span data-ttu-id="f9ee1-121">说明</span><span class="sxs-lookup"><span data-stu-id="f9ee1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9ee1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9ee1-122">Authorization</span></span>  | <span data-ttu-id="f9ee1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9ee1-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9ee1-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9ee1-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9ee1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9ee1-128">Request body</span></span>
<span data-ttu-id="f9ee1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ee1-130">响应</span><span class="sxs-lookup"><span data-stu-id="f9ee1-130">Response</span></span>

<span data-ttu-id="f9ee1-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-131">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9ee1-132">示例</span><span class="sxs-lookup"><span data-stu-id="f9ee1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9ee1-133">请求</span><span class="sxs-lookup"><span data-stu-id="f9ee1-133">Request</span></span>
<span data-ttu-id="f9ee1-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="f9ee1-135">响应</span><span class="sxs-lookup"><span data-stu-id="f9ee1-135">Response</span></span>
<span data-ttu-id="f9ee1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9ee1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
