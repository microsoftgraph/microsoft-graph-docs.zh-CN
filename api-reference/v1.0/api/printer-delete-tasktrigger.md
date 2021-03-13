---
title: 删除 printTaskTrigger
description: 删除打印机的任务触发器。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bba66bb6c11d930b1b9065769181f55efc114dd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772014"
---
# <a name="delete-printtasktrigger"></a><span data-ttu-id="bfb38-103">删除 printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="bfb38-103">Delete printTaskTrigger</span></span>
<span data-ttu-id="bfb38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfb38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="bfb38-105">删除[打印机的任务](../resources/printtasktrigger.md)[触发器](../resources/printer.md)，以防止相关打印事件触发指定打印机上的任务。</span><span class="sxs-lookup"><span data-stu-id="bfb38-105">Delete the [task trigger](../resources/printtasktrigger.md) of a [printer](../resources/printer.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfb38-106">权限</span><span class="sxs-lookup"><span data-stu-id="bfb38-106">Permissions</span></span>
<span data-ttu-id="bfb38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfb38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bfb38-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="bfb38-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="bfb38-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfb38-110">Permission type</span></span> | <span data-ttu-id="bfb38-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfb38-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bfb38-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb38-112">Delegated (work or school account)</span></span>| <span data-ttu-id="bfb38-113">Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bfb38-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="bfb38-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfb38-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfb38-115">Not Supported.</span></span>|
|<span data-ttu-id="bfb38-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfb38-116">Application</span></span>|<span data-ttu-id="bfb38-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfb38-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfb38-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfb38-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="bfb38-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfb38-119">Request headers</span></span>
|<span data-ttu-id="bfb38-120">名称</span><span class="sxs-lookup"><span data-stu-id="bfb38-120">Name</span></span>|<span data-ttu-id="bfb38-121">说明</span><span class="sxs-lookup"><span data-stu-id="bfb38-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bfb38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfb38-122">Authorization</span></span>|<span data-ttu-id="bfb38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfb38-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfb38-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfb38-125">Request body</span></span>
<span data-ttu-id="bfb38-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfb38-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfb38-127">响应</span><span class="sxs-lookup"><span data-stu-id="bfb38-127">Response</span></span>

<span data-ttu-id="bfb38-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bfb38-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bfb38-129">示例</span><span class="sxs-lookup"><span data-stu-id="bfb38-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bfb38-130">请求</span><span class="sxs-lookup"><span data-stu-id="bfb38-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bfb38-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb38-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printtasktrigger"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="bfb38-132">C#</span><span class="sxs-lookup"><span data-stu-id="bfb38-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printtasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfb38-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfb38-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printtasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfb38-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfb38-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printtasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfb38-135">Java</span><span class="sxs-lookup"><span data-stu-id="bfb38-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printtasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bfb38-136">响应</span><span class="sxs-lookup"><span data-stu-id="bfb38-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

