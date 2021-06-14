---
title: 从 educationAssignment 中删除 educationRubric
description: 从 educationAssignment 中删除 educationRubric
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9ce6eb7090c75fab942fc9cd5e317b5526a6dd7b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912348"
---
# <a name="delete-educationrubric-from-educationassignment"></a><span data-ttu-id="ab57b-103">从 educationAssignment 中删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="ab57b-103">Delete educationRubric from educationAssignment</span></span>

<span data-ttu-id="ab57b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab57b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab57b-105">从[educationAssignment](../resources/educationassignment.md)中删除[educationRubric。](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="ab57b-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>
<span data-ttu-id="ab57b-106">此方法不会删除测试点本身。</span><span class="sxs-lookup"><span data-stu-id="ab57b-106">This method does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab57b-107">权限</span><span class="sxs-lookup"><span data-stu-id="ab57b-107">Permissions</span></span>

<span data-ttu-id="ab57b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab57b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab57b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab57b-110">Permission type</span></span>                        | <span data-ttu-id="ab57b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab57b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab57b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab57b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab57b-113">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab57b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="ab57b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab57b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab57b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab57b-115">Not supported.</span></span> |
| <span data-ttu-id="ab57b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab57b-116">Application</span></span>                            | <span data-ttu-id="ab57b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab57b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab57b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab57b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ab57b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab57b-119">Request headers</span></span>

| <span data-ttu-id="ab57b-120">名称</span><span class="sxs-lookup"><span data-stu-id="ab57b-120">Name</span></span>          | <span data-ttu-id="ab57b-121">说明</span><span class="sxs-lookup"><span data-stu-id="ab57b-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ab57b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab57b-122">Authorization</span></span> | <span data-ttu-id="ab57b-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ab57b-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab57b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab57b-124">Request body</span></span>

<span data-ttu-id="ab57b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab57b-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab57b-126">响应</span><span class="sxs-lookup"><span data-stu-id="ab57b-126">Response</span></span>

<span data-ttu-id="ab57b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ab57b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab57b-129">示例</span><span class="sxs-lookup"><span data-stu-id="ab57b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab57b-130">请求</span><span class="sxs-lookup"><span data-stu-id="ab57b-130">Request</span></span>

<span data-ttu-id="ab57b-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab57b-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

### <a name="response"></a><span data-ttu-id="ab57b-132">响应</span><span class="sxs-lookup"><span data-stu-id="ab57b-132">Response</span></span>

<span data-ttu-id="ab57b-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab57b-133">The following is an example of the response.</span></span>

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


