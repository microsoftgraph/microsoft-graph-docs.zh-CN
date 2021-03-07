---
title: 更新 printTaskDefinition
description: 更新任务定义。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 98f075e89828a1e07fe3ee04bbed0b95b511b0d5
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517001"
---
# <a name="update-printtaskdefinition"></a><span data-ttu-id="396b0-103">更新 printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="396b0-103">Update printTaskDefinition</span></span>

<span data-ttu-id="396b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="396b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="396b0-105">更新任务定义。</span><span class="sxs-lookup"><span data-stu-id="396b0-105">Update a task definition.</span></span>

<span data-ttu-id="396b0-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="396b0-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="396b0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="396b0-107">Permissions</span></span>
<span data-ttu-id="396b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="396b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="396b0-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="396b0-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="396b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="396b0-111">Permission type</span></span> | <span data-ttu-id="396b0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="396b0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="396b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="396b0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="396b0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="396b0-114">Not supported.</span></span> |
|<span data-ttu-id="396b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="396b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="396b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="396b0-116">Not Supported.</span></span>|
|<span data-ttu-id="396b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="396b0-117">Application</span></span>| <span data-ttu-id="396b0-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="396b0-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="396b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="396b0-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="396b0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="396b0-120">Request headers</span></span>
|<span data-ttu-id="396b0-121">名称</span><span class="sxs-lookup"><span data-stu-id="396b0-121">Name</span></span>|<span data-ttu-id="396b0-122">说明</span><span class="sxs-lookup"><span data-stu-id="396b0-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="396b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="396b0-123">Authorization</span></span>|<span data-ttu-id="396b0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="396b0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="396b0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="396b0-126">Content-Type</span></span>|<span data-ttu-id="396b0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="396b0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="396b0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="396b0-129">Request body</span></span>
<span data-ttu-id="396b0-130">在请求正文中，提供应更新的相关 [printTaskDefinition](../resources/printtaskdefinition.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="396b0-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="396b0-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="396b0-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="396b0-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="396b0-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="396b0-133">属性</span><span class="sxs-lookup"><span data-stu-id="396b0-133">Property</span></span>     | <span data-ttu-id="396b0-134">类型</span><span class="sxs-lookup"><span data-stu-id="396b0-134">Type</span></span>        | <span data-ttu-id="396b0-135">说明</span><span class="sxs-lookup"><span data-stu-id="396b0-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="396b0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="396b0-136">displayName</span></span>|<span data-ttu-id="396b0-137">String</span><span class="sxs-lookup"><span data-stu-id="396b0-137">String</span></span>|<span data-ttu-id="396b0-138">**printTaskDefinition 的名称**。</span><span class="sxs-lookup"><span data-stu-id="396b0-138">The name of the **printTaskDefinition**.</span></span>|
|<span data-ttu-id="396b0-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="396b0-139">createdBy</span></span>|<span data-ttu-id="396b0-140">String</span><span class="sxs-lookup"><span data-stu-id="396b0-140">String</span></span>|<span data-ttu-id="396b0-141">有关创建任务定义的应用的信息。</span><span class="sxs-lookup"><span data-stu-id="396b0-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="396b0-142">只能 `createdBy.displayName` 更新属性。</span><span class="sxs-lookup"><span data-stu-id="396b0-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="396b0-143">响应</span><span class="sxs-lookup"><span data-stu-id="396b0-143">Response</span></span>

<span data-ttu-id="396b0-144">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="396b0-144">If successful, this method returns a `200 OK` response code and an updated [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="396b0-145">示例</span><span class="sxs-lookup"><span data-stu-id="396b0-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="396b0-146">请求</span><span class="sxs-lookup"><span data-stu-id="396b0-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printtaskdefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
Content-Type: application/json
Content-length: 163

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```

### <a name="response"></a><span data-ttu-id="396b0-147">响应</span><span class="sxs-lookup"><span data-stu-id="396b0-147">Response</span></span>
<span data-ttu-id="396b0-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="396b0-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId" : "479688a0-cc3a-4993-ab24-54c7c80b047e",
    "displayName": "Requesting App Display Name"
  }
}
```

