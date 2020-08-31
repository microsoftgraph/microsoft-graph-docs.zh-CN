---
title: 列出 identityRiskEvents
description: 检索 identityriskevent 对象的列表。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 14dcac081d870a5a25ffa8afdb8dd7424e44cfd8
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311716"
---
# <a name="list-identityriskevents-deprecated"></a><span data-ttu-id="c6bbd-103">列出 identityRiskEvents (弃用) </span><span class="sxs-lookup"><span data-stu-id="c6bbd-103">List identityRiskEvents (deprecated)</span></span>

<span data-ttu-id="c6bbd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6bbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="c6bbd-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="c6bbd-106">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="c6bbd-107">检索 identityriskevent 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-107">Retrieve a list of identityriskevent objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6bbd-108">权限</span><span class="sxs-lookup"><span data-stu-id="c6bbd-108">Permissions</span></span>
<span data-ttu-id="c6bbd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6bbd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6bbd-111">Permission type</span></span>      | <span data-ttu-id="c6bbd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6bbd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6bbd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6bbd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6bbd-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6bbd-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="c6bbd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6bbd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6bbd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-116">Not supported.</span></span>    |
|<span data-ttu-id="c6bbd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6bbd-117">Application</span></span> | <span data-ttu-id="c6bbd-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6bbd-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6bbd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6bbd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="c6bbd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6bbd-120">Request headers</span></span>
| <span data-ttu-id="c6bbd-121">名称</span><span class="sxs-lookup"><span data-stu-id="c6bbd-121">Name</span></span>      |<span data-ttu-id="c6bbd-122">说明</span><span class="sxs-lookup"><span data-stu-id="c6bbd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6bbd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6bbd-123">Authorization</span></span>  | <span data-ttu-id="c6bbd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6bbd-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c6bbd-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c6bbd-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6bbd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6bbd-129">Request body</span></span>
<span data-ttu-id="c6bbd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6bbd-131">响应</span><span class="sxs-lookup"><span data-stu-id="c6bbd-131">Response</span></span>

<span data-ttu-id="c6bbd-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [identityRiskEvent](../resources/identityriskevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-132">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6bbd-133">示例</span><span class="sxs-lookup"><span data-stu-id="c6bbd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6bbd-134">请求</span><span class="sxs-lookup"><span data-stu-id="c6bbd-134">Request</span></span>
<span data-ttu-id="c6bbd-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6bbd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6bbd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityRiskEvents
```
# <a name="c"></a>[<span data-ttu-id="c6bbd-137">C#</span><span class="sxs-lookup"><span data-stu-id="c6bbd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6bbd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6bbd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6bbd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6bbd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c6bbd-140">响应</span><span class="sxs-lookup"><span data-stu-id="c6bbd-140">Response</span></span>
<span data-ttu-id="c6bbd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6bbd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
