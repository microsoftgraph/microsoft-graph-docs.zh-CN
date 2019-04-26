---
title: 删除学生
description: 从 educationClass 删除 educationUser
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ac5ee332c58a070d9f25dfb3bde78177fb323b02
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324946"
---
# <a name="remove-a-student"></a><span data-ttu-id="e6f34-103">删除学生</span><span class="sxs-lookup"><span data-stu-id="e6f34-103">Remove a student</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f34-104">从 [educationClass](../resources/educationclass.md) 删除 [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e6f34-104">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="e6f34-105">**注意：** 教师_和_学生包含在课程 **members** 集合中。</span><span class="sxs-lookup"><span data-stu-id="e6f34-105">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="e6f34-106">在调用此 API 之前，确定要删除的 **educationUser** 不是教师。</span><span class="sxs-lookup"><span data-stu-id="e6f34-106">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="e6f34-107">要获取教师列表，可调用 [educationclass_list_teachers](educationclass-list-teachers.md) 并验证要删除的用户的用户 ID 不在返回的教师列表中。</span><span class="sxs-lookup"><span data-stu-id="e6f34-107">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6f34-108">权限</span><span class="sxs-lookup"><span data-stu-id="e6f34-108">Permissions</span></span>
<span data-ttu-id="e6f34-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6f34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6f34-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6f34-111">Permission type</span></span>      | <span data-ttu-id="e6f34-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6f34-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6f34-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6f34-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6f34-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6f34-114">Not supported.</span></span>  |
|<span data-ttu-id="e6f34-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6f34-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6f34-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6f34-116">Not supported.</span></span>  |
|<span data-ttu-id="e6f34-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6f34-117">Application</span></span> | <span data-ttu-id="e6f34-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f34-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e6f34-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6f34-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e6f34-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6f34-120">Request headers</span></span>
| <span data-ttu-id="e6f34-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6f34-121">Header</span></span>       | <span data-ttu-id="e6f34-122">值</span><span class="sxs-lookup"><span data-stu-id="e6f34-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6f34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6f34-123">Authorization</span></span>  | <span data-ttu-id="e6f34-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6f34-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6f34-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6f34-126">Request body</span></span>
<span data-ttu-id="e6f34-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6f34-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e6f34-128">响应</span><span class="sxs-lookup"><span data-stu-id="e6f34-128">Response</span></span>
<span data-ttu-id="e6f34-129">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="e6f34-129">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6f34-130">示例</span><span class="sxs-lookup"><span data-stu-id="e6f34-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6f34-131">请求</span><span class="sxs-lookup"><span data-stu-id="e6f34-131">Request</span></span>
<span data-ttu-id="e6f34-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6f34-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="e6f34-133">响应</span><span class="sxs-lookup"><span data-stu-id="e6f34-133">Response</span></span>
<span data-ttu-id="e6f34-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e6f34-134">The following is an example of the response.</span></span> 
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
