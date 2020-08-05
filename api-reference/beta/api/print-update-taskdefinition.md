---
title: Update taskDefinition
description: 更新任务定义。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 60c8c53cc28724a7b36e00d1b1695288356cb343
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566385"
---
# <a name="update-taskdefinition"></a><span data-ttu-id="009c7-103">Update taskDefinition</span><span class="sxs-lookup"><span data-stu-id="009c7-103">Update taskDefinition</span></span>

<span data-ttu-id="009c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="009c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="009c7-105">更新任务定义。</span><span class="sxs-lookup"><span data-stu-id="009c7-105">Update a task definition.</span></span>

<span data-ttu-id="009c7-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="009c7-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="009c7-107">权限</span><span class="sxs-lookup"><span data-stu-id="009c7-107">Permissions</span></span>
<span data-ttu-id="009c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="009c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="009c7-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="009c7-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="009c7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="009c7-111">Permission type</span></span> | <span data-ttu-id="009c7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="009c7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="009c7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="009c7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="009c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="009c7-114">Not supported.</span></span> |
|<span data-ttu-id="009c7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="009c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="009c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="009c7-116">Not Supported.</span></span>|
|<span data-ttu-id="009c7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="009c7-117">Application</span></span>| <span data-ttu-id="009c7-118">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="009c7-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="009c7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="009c7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="009c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="009c7-120">Request headers</span></span>
| <span data-ttu-id="009c7-121">名称</span><span class="sxs-lookup"><span data-stu-id="009c7-121">Name</span></span>      |<span data-ttu-id="009c7-122">说明</span><span class="sxs-lookup"><span data-stu-id="009c7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="009c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="009c7-123">Authorization</span></span> | <span data-ttu-id="009c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="009c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="009c7-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="009c7-126">Content-type</span></span>  | <span data-ttu-id="009c7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="009c7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="009c7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="009c7-129">Request body</span></span>
<span data-ttu-id="009c7-130">在请求正文中，提供应更新的相关[printTaskDefinition](../resources/printtaskdefinition.md)字段的值。</span><span class="sxs-lookup"><span data-stu-id="009c7-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="009c7-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="009c7-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="009c7-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="009c7-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="009c7-133">属性</span><span class="sxs-lookup"><span data-stu-id="009c7-133">Property</span></span>     | <span data-ttu-id="009c7-134">类型</span><span class="sxs-lookup"><span data-stu-id="009c7-134">Type</span></span>        | <span data-ttu-id="009c7-135">说明</span><span class="sxs-lookup"><span data-stu-id="009c7-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="009c7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="009c7-136">displayName</span></span>|<span data-ttu-id="009c7-137">字符串</span><span class="sxs-lookup"><span data-stu-id="009c7-137">String</span></span>|<span data-ttu-id="009c7-138">PrintTaskDefinition 的名称。</span><span class="sxs-lookup"><span data-stu-id="009c7-138">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="009c7-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="009c7-139">createdBy</span></span>|<span data-ttu-id="009c7-140">String</span><span class="sxs-lookup"><span data-stu-id="009c7-140">String</span></span>|<span data-ttu-id="009c7-141">有关创建任务定义的应用程序的信息。</span><span class="sxs-lookup"><span data-stu-id="009c7-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="009c7-142">只有 `createdBy.displayName` 属性可以更新。</span><span class="sxs-lookup"><span data-stu-id="009c7-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="009c7-143">响应</span><span class="sxs-lookup"><span data-stu-id="009c7-143">Response</span></span>
<span data-ttu-id="009c7-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="009c7-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="009c7-146">示例</span><span class="sxs-lookup"><span data-stu-id="009c7-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="009c7-147">请求</span><span class="sxs-lookup"><span data-stu-id="009c7-147">Request</span></span>
<span data-ttu-id="009c7-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="009c7-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="009c7-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="009c7-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_update_taskdefinition"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="009c7-150">C#</span><span class="sxs-lookup"><span data-stu-id="009c7-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-update-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="009c7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="009c7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-update-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="009c7-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="009c7-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-update-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="009c7-153">响应</span><span class="sxs-lookup"><span data-stu-id="009c7-153">Response</span></span>
<span data-ttu-id="009c7-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="009c7-154">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
