---
title: Get taskTrigger
description: 从打印机获取任务触发器。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ab17b71bcdb166b4db2732b88e9ba9b3b4ddc83c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517307"
---
# <a name="get-printtasktrigger"></a><span data-ttu-id="171ea-103">获取 printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="171ea-103">Get printTaskTrigger</span></span>

<span data-ttu-id="171ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="171ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="171ea-105">从 [打印机获取](../resources/printtasktrigger.md) 任务 [触发器](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="171ea-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="171ea-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="171ea-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="171ea-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="171ea-107">Permissions</span></span>
<span data-ttu-id="171ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="171ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="171ea-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="171ea-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="171ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="171ea-111">Permission type</span></span> | <span data-ttu-id="171ea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="171ea-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="171ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="171ea-113">Delegated (work or school account)</span></span>| <span data-ttu-id="171ea-114">Printer.Read.All、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="171ea-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="171ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="171ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="171ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="171ea-116">Not Supported.</span></span>|
|<span data-ttu-id="171ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="171ea-117">Application</span></span>|<span data-ttu-id="171ea-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="171ea-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="171ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="171ea-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="171ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="171ea-120">Request headers</span></span>
|<span data-ttu-id="171ea-121">名称</span><span class="sxs-lookup"><span data-stu-id="171ea-121">Name</span></span>|<span data-ttu-id="171ea-122">说明</span><span class="sxs-lookup"><span data-stu-id="171ea-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="171ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="171ea-123">Authorization</span></span>|<span data-ttu-id="171ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="171ea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="171ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="171ea-126">Request body</span></span>
<span data-ttu-id="171ea-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="171ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="171ea-128">响应</span><span class="sxs-lookup"><span data-stu-id="171ea-128">Response</span></span>

<span data-ttu-id="171ea-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printTaskTrigger](../resources/printtasktrigger.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="171ea-129">If successful, this method returns a `200 OK` response code and a [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="171ea-130">示例</span><span class="sxs-lookup"><span data-stu-id="171ea-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="171ea-131">请求</span><span class="sxs-lookup"><span data-stu-id="171ea-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtasktrigger"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```


### <a name="response"></a><span data-ttu-id="171ea-132">响应</span><span class="sxs-lookup"><span data-stu-id="171ea-132">Response</span></span>
<span data-ttu-id="171ea-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="171ea-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/taskTriggers/$entity",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

