---
title: 删除 educationAssignment
description: 删除现有工作分配。 只有班级内的教师才能删除作业。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ff82696996c9731209b448245515011e2f9baf2a
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911420"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="67d94-104">删除 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="67d94-104">Delete educationAssignment</span></span>

<span data-ttu-id="67d94-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67d94-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67d94-106">删除现有工作分配。</span><span class="sxs-lookup"><span data-stu-id="67d94-106">Delete an existing assignment.</span></span> 

<span data-ttu-id="67d94-107">只有班级内的教师才能删除作业。</span><span class="sxs-lookup"><span data-stu-id="67d94-107">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="67d94-108">权限</span><span class="sxs-lookup"><span data-stu-id="67d94-108">Permissions</span></span>

<span data-ttu-id="67d94-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67d94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67d94-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="67d94-111">Permission type</span></span>                        | <span data-ttu-id="67d94-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67d94-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="67d94-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67d94-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="67d94-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67d94-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="67d94-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67d94-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67d94-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67d94-116">Not Supported.</span></span>                                          |
| <span data-ttu-id="67d94-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="67d94-117">Application</span></span>                            | <span data-ttu-id="67d94-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="67d94-118">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="67d94-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67d94-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```

## <a name="request-headers"></a><span data-ttu-id="67d94-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="67d94-120">Request headers</span></span>

| <span data-ttu-id="67d94-121">标头</span><span class="sxs-lookup"><span data-stu-id="67d94-121">Header</span></span>        | <span data-ttu-id="67d94-122">值</span><span class="sxs-lookup"><span data-stu-id="67d94-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="67d94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67d94-123">Authorization</span></span> | <span data-ttu-id="67d94-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67d94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67d94-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="67d94-126">Request body</span></span>

<span data-ttu-id="67d94-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67d94-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67d94-128">响应</span><span class="sxs-lookup"><span data-stu-id="67d94-128">Response</span></span>

<span data-ttu-id="67d94-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="67d94-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67d94-131">示例</span><span class="sxs-lookup"><span data-stu-id="67d94-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="67d94-132">请求</span><span class="sxs-lookup"><span data-stu-id="67d94-132">Request</span></span>

<span data-ttu-id="67d94-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67d94-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "delete_educationassignment_1"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
```

### <a name="response"></a><span data-ttu-id="67d94-134">响应</span><span class="sxs-lookup"><span data-stu-id="67d94-134">Response</span></span>
<span data-ttu-id="67d94-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67d94-135">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


