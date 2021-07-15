---
title: 列出 cloudPcConnections
description: 获取 cloudPcConnection 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e0b8ab55319ed04d64318d422b36a57550dc29a0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441569"
---
# <a name="list-cloudpcconnections"></a><span data-ttu-id="0a0cb-103">列出 cloudPcConnections</span><span class="sxs-lookup"><span data-stu-id="0a0cb-103">List cloudPcConnections</span></span>
<span data-ttu-id="0a0cb-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0a0cb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a0cb-105">获取 [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-105">Get a list of the [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a0cb-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a0cb-106">Permissions</span></span>
<span data-ttu-id="0a0cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a0cb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a0cb-109">Permission type</span></span>|<span data-ttu-id="0a0cb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a0cb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a0cb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a0cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a0cb-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a0cb-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="0a0cb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a0cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a0cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-114">Not supported.</span></span>|
|<span data-ttu-id="0a0cb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a0cb-115">Application</span></span>|<span data-ttu-id="0a0cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a0cb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a0cb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcConnections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a0cb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0a0cb-118">Optional query parameters</span></span>
<span data-ttu-id="0a0cb-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a0cb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a0cb-120">Request headers</span></span>
|<span data-ttu-id="0a0cb-121">名称</span><span class="sxs-lookup"><span data-stu-id="0a0cb-121">Name</span></span>|<span data-ttu-id="0a0cb-122">说明</span><span class="sxs-lookup"><span data-stu-id="0a0cb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a0cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a0cb-123">Authorization</span></span>|<span data-ttu-id="0a0cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a0cb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a0cb-126">Request body</span></span>
<span data-ttu-id="0a0cb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a0cb-128">响应</span><span class="sxs-lookup"><span data-stu-id="0a0cb-128">Response</span></span>

<span data-ttu-id="0a0cb-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a0cb-130">示例</span><span class="sxs-lookup"><span data-stu-id="0a0cb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a0cb-131">请求</span><span class="sxs-lookup"><span data-stu-id="0a0cb-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0a0cb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a0cb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcconnection"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcConnections
```
# <a name="c"></a>[<span data-ttu-id="0a0cb-133">C#</span><span class="sxs-lookup"><span data-stu-id="0a0cb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a0cb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a0cb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a0cb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a0cb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a0cb-136">Java</span><span class="sxs-lookup"><span data-stu-id="0a0cb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0a0cb-137">响应</span><span class="sxs-lookup"><span data-stu-id="0a0cb-137">Response</span></span>
><span data-ttu-id="0a0cb-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a0cb-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcConnection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/cloudPcConnections",
  "value": [
    {
      "id": "021bd3a9-59c6-4503-b408-c326a98f238f",
      "lastUpdated": "2021-07-11T18:02:16.6450704Z",
      "displayName": "RunnerPlus-Az-Connection",
      "organizationId": "0b9701e1-f1ae-4f15-bd67-f4f591595454",
      "organizationDisplayName": "Terra Firm",
      "healthCheckStatus": "Passed",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee",
      "lastRefreshedDateTime": "2021-07-11T18:02:16.6450704Z"
    }
  ]
}
```
