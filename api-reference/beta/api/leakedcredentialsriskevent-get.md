---
title: 获取 leakedCredentialsRiskEvent
description: 检索 leakedcredentialsriskevent 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b5d1fb18016acad5218e6eaad2642d9caa11caa3
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181236"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="40085-103">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="40085-103">Get leakedCredentialsRiskEvent</span></span>

<span data-ttu-id="40085-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40085-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="40085-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="40085-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="40085-106">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="40085-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="40085-107">检索 leakedcredentialsriskevent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="40085-107">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40085-108">权限</span><span class="sxs-lookup"><span data-stu-id="40085-108">Permissions</span></span>
<span data-ttu-id="40085-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40085-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40085-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40085-111">Permission type</span></span>      | <span data-ttu-id="40085-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40085-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40085-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40085-113">Delegated (work or school account)</span></span> | <span data-ttu-id="40085-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="40085-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="40085-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40085-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40085-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40085-116">Not supported.</span></span>    |
|<span data-ttu-id="40085-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40085-117">Application</span></span> | <span data-ttu-id="40085-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="40085-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40085-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40085-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40085-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40085-120">Request headers</span></span>
| <span data-ttu-id="40085-121">名称</span><span class="sxs-lookup"><span data-stu-id="40085-121">Name</span></span>      |<span data-ttu-id="40085-122">说明</span><span class="sxs-lookup"><span data-stu-id="40085-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40085-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40085-123">Authorization</span></span>  | <span data-ttu-id="40085-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40085-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40085-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40085-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="40085-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="40085-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40085-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="40085-129">Request body</span></span>
<span data-ttu-id="40085-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40085-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40085-131">响应</span><span class="sxs-lookup"><span data-stu-id="40085-131">Response</span></span>

<span data-ttu-id="40085-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40085-132">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40085-133">示例</span><span class="sxs-lookup"><span data-stu-id="40085-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40085-134">请求</span><span class="sxs-lookup"><span data-stu-id="40085-134">Request</span></span>
<span data-ttu-id="40085-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40085-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="40085-136">响应</span><span class="sxs-lookup"><span data-stu-id="40085-136">Response</span></span>
<span data-ttu-id="40085-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40085-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
