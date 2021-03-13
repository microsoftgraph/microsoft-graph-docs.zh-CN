---
title: 创建 printTaskDefinition
description: 创建新的任务定义。
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ee7172c76863cb62a24c44ba73de2f02bb27e30c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772210"
---
# <a name="create-printtaskdefinition"></a><span data-ttu-id="9d7da-103">创建 printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="9d7da-103">Create printTaskDefinition</span></span>
<span data-ttu-id="9d7da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d7da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="9d7da-105">创建新的任务定义。</span><span class="sxs-lookup"><span data-stu-id="9d7da-105">Create a new task definition.</span></span>

<span data-ttu-id="9d7da-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="9d7da-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d7da-107">权限</span><span class="sxs-lookup"><span data-stu-id="9d7da-107">Permissions</span></span>
<span data-ttu-id="9d7da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d7da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9d7da-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9d7da-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9d7da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d7da-111">Permission type</span></span> | <span data-ttu-id="9d7da-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d7da-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9d7da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d7da-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9d7da-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d7da-114">Not supported.</span></span> |
|<span data-ttu-id="9d7da-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d7da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d7da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d7da-116">Not Supported.</span></span>|
|<span data-ttu-id="9d7da-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d7da-117">Application</span></span>| <span data-ttu-id="9d7da-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d7da-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d7da-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d7da-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="9d7da-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d7da-120">Request headers</span></span>
|<span data-ttu-id="9d7da-121">名称</span><span class="sxs-lookup"><span data-stu-id="9d7da-121">Name</span></span>|<span data-ttu-id="9d7da-122">说明</span><span class="sxs-lookup"><span data-stu-id="9d7da-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9d7da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d7da-123">Authorization</span></span>|<span data-ttu-id="9d7da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d7da-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9d7da-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d7da-126">Content-Type</span></span>|<span data-ttu-id="9d7da-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9d7da-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d7da-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d7da-129">Request body</span></span>
<span data-ttu-id="9d7da-130">在请求正文中，提供 [printTaskDefinition](../resources/printtaskdefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d7da-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="9d7da-131">[printTaskDefinition](../resources/printtaskdefinition.md)对象的 **id** 和 **createdBy.appId** 属性会在创建资源时自动设置。</span><span class="sxs-lookup"><span data-stu-id="9d7da-131">The **id** and **createdBy.appId** properties of the [printTaskDefinition](../resources/printtaskdefinition.md) object are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="9d7da-132">响应</span><span class="sxs-lookup"><span data-stu-id="9d7da-132">Response</span></span>

<span data-ttu-id="9d7da-133">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [printTaskDefinition](../resources/printtaskdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d7da-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d7da-134">示例</span><span class="sxs-lookup"><span data-stu-id="9d7da-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d7da-135">请求</span><span class="sxs-lookup"><span data-stu-id="9d7da-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9d7da-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d7da-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printtaskdefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/taskDefinitions
Content-Type: application/json
Content-length: 163

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9d7da-137">C#</span><span class="sxs-lookup"><span data-stu-id="9d7da-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printtaskdefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d7da-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d7da-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printtaskdefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d7da-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d7da-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printtaskdefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d7da-140">Java</span><span class="sxs-lookup"><span data-stu-id="9d7da-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printtaskdefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9d7da-141">响应</span><span class="sxs-lookup"><span data-stu-id="9d7da-141">Response</span></span>
<span data-ttu-id="9d7da-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9d7da-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

