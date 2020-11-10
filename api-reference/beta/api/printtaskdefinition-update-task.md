---
title: 更新任务
description: 更新打印任务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6ed3b7b4faac9709621485027d7601994ead8a5c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968119"
---
# <a name="update-task"></a><span data-ttu-id="8f039-103">更新任务</span><span class="sxs-lookup"><span data-stu-id="8f039-103">Update task</span></span>

<span data-ttu-id="8f039-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f039-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f039-105">更新打印任务。</span><span class="sxs-lookup"><span data-stu-id="8f039-105">Update a print task.</span></span>

<span data-ttu-id="8f039-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅 [扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="8f039-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f039-107">权限</span><span class="sxs-lookup"><span data-stu-id="8f039-107">Permissions</span></span>
<span data-ttu-id="8f039-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8f039-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="8f039-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8f039-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f039-111">Permission type</span></span> | <span data-ttu-id="8f039-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f039-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8f039-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f039-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8f039-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f039-114">Not supported.</span></span> |
|<span data-ttu-id="8f039-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f039-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f039-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f039-116">Not Supported.</span></span>|
|<span data-ttu-id="8f039-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f039-117">Application</span></span>| <span data-ttu-id="8f039-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f039-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f039-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f039-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f039-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f039-120">Request headers</span></span>
| <span data-ttu-id="8f039-121">名称</span><span class="sxs-lookup"><span data-stu-id="8f039-121">Name</span></span>      |<span data-ttu-id="8f039-122">说明</span><span class="sxs-lookup"><span data-stu-id="8f039-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f039-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f039-123">Authorization</span></span> | <span data-ttu-id="8f039-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f039-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f039-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f039-126">Request body</span></span>
<span data-ttu-id="8f039-127">在请求正文中，提供应更新的相关 [printTask](../resources/printtask.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="8f039-127">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="8f039-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8f039-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8f039-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8f039-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8f039-130">属性</span><span class="sxs-lookup"><span data-stu-id="8f039-130">Property</span></span>     | <span data-ttu-id="8f039-131">类型</span><span class="sxs-lookup"><span data-stu-id="8f039-131">Type</span></span>        | <span data-ttu-id="8f039-132">说明</span><span class="sxs-lookup"><span data-stu-id="8f039-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f039-133">status</span><span class="sxs-lookup"><span data-stu-id="8f039-133">status</span></span>|<span data-ttu-id="8f039-134">String</span><span class="sxs-lookup"><span data-stu-id="8f039-134">String</span></span>|<span data-ttu-id="8f039-135">包含 `state` 和 `description` 值，用于描述任务的当前状态。</span><span class="sxs-lookup"><span data-stu-id="8f039-135">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="8f039-136">响应</span><span class="sxs-lookup"><span data-stu-id="8f039-136">Response</span></span>
<span data-ttu-id="8f039-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f039-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f039-139">示例</span><span class="sxs-lookup"><span data-stu-id="8f039-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f039-140">请求</span><span class="sxs-lookup"><span data-stu-id="8f039-140">Request</span></span>
<span data-ttu-id="8f039-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8f039-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f039-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f039-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_task"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8f039-143">C#</span><span class="sxs-lookup"><span data-stu-id="8f039-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f039-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f039-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f039-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f039-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f039-146">Java</span><span class="sxs-lookup"><span data-stu-id="8f039-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="8f039-147">响应</span><span class="sxs-lookup"><span data-stu-id="8f039-147">Response</span></span>
<span data-ttu-id="8f039-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8f039-148">The following is an example of the response.</span></span>
><span data-ttu-id="8f039-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8f039-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


