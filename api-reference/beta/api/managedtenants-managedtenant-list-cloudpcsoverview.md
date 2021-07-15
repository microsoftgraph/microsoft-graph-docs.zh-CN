---
title: 列出 cloudPcOverviews
description: 获取 cloudPcOverview 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: fa30d449a30d5c3657dcf8a785342a45d0e6a094
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441467"
---
# <a name="list-cloudpcoverviews"></a><span data-ttu-id="2b0b9-103">列出 cloudPcOverviews</span><span class="sxs-lookup"><span data-stu-id="2b0b9-103">List cloudPcOverviews</span></span>
<span data-ttu-id="2b0b9-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2b0b9-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b0b9-105">获取 [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-105">Get a list of the [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b0b9-106">权限</span><span class="sxs-lookup"><span data-stu-id="2b0b9-106">Permissions</span></span>
<span data-ttu-id="2b0b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b0b9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b0b9-109">Permission type</span></span>|<span data-ttu-id="2b0b9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b0b9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b0b9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b0b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b0b9-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b0b9-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="2b0b9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b0b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b0b9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-114">Not supported.</span></span>|
|<span data-ttu-id="2b0b9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b0b9-115">Application</span></span>|<span data-ttu-id="2b0b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b0b9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b0b9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcsOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b0b9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2b0b9-118">Optional query parameters</span></span>
<span data-ttu-id="2b0b9-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b0b9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b0b9-120">Request headers</span></span>
|<span data-ttu-id="2b0b9-121">名称</span><span class="sxs-lookup"><span data-stu-id="2b0b9-121">Name</span></span>|<span data-ttu-id="2b0b9-122">说明</span><span class="sxs-lookup"><span data-stu-id="2b0b9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b0b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b0b9-123">Authorization</span></span>|<span data-ttu-id="2b0b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b0b9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b0b9-126">Request body</span></span>
<span data-ttu-id="2b0b9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b0b9-128">响应</span><span class="sxs-lookup"><span data-stu-id="2b0b9-128">Response</span></span>

<span data-ttu-id="2b0b9-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b0b9-130">示例</span><span class="sxs-lookup"><span data-stu-id="2b0b9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b0b9-131">请求</span><span class="sxs-lookup"><span data-stu-id="2b0b9-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2b0b9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b0b9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcsOverview
```
# <a name="c"></a>[<span data-ttu-id="2b0b9-133">C#</span><span class="sxs-lookup"><span data-stu-id="2b0b9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcoverview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b0b9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b0b9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcoverview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b0b9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b0b9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcoverview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b0b9-136">Java</span><span class="sxs-lookup"><span data-stu-id="2b0b9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcoverview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2b0b9-137">响应</span><span class="sxs-lookup"><span data-stu-id="2b0b9-137">Response</span></span>
><span data-ttu-id="2b0b9-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2b0b9-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcOverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.cloudPcOverview",
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee",
      "totalCloudPcStatus": 18,
      "numberOfCloudPcStatusNotProvisioned": 4,
      "numberOfCloudPcStatusProvisioning": 0,
      "numberOfCloudPcStatusProvisioned": 14,
      "numberOfCloudPcStatusUpgrading": 0,
      "numberOfCloudPcStatusInGracePeriod": 0,
      "numberOfCloudPcStatusDeprovisioning": 0,
      "numberOfCloudPcStatusFailed": 0,
      "numberOfCloudPcStatusUnknown": 0,
      "totalCloudPcConnectionStatus": 25,
      "numberOfCloudPcConnectionStatusPending": 0,
      "numberOfCloudPcConnectionStatusRunning": 0,
      "numberOfCloudPcConnectionStatusPassed": 17,
      "numberOfCloudPcConnectionStatusFailed": 6,
      "numberOfCloudPcConnectionStatusUnkownFutureValue": 0,
      "lastRefreshedDateTime": "2021-07-11T17:18:46.4830816Z"
    }
  ]
}
```
