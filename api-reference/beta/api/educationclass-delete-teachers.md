---
title: 删除 teacher
description: 从课程中删除教师。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3eedc8905fb9cb902311fcd218d2df7330362116
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324724"
---
# <a name="remove-teacher"></a><span data-ttu-id="99e7c-103">删除 teacher</span><span class="sxs-lookup"><span data-stu-id="99e7c-103">Remove teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99e7c-104">从课程中删除教师。</span><span class="sxs-lookup"><span data-stu-id="99e7c-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="99e7c-105">权限</span><span class="sxs-lookup"><span data-stu-id="99e7c-105">Permissions</span></span>
<span data-ttu-id="99e7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99e7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99e7c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="99e7c-108">Permission type</span></span>      | <span data-ttu-id="99e7c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99e7c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99e7c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99e7c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="99e7c-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="99e7c-111">Not supported.</span></span>  |
|<span data-ttu-id="99e7c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99e7c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="99e7c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="99e7c-113">Not supported.</span></span>  |
|<span data-ttu-id="99e7c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="99e7c-114">Application</span></span> | <span data-ttu-id="99e7c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e7c-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="99e7c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99e7c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="99e7c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="99e7c-117">Request headers</span></span>
| <span data-ttu-id="99e7c-118">标头</span><span class="sxs-lookup"><span data-stu-id="99e7c-118">Header</span></span>       | <span data-ttu-id="99e7c-119">值</span><span class="sxs-lookup"><span data-stu-id="99e7c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99e7c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e7c-120">Authorization</span></span>  | <span data-ttu-id="99e7c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99e7c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99e7c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="99e7c-123">Request body</span></span>
<span data-ttu-id="99e7c-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99e7c-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="99e7c-125">响应</span><span class="sxs-lookup"><span data-stu-id="99e7c-125">Response</span></span>
<span data-ttu-id="99e7c-126">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="99e7c-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e7c-127">示例</span><span class="sxs-lookup"><span data-stu-id="99e7c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99e7c-128">请求</span><span class="sxs-lookup"><span data-stu-id="99e7c-128">Request</span></span>
<span data-ttu-id="99e7c-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99e7c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/<id>/teachers/14012
```

##### <a name="response"></a><span data-ttu-id="99e7c-130">响应</span><span class="sxs-lookup"><span data-stu-id="99e7c-130">Response</span></span>
<span data-ttu-id="99e7c-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99e7c-131">The following is an example of the response.</span></span> 
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
