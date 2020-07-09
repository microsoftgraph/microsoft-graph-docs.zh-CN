---
title: 更新 taskDefinition
description: 更新任务定义。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c0f0140b23291b77a5c00ff42b209f1f2af89a67
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091583"
---
# <a name="update-taskdefinition"></a><span data-ttu-id="6ecf6-103">更新 taskDefinition</span><span class="sxs-lookup"><span data-stu-id="6ecf6-103">Update taskDefinition</span></span>

<span data-ttu-id="6ecf6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ecf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ecf6-105">更新任务定义。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-105">Update a task definition.</span></span>

<span data-ttu-id="6ecf6-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ecf6-107">权限</span><span class="sxs-lookup"><span data-stu-id="6ecf6-107">Permissions</span></span>
<span data-ttu-id="6ecf6-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6ecf6-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6ecf6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecf6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6ecf6-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="6ecf6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ecf6-111">Permission type</span></span> | <span data-ttu-id="6ecf6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ecf6-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6ecf6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ecf6-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6ecf6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-114">Not supported.</span></span> |
|<span data-ttu-id="6ecf6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ecf6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ecf6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-116">Not Supported.</span></span>|
|<span data-ttu-id="6ecf6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ecf6-117">Application</span></span>| <span data-ttu-id="6ecf6-118">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6ecf6-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ecf6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ecf6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6ecf6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ecf6-120">Request headers</span></span>
| <span data-ttu-id="6ecf6-121">名称</span><span class="sxs-lookup"><span data-stu-id="6ecf6-121">Name</span></span>      |<span data-ttu-id="6ecf6-122">说明</span><span class="sxs-lookup"><span data-stu-id="6ecf6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ecf6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ecf6-123">Authorization</span></span> | <span data-ttu-id="6ecf6-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6ecf6-124">Bearer {token}.</span></span> <span data-ttu-id="6ecf6-125">Required.</span><span class="sxs-lookup"><span data-stu-id="6ecf6-125">Required.</span></span> |
| <span data-ttu-id="6ecf6-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="6ecf6-126">Content-type</span></span>  | <span data-ttu-id="6ecf6-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="6ecf6-127">application/json.</span></span> <span data-ttu-id="6ecf6-128">Required.</span><span class="sxs-lookup"><span data-stu-id="6ecf6-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ecf6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ecf6-129">Request body</span></span>
<span data-ttu-id="6ecf6-130">在请求正文中，提供应更新的相关[printTaskDefinition](../resources/printtaskdefinition.md)字段的值。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="6ecf6-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6ecf6-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6ecf6-133">属性</span><span class="sxs-lookup"><span data-stu-id="6ecf6-133">Property</span></span>     | <span data-ttu-id="6ecf6-134">类型</span><span class="sxs-lookup"><span data-stu-id="6ecf6-134">Type</span></span>        | <span data-ttu-id="6ecf6-135">说明</span><span class="sxs-lookup"><span data-stu-id="6ecf6-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6ecf6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6ecf6-136">displayName</span></span>|<span data-ttu-id="6ecf6-137">String</span><span class="sxs-lookup"><span data-stu-id="6ecf6-137">String</span></span>|<span data-ttu-id="6ecf6-138">PrintTaskDefinition 的名称。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-138">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="6ecf6-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="6ecf6-139">createdBy</span></span>|<span data-ttu-id="6ecf6-140">String</span><span class="sxs-lookup"><span data-stu-id="6ecf6-140">String</span></span>|<span data-ttu-id="6ecf6-141">有关创建任务定义的应用程序的信息。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="6ecf6-142">只有 `createdBy.displayName` 属性可以更新。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="6ecf6-143">响应</span><span class="sxs-lookup"><span data-stu-id="6ecf6-143">Response</span></span>
<span data-ttu-id="6ecf6-144">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="6ecf6-144">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="6ecf6-145">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="6ecf6-145">It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ecf6-146">示例</span><span class="sxs-lookup"><span data-stu-id="6ecf6-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ecf6-147">请求</span><span class="sxs-lookup"><span data-stu-id="6ecf6-147">Request</span></span>
<span data-ttu-id="6ecf6-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-148">The following is an example of the request.</span></span>

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

---

### <a name="response"></a><span data-ttu-id="6ecf6-149">响应</span><span class="sxs-lookup"><span data-stu-id="6ecf6-149">Response</span></span>
<span data-ttu-id="6ecf6-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6ecf6-150">The following is an example of the response.</span></span>
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
