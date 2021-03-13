---
title: 获取任务
description: 获取有关打印任务的详细信息。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7b9a9b2e5ff6fdcc3e7bd7c74aa5a173d551f41b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773443"
---
# <a name="get-printtask"></a><span data-ttu-id="3514c-103">获取 printTask</span><span class="sxs-lookup"><span data-stu-id="3514c-103">Get printTask</span></span>
<span data-ttu-id="3514c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3514c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="3514c-105">获取有关打印任务的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3514c-105">Get details about a print task.</span></span>

<span data-ttu-id="3514c-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="3514c-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="3514c-107">权限</span><span class="sxs-lookup"><span data-stu-id="3514c-107">Permissions</span></span>
<span data-ttu-id="3514c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3514c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3514c-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="3514c-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3514c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3514c-111">Permission type</span></span> | <span data-ttu-id="3514c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3514c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3514c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3514c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3514c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3514c-114">Not supported.</span></span> |
|<span data-ttu-id="3514c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3514c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3514c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3514c-116">Not Supported.</span></span>|
|<span data-ttu-id="3514c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3514c-117">Application</span></span>| <span data-ttu-id="3514c-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3514c-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3514c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3514c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="3514c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3514c-120">Request headers</span></span>
|<span data-ttu-id="3514c-121">名称</span><span class="sxs-lookup"><span data-stu-id="3514c-121">Name</span></span>|<span data-ttu-id="3514c-122">说明</span><span class="sxs-lookup"><span data-stu-id="3514c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3514c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3514c-123">Authorization</span></span>|<span data-ttu-id="3514c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3514c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3514c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3514c-126">Request body</span></span>
<span data-ttu-id="3514c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3514c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3514c-128">响应</span><span class="sxs-lookup"><span data-stu-id="3514c-128">Response</span></span>

<span data-ttu-id="3514c-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printTask](../resources/printtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3514c-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3514c-130">示例</span><span class="sxs-lookup"><span data-stu-id="3514c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3514c-131">请求</span><span class="sxs-lookup"><span data-stu-id="3514c-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3514c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3514c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```
# <a name="c"></a>[<span data-ttu-id="3514c-133">C#</span><span class="sxs-lookup"><span data-stu-id="3514c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3514c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3514c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3514c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3514c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3514c-136">Java</span><span class="sxs-lookup"><span data-stu-id="3514c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printtask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3514c-137">响应</span><span class="sxs-lookup"><span data-stu-id="3514c-137">Response</span></span>
<span data-ttu-id="3514c-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3514c-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions('3203656e-6069-4e10-8147-d25290b00a3c')/tasks/$entity",
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

