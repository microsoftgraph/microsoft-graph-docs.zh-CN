---
title: 删除 educationRubric
description: 删除 educationRubric 对象。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0b488c7c3307a7ac2388d36861eb4895fec44484
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912345"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="1dd09-103">删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="1dd09-103">Delete educationRubric</span></span>

<span data-ttu-id="1dd09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd09-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1dd09-105">删除 [educationRubric](../resources/educationrubric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dd09-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd09-106">权限</span><span class="sxs-lookup"><span data-stu-id="1dd09-106">Permissions</span></span>

<span data-ttu-id="1dd09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1dd09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dd09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dd09-109">Permission type</span></span>                        | <span data-ttu-id="1dd09-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1dd09-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1dd09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dd09-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dd09-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dd09-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1dd09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dd09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dd09-114">Not supported.</span></span> |
| <span data-ttu-id="1dd09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1dd09-115">Application</span></span>                            | <span data-ttu-id="1dd09-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dd09-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd09-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dd09-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

## <a name="request-headers"></a><span data-ttu-id="1dd09-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dd09-118">Request headers</span></span>

| <span data-ttu-id="1dd09-119">名称</span><span class="sxs-lookup"><span data-stu-id="1dd09-119">Name</span></span>          | <span data-ttu-id="1dd09-120">说明</span><span class="sxs-lookup"><span data-stu-id="1dd09-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1dd09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dd09-121">Authorization</span></span> | <span data-ttu-id="1dd09-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1dd09-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dd09-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dd09-123">Request body</span></span>

<span data-ttu-id="1dd09-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1dd09-124">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dd09-125">响应</span><span class="sxs-lookup"><span data-stu-id="1dd09-125">Response</span></span>

<span data-ttu-id="1dd09-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1dd09-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1dd09-128">示例</span><span class="sxs-lookup"><span data-stu-id="1dd09-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1dd09-129">请求</span><span class="sxs-lookup"><span data-stu-id="1dd09-129">Request</span></span>

<span data-ttu-id="1dd09-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1dd09-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

### <a name="response"></a><span data-ttu-id="1dd09-131">响应</span><span class="sxs-lookup"><span data-stu-id="1dd09-131">Response</span></span>

<span data-ttu-id="1dd09-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1dd09-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


