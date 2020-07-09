---
title: 获取任务
description: 获取有关打印任务的详细信息。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c9dcb0d872c5fc7c54877f9b43333778fe411ba7
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091568"
---
# <a name="get-task"></a><span data-ttu-id="f588f-103">获取任务</span><span class="sxs-lookup"><span data-stu-id="f588f-103">Get task</span></span>

<span data-ttu-id="f588f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f588f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f588f-105">获取有关打印任务的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f588f-105">Get details about a print task.</span></span>

<span data-ttu-id="f588f-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="f588f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f588f-107">权限</span><span class="sxs-lookup"><span data-stu-id="f588f-107">Permissions</span></span>
<span data-ttu-id="f588f-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f588f-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f588f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f588f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f588f-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="f588f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f588f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f588f-111">Permission type</span></span> | <span data-ttu-id="f588f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f588f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f588f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f588f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f588f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f588f-114">Not supported.</span></span> |
|<span data-ttu-id="f588f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f588f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f588f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f588f-116">Not Supported.</span></span>|
|<span data-ttu-id="f588f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f588f-117">Application</span></span>| <span data-ttu-id="f588f-118">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="f588f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f588f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f588f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f588f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f588f-120">Request headers</span></span>
| <span data-ttu-id="f588f-121">名称</span><span class="sxs-lookup"><span data-stu-id="f588f-121">Name</span></span>      |<span data-ttu-id="f588f-122">说明</span><span class="sxs-lookup"><span data-stu-id="f588f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f588f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f588f-123">Authorization</span></span> | <span data-ttu-id="f588f-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f588f-124">Bearer {token}.</span></span> <span data-ttu-id="f588f-125">Required.</span><span class="sxs-lookup"><span data-stu-id="f588f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f588f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f588f-126">Request body</span></span>
<span data-ttu-id="f588f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f588f-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f588f-128">响应</span><span class="sxs-lookup"><span data-stu-id="f588f-128">Response</span></span>
<span data-ttu-id="f588f-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printTask](../resources/printtask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f588f-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f588f-130">示例</span><span class="sxs-lookup"><span data-stu-id="f588f-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="f588f-131">请求</span><span class="sxs-lookup"><span data-stu-id="f588f-131">Request</span></span>
<span data-ttu-id="f588f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f588f-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_task"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3
```

---

### <a name="response"></a><span data-ttu-id="f588f-133">响应</span><span class="sxs-lookup"><span data-stu-id="f588f-133">Response</span></span>
<span data-ttu-id="f588f-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f588f-134">The following is an example of the response.</span></span>
><span data-ttu-id="f588f-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="f588f-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f588f-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f588f-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 392

{

  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions('3203656e-6069-4e10-8147-d25290b00a3c')/tasks/$entity",
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
