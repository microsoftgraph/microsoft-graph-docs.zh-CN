---
title: 删除 taskDefinition
description: 删除任务定义。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23d7438d573cb0ac8ff17c0a9c100bece71bb68c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091648"
---
# <a name="delete-taskdefinition"></a><span data-ttu-id="da1bf-103">删除 taskDefinition</span><span class="sxs-lookup"><span data-stu-id="da1bf-103">Delete taskDefinition</span></span>

<span data-ttu-id="da1bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da1bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da1bf-105">删除**taskDefinition**。</span><span class="sxs-lookup"><span data-stu-id="da1bf-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="da1bf-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="da1bf-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="da1bf-107">权限</span><span class="sxs-lookup"><span data-stu-id="da1bf-107">Permissions</span></span>
<span data-ttu-id="da1bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da1bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="da1bf-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="da1bf-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="da1bf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da1bf-111">Permission type</span></span> | <span data-ttu-id="da1bf-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da1bf-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="da1bf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da1bf-113">Delegated (work or school account)</span></span>| <span data-ttu-id="da1bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="da1bf-114">Not supported.</span></span> |
|<span data-ttu-id="da1bf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da1bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da1bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da1bf-116">Not Supported.</span></span>|
|<span data-ttu-id="da1bf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da1bf-117">Application</span></span>| <span data-ttu-id="da1bf-118">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="da1bf-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da1bf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da1bf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/taskDefinitions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="da1bf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da1bf-120">Request headers</span></span>
| <span data-ttu-id="da1bf-121">名称</span><span class="sxs-lookup"><span data-stu-id="da1bf-121">Name</span></span>          | <span data-ttu-id="da1bf-122">说明</span><span class="sxs-lookup"><span data-stu-id="da1bf-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="da1bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da1bf-123">Authorization</span></span> | <span data-ttu-id="da1bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da1bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da1bf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da1bf-126">Request body</span></span>
<span data-ttu-id="da1bf-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da1bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da1bf-128">响应</span><span class="sxs-lookup"><span data-stu-id="da1bf-128">Response</span></span>
<span data-ttu-id="da1bf-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="da1bf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da1bf-131">示例</span><span class="sxs-lookup"><span data-stu-id="da1bf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="da1bf-132">请求</span><span class="sxs-lookup"><span data-stu-id="da1bf-132">Request</span></span>
<span data-ttu-id="da1bf-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da1bf-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_taskdefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19
```

---

### <a name="response"></a><span data-ttu-id="da1bf-134">响应</span><span class="sxs-lookup"><span data-stu-id="da1bf-134">Response</span></span>
<span data-ttu-id="da1bf-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da1bf-135">The following is an example of the response.</span></span>
><span data-ttu-id="da1bf-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="da1bf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
