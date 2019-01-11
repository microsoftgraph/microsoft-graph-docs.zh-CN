---
title: 列表 identityRiskEvents
description: 检索 identityriskevent 对象的列表。
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: fbd5e739986ded9fa6f5346e35808f4018bff625
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894248"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="ad691-103">列表 identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="ad691-103">List identityRiskEvents</span></span>

> <span data-ttu-id="ad691-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad691-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad691-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad691-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad691-106">检索 identityriskevent 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ad691-106">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad691-107">权限</span><span class="sxs-lookup"><span data-stu-id="ad691-107">Permissions</span></span>
<span data-ttu-id="ad691-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad691-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad691-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad691-110">Permission type</span></span>      | <span data-ttu-id="ad691-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad691-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad691-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad691-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad691-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad691-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="ad691-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad691-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad691-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad691-115">Not supported.</span></span>    |
|<span data-ttu-id="ad691-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad691-116">Application</span></span> | <span data-ttu-id="ad691-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad691-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad691-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad691-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="ad691-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad691-119">Request headers</span></span>
| <span data-ttu-id="ad691-120">名称</span><span class="sxs-lookup"><span data-stu-id="ad691-120">Name</span></span>      |<span data-ttu-id="ad691-121">说明</span><span class="sxs-lookup"><span data-stu-id="ad691-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad691-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad691-122">Authorization</span></span>  | <span data-ttu-id="ad691-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad691-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad691-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ad691-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ad691-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ad691-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad691-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad691-128">Request body</span></span>
<span data-ttu-id="ad691-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad691-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad691-130">响应</span><span class="sxs-lookup"><span data-stu-id="ad691-130">Response</span></span>

<span data-ttu-id="ad691-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[identityRiskEvent](../resources/identityriskevent.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="ad691-131">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad691-132">示例</span><span class="sxs-lookup"><span data-stu-id="ad691-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad691-133">请求</span><span class="sxs-lookup"><span data-stu-id="ad691-133">Request</span></span>
<span data-ttu-id="ad691-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad691-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="ad691-135">响应</span><span class="sxs-lookup"><span data-stu-id="ad691-135">Response</span></span>
<span data-ttu-id="ad691-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad691-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
