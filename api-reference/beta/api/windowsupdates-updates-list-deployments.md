---
title: 列出部署
description: 获取部署对象及其属性的列表。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 4eda89bc8f9bbdd2ec65f6701347f79989cdebff
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239154"
---
# <a name="list-deployments"></a><span data-ttu-id="2d620-103">列出部署</span><span class="sxs-lookup"><span data-stu-id="2d620-103">List deployments</span></span>
<span data-ttu-id="2d620-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="2d620-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d620-105">获取部署 [对象及其](../resources/windowsupdates-deployment.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="2d620-105">Get a list of [deployment](../resources/windowsupdates-deployment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d620-106">权限</span><span class="sxs-lookup"><span data-stu-id="2d620-106">Permissions</span></span>
<span data-ttu-id="2d620-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d620-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d620-109">Permission type</span></span>|<span data-ttu-id="2d620-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d620-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d620-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d620-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d620-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d620-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="2d620-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d620-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d620-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d620-114">Not supported.</span></span>|
|<span data-ttu-id="2d620-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d620-115">Application</span></span>|<span data-ttu-id="2d620-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d620-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d620-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d620-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d620-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2d620-118">Optional query parameters</span></span>
<span data-ttu-id="2d620-119">此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="2d620-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d620-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d620-120">Request headers</span></span>
|<span data-ttu-id="2d620-121">名称</span><span class="sxs-lookup"><span data-stu-id="2d620-121">Name</span></span>|<span data-ttu-id="2d620-122">说明</span><span class="sxs-lookup"><span data-stu-id="2d620-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d620-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d620-123">Authorization</span></span>|<span data-ttu-id="2d620-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d620-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d620-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d620-126">Request body</span></span>
<span data-ttu-id="2d620-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d620-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d620-128">响应</span><span class="sxs-lookup"><span data-stu-id="2d620-128">Response</span></span>

<span data-ttu-id="2d620-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [部署](../resources/windowsupdates-deployment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d620-129">If successful, this method returns a `200 OK` response code and a collection of [deployment](../resources/windowsupdates-deployment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d620-130">示例</span><span class="sxs-lookup"><span data-stu-id="2d620-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d620-131">请求</span><span class="sxs-lookup"><span data-stu-id="2d620-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2d620-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d620-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments
```
# <a name="c"></a>[<span data-ttu-id="2d620-133">C#</span><span class="sxs-lookup"><span data-stu-id="2d620-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d620-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d620-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d620-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d620-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d620-136">Java</span><span class="sxs-lookup"><span data-stu-id="2d620-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2d620-137">响应</span><span class="sxs-lookup"><span data-stu-id="2d620-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.deployment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
      "id": "b5171742-1742-b517-4217-17b5421717b5",
      "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
      },
      "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
      },
      "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```

