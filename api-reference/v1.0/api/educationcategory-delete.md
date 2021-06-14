---
title: 删除 educationCategory
description: 删除现有类别。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eed94985bfa1de66215f7afd1ca64d236846a118
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911413"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="052b3-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="052b3-103">Delete educationCategory</span></span>

<span data-ttu-id="052b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="052b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="052b3-105">删除现有 [类别](../resources/educationcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="052b3-105">Delete an existing [category](../resources/educationcategory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="052b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="052b3-106">Permissions</span></span>

<span data-ttu-id="052b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="052b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="052b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="052b3-109">Permission type</span></span>                        | <span data-ttu-id="052b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="052b3-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="052b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="052b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="052b3-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="052b3-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="052b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="052b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="052b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="052b3-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="052b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="052b3-115">Application</span></span>                            | <span data-ttu-id="052b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="052b3-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="052b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="052b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="052b3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="052b3-118">Request headers</span></span>

| <span data-ttu-id="052b3-119">标头</span><span class="sxs-lookup"><span data-stu-id="052b3-119">Header</span></span>        | <span data-ttu-id="052b3-120">值</span><span class="sxs-lookup"><span data-stu-id="052b3-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="052b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="052b3-121">Authorization</span></span> | <span data-ttu-id="052b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="052b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="052b3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="052b3-124">Request body</span></span>

<span data-ttu-id="052b3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="052b3-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="052b3-126">响应</span><span class="sxs-lookup"><span data-stu-id="052b3-126">Response</span></span>

<span data-ttu-id="052b3-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="052b3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="052b3-129">示例</span><span class="sxs-lookup"><span data-stu-id="052b3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="052b3-130">请求</span><span class="sxs-lookup"><span data-stu-id="052b3-130">Request</span></span>

<span data-ttu-id="052b3-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="052b3-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignmentCategories/b93d3b6b-360c-45c0-8764-e8bb622a9504
```

### <a name="response"></a><span data-ttu-id="052b3-132">响应</span><span class="sxs-lookup"><span data-stu-id="052b3-132">Response</span></span>

<span data-ttu-id="052b3-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="052b3-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


