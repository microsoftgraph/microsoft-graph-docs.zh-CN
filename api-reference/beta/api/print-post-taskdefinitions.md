---
title: 创建 taskDefinition
description: 创建新的任务定义。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 147e1271ee0f5bcd7c04e167e172c48939a4da98
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091582"
---
# <a name="create-taskdefinition"></a><span data-ttu-id="3e696-103">创建 taskDefinition</span><span class="sxs-lookup"><span data-stu-id="3e696-103">Create taskDefinition</span></span>

<span data-ttu-id="3e696-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e696-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e696-105">创建新的任务定义。</span><span class="sxs-lookup"><span data-stu-id="3e696-105">Create a new task definition.</span></span>

<span data-ttu-id="3e696-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="3e696-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e696-107">权限</span><span class="sxs-lookup"><span data-stu-id="3e696-107">Permissions</span></span>
<span data-ttu-id="3e696-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3e696-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="3e696-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3e696-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e696-111">Permission type</span></span> | <span data-ttu-id="3e696-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e696-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3e696-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e696-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3e696-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e696-114">Not supported.</span></span> |
|<span data-ttu-id="3e696-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e696-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e696-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e696-116">Not Supported.</span></span>|
|<span data-ttu-id="3e696-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e696-117">Application</span></span>| <span data-ttu-id="3e696-118">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="3e696-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e696-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e696-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3e696-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e696-120">Request headers</span></span>
| <span data-ttu-id="3e696-121">名称</span><span class="sxs-lookup"><span data-stu-id="3e696-121">Name</span></span>      |<span data-ttu-id="3e696-122">说明</span><span class="sxs-lookup"><span data-stu-id="3e696-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e696-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e696-123">Authorization</span></span> | <span data-ttu-id="3e696-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e696-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e696-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3e696-126">Content-type</span></span>  | <span data-ttu-id="3e696-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3e696-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e696-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e696-129">Request body</span></span>
<span data-ttu-id="3e696-130">在请求正文中，提供[printTaskDefinition](../resources/printtaskdefinition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e696-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="3e696-131">[PrintTaskDefinition](../resources/printtaskdefinition.md)的**id**和**createdBy**属性是在创建资源时自动设置的。</span><span class="sxs-lookup"><span data-stu-id="3e696-131">The [printTaskDefinition](../resources/printtaskdefinition.md)'s **id** and **createdBy.appId** properties are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="3e696-132">响应</span><span class="sxs-lookup"><span data-stu-id="3e696-132">Response</span></span>
<span data-ttu-id="3e696-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[printTaskDefinition](../resources/printtaskdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3e696-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e696-134">示例</span><span class="sxs-lookup"><span data-stu-id="3e696-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e696-135">请求</span><span class="sxs-lookup"><span data-stu-id="3e696-135">Request</span></span>
<span data-ttu-id="3e696-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e696-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "print_create_taskdefinition"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/print/taskDefinitions
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

### <a name="response"></a><span data-ttu-id="3e696-137">响应</span><span class="sxs-lookup"><span data-stu-id="3e696-137">Response</span></span>
<span data-ttu-id="3e696-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e696-138">The following is an example of the response.</span></span>
><span data-ttu-id="3e696-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3e696-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 322

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
