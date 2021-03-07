---
title: Delete taskDefinition
description: 删除任务定义。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 457ebc3ba3f2e125b5d252c138ed08b28d3e0798
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516963"
---
# <a name="delete-printtaskdefinition"></a><span data-ttu-id="2d981-103">删除 printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="2d981-103">Delete printTaskDefinition</span></span>
<span data-ttu-id="2d981-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d981-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2d981-105">删除 **taskDefinition**。</span><span class="sxs-lookup"><span data-stu-id="2d981-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="2d981-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="2d981-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d981-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2d981-107">Permissions</span></span>
<span data-ttu-id="2d981-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2d981-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="2d981-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="2d981-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d981-111">Permission type</span></span> | <span data-ttu-id="2d981-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d981-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2d981-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d981-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2d981-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d981-114">Not supported.</span></span> |
|<span data-ttu-id="2d981-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d981-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d981-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d981-116">Not Supported.</span></span>|
|<span data-ttu-id="2d981-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d981-117">Application</span></span>| <span data-ttu-id="2d981-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d981-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d981-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d981-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="2d981-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d981-120">Request headers</span></span>
|<span data-ttu-id="2d981-121">名称</span><span class="sxs-lookup"><span data-stu-id="2d981-121">Name</span></span>|<span data-ttu-id="2d981-122">说明</span><span class="sxs-lookup"><span data-stu-id="2d981-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d981-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d981-123">Authorization</span></span>|<span data-ttu-id="2d981-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d981-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d981-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d981-126">Request body</span></span>
<span data-ttu-id="2d981-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d981-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d981-128">响应</span><span class="sxs-lookup"><span data-stu-id="2d981-128">Response</span></span>
<span data-ttu-id="2d981-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d981-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d981-131">示例</span><span class="sxs-lookup"><span data-stu-id="2d981-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d981-132">请求</span><span class="sxs-lookup"><span data-stu-id="2d981-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printtaskdefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```


### <a name="response"></a><span data-ttu-id="2d981-133">响应</span><span class="sxs-lookup"><span data-stu-id="2d981-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

