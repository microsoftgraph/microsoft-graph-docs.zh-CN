---
title: 列出 taskDefinitions
description: 检索在租户中定义的请求应用程序的任务定义列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 91d00b7773b56d4c5f522981c7a59dde3744a710
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091585"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="29695-103">列出 taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="29695-103">List taskDefinitions</span></span>

<span data-ttu-id="29695-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29695-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29695-105">检索在租户中定义的请求应用程序的[任务定义](../resources/printtaskdefinition.md)列表。</span><span class="sxs-lookup"><span data-stu-id="29695-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="29695-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="29695-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="29695-107">权限</span><span class="sxs-lookup"><span data-stu-id="29695-107">Permissions</span></span>
<span data-ttu-id="29695-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="29695-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="29695-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="29695-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29695-111">Permission type</span></span> | <span data-ttu-id="29695-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29695-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="29695-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29695-113">Delegated (work or school account)</span></span>| <span data-ttu-id="29695-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="29695-114">Not supported.</span></span> |
|<span data-ttu-id="29695-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29695-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29695-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29695-116">Not Supported.</span></span>|
|<span data-ttu-id="29695-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29695-117">Application</span></span>| <span data-ttu-id="29695-118">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="29695-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29695-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29695-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29695-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="29695-120">Optional query parameters</span></span>
<span data-ttu-id="29695-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="29695-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="29695-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="29695-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="29695-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="29695-123">Exceptions</span></span>
<span data-ttu-id="29695-124">某些运算符不受支持：、、、、 `$count` `$format` `$search` `$select` `$skip` 、 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="29695-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29695-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="29695-125">Request headers</span></span>
| <span data-ttu-id="29695-126">名称</span><span class="sxs-lookup"><span data-stu-id="29695-126">Name</span></span>      |<span data-ttu-id="29695-127">说明</span><span class="sxs-lookup"><span data-stu-id="29695-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="29695-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="29695-128">Authorization</span></span> | <span data-ttu-id="29695-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29695-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29695-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="29695-131">Request body</span></span>
<span data-ttu-id="29695-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29695-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="29695-133">响应</span><span class="sxs-lookup"><span data-stu-id="29695-133">Response</span></span>
<span data-ttu-id="29695-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printTaskDefinition](../resources/printtaskdefinition.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="29695-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29695-135">示例</span><span class="sxs-lookup"><span data-stu-id="29695-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="29695-136">请求</span><span class="sxs-lookup"><span data-stu-id="29695-136">Request</span></span>
<span data-ttu-id="29695-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="29695-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```

---

### <a name="response"></a><span data-ttu-id="29695-138">响应</span><span class="sxs-lookup"><span data-stu-id="29695-138">Response</span></span>
<span data-ttu-id="29695-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="29695-139">The following is an example of the response.</span></span>
><span data-ttu-id="29695-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="29695-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions",
  "value": [
    {
      "id": "fab143fd-ee61-4358-8558-2c7dee953982",
      "displayName": "Test TaskDefinitionName",
      "createdBy": {
        "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
        "displayName": "Requesting App Display Name"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
