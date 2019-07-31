---
title: 'educationSubmission: 撤回'
description: '指示学生想要参加提交。 仅学生可以执行此操作。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d37d34685aabe00bff82de453e68a8ebba36aa3a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955073"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="cd30f-104">educationSubmission: 撤回</span><span class="sxs-lookup"><span data-stu-id="cd30f-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd30f-105">指示学生想要参加提交。</span><span class="sxs-lookup"><span data-stu-id="cd30f-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="cd30f-106">仅学生可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="cd30f-106">This action can only be done by a student.</span></span> <span data-ttu-id="cd30f-107">它会将提交的状态从 "已提交" 更改为 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="cd30f-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="cd30f-108">权限</span><span class="sxs-lookup"><span data-stu-id="cd30f-108">Permissions</span></span>

<span data-ttu-id="cd30f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd30f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd30f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd30f-111">Permission type</span></span>                        | <span data-ttu-id="cd30f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd30f-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="cd30f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd30f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd30f-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="cd30f-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="cd30f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd30f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd30f-116">不支持</span><span class="sxs-lookup"><span data-stu-id="cd30f-116">Not supported</span></span>                                           |
| <span data-ttu-id="cd30f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd30f-117">Application</span></span>                            | <span data-ttu-id="cd30f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd30f-118">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="cd30f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd30f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/recall
```

## <a name="request-headers"></a><span data-ttu-id="cd30f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd30f-120">Request headers</span></span>

| <span data-ttu-id="cd30f-121">标头</span><span class="sxs-lookup"><span data-stu-id="cd30f-121">Header</span></span>        | <span data-ttu-id="cd30f-122">值</span><span class="sxs-lookup"><span data-stu-id="cd30f-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="cd30f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd30f-123">Authorization</span></span> | <span data-ttu-id="cd30f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd30f-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cd30f-126">响应</span><span class="sxs-lookup"><span data-stu-id="cd30f-126">Response</span></span>

<span data-ttu-id="cd30f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cd30f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd30f-129">示例</span><span class="sxs-lookup"><span data-stu-id="cd30f-129">Example</span></span>

<span data-ttu-id="cd30f-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="cd30f-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cd30f-131">请求</span><span class="sxs-lookup"><span data-stu-id="cd30f-131">Request</span></span>

<span data-ttu-id="cd30f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cd30f-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="cd30f-133">响应</span><span class="sxs-lookup"><span data-stu-id="cd30f-133">Response</span></span>

<span data-ttu-id="cd30f-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cd30f-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
