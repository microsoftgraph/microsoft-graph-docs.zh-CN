---
title: 列出 identityRiskEvents
description: 检索 identityriskevent 对象的列表。
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d92878a880154a33039bb9a745eb8f91d742dd3d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869505"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="6aa4b-103">列出 identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="6aa4b-103">List identityRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="6aa4b-104">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="6aa4b-105">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="6aa4b-106">检索 identityriskevent 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-106">Retrieve a list of identityriskevent objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aa4b-107">权限</span><span class="sxs-lookup"><span data-stu-id="6aa4b-107">Permissions</span></span>
<span data-ttu-id="6aa4b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aa4b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6aa4b-110">Permission type</span></span>      | <span data-ttu-id="6aa4b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6aa4b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aa4b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6aa4b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6aa4b-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aa4b-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="6aa4b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6aa4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aa4b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-115">Not supported.</span></span>    |
|<span data-ttu-id="6aa4b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6aa4b-116">Application</span></span> | <span data-ttu-id="6aa4b-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aa4b-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aa4b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6aa4b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="6aa4b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6aa4b-119">Request headers</span></span>
| <span data-ttu-id="6aa4b-120">名称</span><span class="sxs-lookup"><span data-stu-id="6aa4b-120">Name</span></span>      |<span data-ttu-id="6aa4b-121">说明</span><span class="sxs-lookup"><span data-stu-id="6aa4b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6aa4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aa4b-122">Authorization</span></span>  | <span data-ttu-id="6aa4b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6aa4b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6aa4b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6aa4b-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aa4b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6aa4b-128">Request body</span></span>
<span data-ttu-id="6aa4b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aa4b-130">响应</span><span class="sxs-lookup"><span data-stu-id="6aa4b-130">Response</span></span>

<span data-ttu-id="6aa4b-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[identityRiskEvent](../resources/identityriskevent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-131">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6aa4b-132">示例</span><span class="sxs-lookup"><span data-stu-id="6aa4b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6aa4b-133">请求</span><span class="sxs-lookup"><span data-stu-id="6aa4b-133">Request</span></span>
<span data-ttu-id="6aa4b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6aa4b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6aa4b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityRiskEvents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6aa4b-136">C#</span><span class="sxs-lookup"><span data-stu-id="6aa4b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6aa4b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6aa4b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6aa4b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6aa4b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6aa4b-139">响应</span><span class="sxs-lookup"><span data-stu-id="6aa4b-139">Response</span></span>
<span data-ttu-id="6aa4b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6aa4b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
