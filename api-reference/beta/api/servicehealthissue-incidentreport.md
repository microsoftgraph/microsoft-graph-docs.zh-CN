---
title: serviceHealthIssue：incidentReport
description: 提供事件后评审 (PIR) 租户的指定服务问题文档。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 1cf516a081108ba6588a93210e7d6c60967d8380
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209225"
---
# <a name="servicehealthissue-incidentreport"></a><span data-ttu-id="1e0db-103">serviceHealthIssue：incidentReport</span><span class="sxs-lookup"><span data-stu-id="1e0db-103">serviceHealthIssue: incidentReport</span></span>
<span data-ttu-id="1e0db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e0db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e0db-105">提供事件后评审 (PIR) 租户的指定服务问题文档。</span><span class="sxs-lookup"><span data-stu-id="1e0db-105">Provide the Post-Incident Review (PIR) document of a specified service issue for tenant.</span></span>

<span data-ttu-id="1e0db-106">如果租户不存在指定问题，则操作将返回错误。</span><span class="sxs-lookup"><span data-stu-id="1e0db-106">The operation returns an error if the specified issue doesn't exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e0db-107">权限</span><span class="sxs-lookup"><span data-stu-id="1e0db-107">Permissions</span></span>
<span data-ttu-id="1e0db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e0db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e0db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e0db-110">Permission type</span></span>|<span data-ttu-id="1e0db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e0db-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e0db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e0db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e0db-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e0db-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="1e0db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e0db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e0db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e0db-115">Not supported.</span></span>|
|<span data-ttu-id="1e0db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e0db-116">Application</span></span>|<span data-ttu-id="1e0db-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e0db-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e0db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e0db-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}/incidentReport
```

## <a name="request-headers"></a><span data-ttu-id="1e0db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e0db-119">Request headers</span></span>
|<span data-ttu-id="1e0db-120">名称</span><span class="sxs-lookup"><span data-stu-id="1e0db-120">Name</span></span>|<span data-ttu-id="1e0db-121">说明</span><span class="sxs-lookup"><span data-stu-id="1e0db-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1e0db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e0db-122">Authorization</span></span>|<span data-ttu-id="1e0db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e0db-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0db-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e0db-125">Request body</span></span>
<span data-ttu-id="1e0db-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e0db-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e0db-127">响应</span><span class="sxs-lookup"><span data-stu-id="1e0db-127">Response</span></span>

<span data-ttu-id="1e0db-128">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和文件流。</span><span class="sxs-lookup"><span data-stu-id="1e0db-128">If successful, this function returns a `200 OK` response code and a file stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e0db-129">示例</span><span class="sxs-lookup"><span data-stu-id="1e0db-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e0db-130">请求</span><span class="sxs-lookup"><span data-stu-id="1e0db-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1e0db-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e0db-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO248163"],
  "name": "servicehealthissue_incidentreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO248163/incidentReport
```
# <a name="c"></a>[<span data-ttu-id="1e0db-132">C#</span><span class="sxs-lookup"><span data-stu-id="1e0db-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/servicehealthissue-incidentreport-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e0db-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e0db-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/servicehealthissue-incidentreport-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e0db-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e0db-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/servicehealthissue-incidentreport-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e0db-135">Java</span><span class="sxs-lookup"><span data-stu-id="1e0db-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/servicehealthissue-incidentreport-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1e0db-136">响应</span><span class="sxs-lookup"><span data-stu-id="1e0db-136">Response</span></span>
><span data-ttu-id="1e0db-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e0db-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": "Stream"
}
```

