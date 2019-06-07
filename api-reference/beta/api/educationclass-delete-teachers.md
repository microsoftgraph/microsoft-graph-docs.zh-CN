---
title: 删除 teacher
description: 从课程中删除教师。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 35151136f38bcf1e74d958f3f48f4e6819ab73cf
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750015"
---
# <a name="remove-teacher"></a><span data-ttu-id="d47b7-103">删除 teacher</span><span class="sxs-lookup"><span data-stu-id="d47b7-103">Remove teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d47b7-104">从课程中删除教师。</span><span class="sxs-lookup"><span data-stu-id="d47b7-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="d47b7-105">权限</span><span class="sxs-lookup"><span data-stu-id="d47b7-105">Permissions</span></span>

<span data-ttu-id="d47b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d47b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d47b7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d47b7-108">Permission type</span></span>                        | <span data-ttu-id="d47b7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d47b7-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d47b7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d47b7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d47b7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="d47b7-111">Not supported.</span></span>                              |
| <span data-ttu-id="d47b7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d47b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d47b7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d47b7-113">Not supported.</span></span>                              |
| <span data-ttu-id="d47b7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d47b7-114">Application</span></span>                            | <span data-ttu-id="d47b7-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47b7-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="d47b7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d47b7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d47b7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d47b7-117">Request headers</span></span>

| <span data-ttu-id="d47b7-118">标头</span><span class="sxs-lookup"><span data-stu-id="d47b7-118">Header</span></span>        | <span data-ttu-id="d47b7-119">值</span><span class="sxs-lookup"><span data-stu-id="d47b7-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d47b7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d47b7-120">Authorization</span></span> | <span data-ttu-id="d47b7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d47b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d47b7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d47b7-123">Request body</span></span>

<span data-ttu-id="d47b7-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d47b7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d47b7-125">响应</span><span class="sxs-lookup"><span data-stu-id="d47b7-125">Response</span></span>

<span data-ttu-id="d47b7-126">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="d47b7-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="d47b7-127">示例</span><span class="sxs-lookup"><span data-stu-id="d47b7-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d47b7-128">请求</span><span class="sxs-lookup"><span data-stu-id="d47b7-128">Request</span></span>

<span data-ttu-id="d47b7-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d47b7-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/teachers/14012
```

##### <a name="response"></a><span data-ttu-id="d47b7-130">响应</span><span class="sxs-lookup"><span data-stu-id="d47b7-130">Response</span></span>

<span data-ttu-id="d47b7-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d47b7-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
