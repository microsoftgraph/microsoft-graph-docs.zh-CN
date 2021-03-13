---
title: 更新任务
description: 更新打印任务。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1375b48ccecc800111b0e84065f58324124021d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771293"
---
# <a name="update-printtask"></a><span data-ttu-id="7b14a-103">更新 printTask</span><span class="sxs-lookup"><span data-stu-id="7b14a-103">Update printTask</span></span>
<span data-ttu-id="7b14a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b14a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7b14a-105">更新打印任务。</span><span class="sxs-lookup"><span data-stu-id="7b14a-105">Update a print task.</span></span>

<span data-ttu-id="7b14a-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="7b14a-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b14a-107">权限</span><span class="sxs-lookup"><span data-stu-id="7b14a-107">Permissions</span></span>
<span data-ttu-id="7b14a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b14a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7b14a-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="7b14a-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="7b14a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b14a-111">Permission type</span></span> | <span data-ttu-id="7b14a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b14a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7b14a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b14a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7b14a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b14a-114">Not supported.</span></span> |
|<span data-ttu-id="7b14a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b14a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b14a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b14a-116">Not Supported.</span></span>|
|<span data-ttu-id="7b14a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b14a-117">Application</span></span>| <span data-ttu-id="7b14a-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b14a-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b14a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b14a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="7b14a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b14a-120">Request headers</span></span>
|<span data-ttu-id="7b14a-121">名称</span><span class="sxs-lookup"><span data-stu-id="7b14a-121">Name</span></span>|<span data-ttu-id="7b14a-122">说明</span><span class="sxs-lookup"><span data-stu-id="7b14a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b14a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b14a-123">Authorization</span></span>|<span data-ttu-id="7b14a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b14a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7b14a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b14a-126">Content-Type</span></span>|<span data-ttu-id="7b14a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7b14a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b14a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b14a-129">Request body</span></span>

<span data-ttu-id="7b14a-130">在请求正文中，提供应更新的相关 [printTask](../resources/printtask.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="7b14a-130">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="7b14a-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="7b14a-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7b14a-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7b14a-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7b14a-133">属性</span><span class="sxs-lookup"><span data-stu-id="7b14a-133">Property</span></span>     | <span data-ttu-id="7b14a-134">类型</span><span class="sxs-lookup"><span data-stu-id="7b14a-134">Type</span></span>        | <span data-ttu-id="7b14a-135">说明</span><span class="sxs-lookup"><span data-stu-id="7b14a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b14a-136">状态</span><span class="sxs-lookup"><span data-stu-id="7b14a-136">status</span></span>|<span data-ttu-id="7b14a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7b14a-137">String</span></span>|<span data-ttu-id="7b14a-138">包括 `state` `description` 描述任务当前状态的值。</span><span class="sxs-lookup"><span data-stu-id="7b14a-138">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="7b14a-139">响应</span><span class="sxs-lookup"><span data-stu-id="7b14a-139">Response</span></span>

<span data-ttu-id="7b14a-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [printTask](../resources/printtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b14a-140">If successful, this method returns a `200 OK` response code and an updated [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b14a-141">示例</span><span class="sxs-lookup"><span data-stu-id="7b14a-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b14a-142">请求</span><span class="sxs-lookup"><span data-stu-id="7b14a-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7b14a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b14a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printtask"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
Content-Type: application/json
Content-length: 152

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="7b14a-144">C#</span><span class="sxs-lookup"><span data-stu-id="7b14a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printtask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b14a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b14a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printtask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b14a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b14a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printtask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b14a-147">Java</span><span class="sxs-lookup"><span data-stu-id="7b14a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printtask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b14a-148">响应</span><span class="sxs-lookup"><span data-stu-id="7b14a-148">Response</span></span>
<span data-ttu-id="7b14a-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b14a-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "Task execution is completed."
  }
}
```

