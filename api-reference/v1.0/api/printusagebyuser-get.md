---
title: 获取 printUsageByUser
description: 检索特定时间段的用户使用情况摘要。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 76341cdcb2b96e57f4c7d0454fe45de977311507
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517323"
---
# <a name="get-printusagebyuser"></a><span data-ttu-id="95bb3-103">获取 printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="95bb3-103">Get printUsageByUser</span></span>
<span data-ttu-id="95bb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95bb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="95bb3-105">检索特定时间段的用户使用情况摘要。</span><span class="sxs-lookup"><span data-stu-id="95bb3-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="95bb3-106">有关每个终结点的说明，请参阅 [printUsageByUser](../resources/printUsageByUser.md)。</span><span class="sxs-lookup"><span data-stu-id="95bb3-106">For descriptions of each endpoint, see [printUsageByUser](../resources/printUsageByUser.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="95bb3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="95bb3-107">Permissions</span></span>
<span data-ttu-id="95bb3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95bb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="95bb3-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="95bb3-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="95bb3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="95bb3-111">Permission type</span></span> | <span data-ttu-id="95bb3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95bb3-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="95bb3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95bb3-113">Delegated (work or school account)</span></span>| <span data-ttu-id="95bb3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb3-114">Reports.Read.All</span></span> |
|<span data-ttu-id="95bb3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95bb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95bb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="95bb3-116">Not Supported.</span></span>|
|<span data-ttu-id="95bb3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="95bb3-117">Application</span></span>|<span data-ttu-id="95bb3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="95bb3-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95bb3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95bb3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByUser/{id}
GET /reports/monthlyPrintUsageByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95bb3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="95bb3-120">Optional query parameters</span></span>
<span data-ttu-id="95bb3-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="95bb3-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="95bb3-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="95bb3-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="95bb3-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="95bb3-123">Request headers</span></span>
|<span data-ttu-id="95bb3-124">名称</span><span class="sxs-lookup"><span data-stu-id="95bb3-124">Name</span></span>|<span data-ttu-id="95bb3-125">说明</span><span class="sxs-lookup"><span data-stu-id="95bb3-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="95bb3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="95bb3-126">Authorization</span></span>|<span data-ttu-id="95bb3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95bb3-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95bb3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="95bb3-129">Request body</span></span>
<span data-ttu-id="95bb3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="95bb3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95bb3-131">响应</span><span class="sxs-lookup"><span data-stu-id="95bb3-131">Response</span></span>

<span data-ttu-id="95bb3-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printUsageByUser](../resources/printusagebyuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95bb3-132">If successful, this method returns a `200 OK` response code and a [printUsageByUser](../resources/printusagebyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95bb3-133">示例</span><span class="sxs-lookup"><span data-stu-id="95bb3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="95bb3-134">请求</span><span class="sxs-lookup"><span data-stu-id="95bb3-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printusagebyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByUser/{id}
```

### <a name="response"></a><span data-ttu-id="95bb3-135">响应</span><span class="sxs-lookup"><span data-stu-id="95bb3-135">Response</span></span>
<span data-ttu-id="95bb3-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="95bb3-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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

