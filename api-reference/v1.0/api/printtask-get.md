---
title: 获取任务
description: 获取有关打印任务的详细信息。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0aff8e70271a0903289a50eb4fb76b21d9269cab
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516973"
---
# <a name="get-printtask"></a><span data-ttu-id="26b1b-103">获取 printTask</span><span class="sxs-lookup"><span data-stu-id="26b1b-103">Get printTask</span></span>
<span data-ttu-id="26b1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="26b1b-105">获取有关打印任务的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26b1b-105">Get details about a print task.</span></span>

<span data-ttu-id="26b1b-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="26b1b-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="26b1b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="26b1b-107">Permissions</span></span>
<span data-ttu-id="26b1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26b1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="26b1b-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="26b1b-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="26b1b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="26b1b-111">Permission type</span></span> | <span data-ttu-id="26b1b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26b1b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="26b1b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26b1b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="26b1b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26b1b-114">Not supported.</span></span> |
|<span data-ttu-id="26b1b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26b1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26b1b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="26b1b-116">Not Supported.</span></span>|
|<span data-ttu-id="26b1b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="26b1b-117">Application</span></span>| <span data-ttu-id="26b1b-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b1b-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26b1b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26b1b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="26b1b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="26b1b-120">Request headers</span></span>
|<span data-ttu-id="26b1b-121">名称</span><span class="sxs-lookup"><span data-stu-id="26b1b-121">Name</span></span>|<span data-ttu-id="26b1b-122">说明</span><span class="sxs-lookup"><span data-stu-id="26b1b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26b1b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26b1b-123">Authorization</span></span>|<span data-ttu-id="26b1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26b1b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b1b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26b1b-126">Request body</span></span>
<span data-ttu-id="26b1b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26b1b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b1b-128">响应</span><span class="sxs-lookup"><span data-stu-id="26b1b-128">Response</span></span>

<span data-ttu-id="26b1b-129">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [printTask](../resources/printtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="26b1b-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26b1b-130">示例</span><span class="sxs-lookup"><span data-stu-id="26b1b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26b1b-131">请求</span><span class="sxs-lookup"><span data-stu-id="26b1b-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

### <a name="response"></a><span data-ttu-id="26b1b-132">响应</span><span class="sxs-lookup"><span data-stu-id="26b1b-132">Response</span></span>
<span data-ttu-id="26b1b-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="26b1b-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

