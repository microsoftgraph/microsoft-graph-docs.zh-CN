---
title: 获取 taskDefinition
description: 获取有关任务定义的详细信息。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8105fa16971ed468e024291f97b529f2938df96c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091563"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="0fad7-103">获取 taskDefinition</span><span class="sxs-lookup"><span data-stu-id="0fad7-103">Get taskDefinition</span></span>

<span data-ttu-id="0fad7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fad7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fad7-105">获取有关任务定义的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0fad7-105">Get details about a task definition.</span></span>

<span data-ttu-id="0fad7-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="0fad7-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fad7-107">权限</span><span class="sxs-lookup"><span data-stu-id="0fad7-107">Permissions</span></span>
<span data-ttu-id="0fad7-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0fad7-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0fad7-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fad7-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0fad7-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="0fad7-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0fad7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fad7-111">Permission type</span></span> | <span data-ttu-id="0fad7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fad7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0fad7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fad7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0fad7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fad7-114">Not supported.</span></span> |
|<span data-ttu-id="0fad7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fad7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fad7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fad7-116">Not Supported.</span></span>|
|<span data-ttu-id="0fad7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fad7-117">Application</span></span>| <span data-ttu-id="0fad7-118">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="0fad7-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fad7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fad7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0fad7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fad7-120">Request headers</span></span>
| <span data-ttu-id="0fad7-121">名称</span><span class="sxs-lookup"><span data-stu-id="0fad7-121">Name</span></span>      |<span data-ttu-id="0fad7-122">说明</span><span class="sxs-lookup"><span data-stu-id="0fad7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0fad7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fad7-123">Authorization</span></span> | <span data-ttu-id="0fad7-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0fad7-124">Bearer {token}.</span></span> <span data-ttu-id="0fad7-125">Required.</span><span class="sxs-lookup"><span data-stu-id="0fad7-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fad7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fad7-126">Request body</span></span>
<span data-ttu-id="0fad7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0fad7-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0fad7-128">响应</span><span class="sxs-lookup"><span data-stu-id="0fad7-128">Response</span></span>
<span data-ttu-id="0fad7-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printTaskDefinition](../resources/printtaskdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0fad7-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fad7-130">示例</span><span class="sxs-lookup"><span data-stu-id="0fad7-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fad7-131">请求</span><span class="sxs-lookup"><span data-stu-id="0fad7-131">Request</span></span>
<span data-ttu-id="0fad7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0fad7-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```

---

### <a name="response"></a><span data-ttu-id="0fad7-133">响应</span><span class="sxs-lookup"><span data-stu-id="0fad7-133">Response</span></span>
<span data-ttu-id="0fad7-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0fad7-134">The following is an example of the response.</span></span>
><span data-ttu-id="0fad7-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0fad7-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0fad7-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0fad7-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 380

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
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
  "description": "Get taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
