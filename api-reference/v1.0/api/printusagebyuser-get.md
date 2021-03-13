---
title: 获取 printUsageByUser
description: 检索特定时间段的用户使用情况摘要。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 10a3ee5b83d2f07d9b2407f26f3b7fa210786a1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774403"
---
# <a name="get-printusagebyuser"></a><span data-ttu-id="06e11-103">获取 printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="06e11-103">Get printUsageByUser</span></span>
<span data-ttu-id="06e11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="06e11-105">检索特定时间段的用户使用情况摘要。</span><span class="sxs-lookup"><span data-stu-id="06e11-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="06e11-106">有关每个终结点的说明，请参阅 [printUsageByUser](../resources/printUsageByUser.md)。</span><span class="sxs-lookup"><span data-stu-id="06e11-106">For descriptions of each endpoint, see [printUsageByUser](../resources/printUsageByUser.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06e11-107">权限</span><span class="sxs-lookup"><span data-stu-id="06e11-107">Permissions</span></span>
<span data-ttu-id="06e11-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06e11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="06e11-110">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="06e11-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="06e11-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="06e11-111">Permission type</span></span> | <span data-ttu-id="06e11-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06e11-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="06e11-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06e11-113">Delegated (work or school account)</span></span>| <span data-ttu-id="06e11-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="06e11-114">Reports.Read.All</span></span> |
|<span data-ttu-id="06e11-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06e11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06e11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06e11-116">Not Supported.</span></span>|
|<span data-ttu-id="06e11-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="06e11-117">Application</span></span>|<span data-ttu-id="06e11-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="06e11-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06e11-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06e11-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByUser/{id}
GET /reports/monthlyPrintUsageByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06e11-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="06e11-120">Optional query parameters</span></span>
<span data-ttu-id="06e11-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="06e11-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="06e11-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="06e11-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="06e11-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="06e11-123">Request headers</span></span>
|<span data-ttu-id="06e11-124">名称</span><span class="sxs-lookup"><span data-stu-id="06e11-124">Name</span></span>|<span data-ttu-id="06e11-125">说明</span><span class="sxs-lookup"><span data-stu-id="06e11-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06e11-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="06e11-126">Authorization</span></span>|<span data-ttu-id="06e11-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06e11-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06e11-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="06e11-129">Request body</span></span>
<span data-ttu-id="06e11-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06e11-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06e11-131">响应</span><span class="sxs-lookup"><span data-stu-id="06e11-131">Response</span></span>

<span data-ttu-id="06e11-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printUsageByUser](../resources/printusagebyuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06e11-132">If successful, this method returns a `200 OK` response code and a [printUsageByUser](../resources/printusagebyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06e11-133">示例</span><span class="sxs-lookup"><span data-stu-id="06e11-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06e11-134">请求</span><span class="sxs-lookup"><span data-stu-id="06e11-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="06e11-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="06e11-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printusagebyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByUser/{id}
```
# <a name="c"></a>[<span data-ttu-id="06e11-136">C#</span><span class="sxs-lookup"><span data-stu-id="06e11-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06e11-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06e11-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06e11-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06e11-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06e11-139">Java</span><span class="sxs-lookup"><span data-stu-id="06e11-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06e11-140">响应</span><span class="sxs-lookup"><span data-stu-id="06e11-140">Response</span></span>
<span data-ttu-id="06e11-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="06e11-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "userPrincipalName": "username@contoso.com",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 42,
  "completedColorJobCount": 0,
  "incompleteJobCount": 6
}
```

