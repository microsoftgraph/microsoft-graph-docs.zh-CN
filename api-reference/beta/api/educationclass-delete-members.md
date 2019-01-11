---
title: 删除学生
description: 从 educationClass 删除 educationUser
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0afab5c80c546a9404ee11fc4d127d15b13a4e9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824148"
---
# <a name="remove-a-student"></a><span data-ttu-id="b08a5-103">删除学生</span><span class="sxs-lookup"><span data-stu-id="b08a5-103">Remove a student</span></span>

> <span data-ttu-id="b08a5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b08a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b08a5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b08a5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b08a5-106">从 [educationClass](../resources/educationclass.md) 删除 [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b08a5-106">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="b08a5-107">**注意：** 教师_和_学生包含在课程 **members** 集合中。</span><span class="sxs-lookup"><span data-stu-id="b08a5-107">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="b08a5-108">在调用此 API 之前，确定要删除的 **educationUser** 不是教师。</span><span class="sxs-lookup"><span data-stu-id="b08a5-108">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="b08a5-109">要获取教师列表，可调用 [educationclass_list_teachers](educationclass-list-teachers.md) 并验证要删除的用户的用户 ID 不在返回的教师列表中。</span><span class="sxs-lookup"><span data-stu-id="b08a5-109">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="b08a5-110">权限</span><span class="sxs-lookup"><span data-stu-id="b08a5-110">Permissions</span></span>
<span data-ttu-id="b08a5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b08a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b08a5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b08a5-113">Permission type</span></span>      | <span data-ttu-id="b08a5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b08a5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b08a5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b08a5-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="b08a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b08a5-116">Not supported.</span></span>  |
|<span data-ttu-id="b08a5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b08a5-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b08a5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b08a5-118">Not supported.</span></span>  |
|<span data-ttu-id="b08a5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b08a5-119">Application</span></span> | <span data-ttu-id="b08a5-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b08a5-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b08a5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b08a5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b08a5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b08a5-122">Request headers</span></span>
| <span data-ttu-id="b08a5-123">标头</span><span class="sxs-lookup"><span data-stu-id="b08a5-123">Header</span></span>       | <span data-ttu-id="b08a5-124">值</span><span class="sxs-lookup"><span data-stu-id="b08a5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b08a5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b08a5-125">Authorization</span></span>  | <span data-ttu-id="b08a5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b08a5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b08a5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b08a5-128">Request body</span></span>
<span data-ttu-id="b08a5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b08a5-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b08a5-130">响应</span><span class="sxs-lookup"><span data-stu-id="b08a5-130">Response</span></span>
<span data-ttu-id="b08a5-131">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="b08a5-131">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="b08a5-132">示例</span><span class="sxs-lookup"><span data-stu-id="b08a5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b08a5-133">请求</span><span class="sxs-lookup"><span data-stu-id="b08a5-133">Request</span></span>
<span data-ttu-id="b08a5-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b08a5-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="b08a5-135">响应</span><span class="sxs-lookup"><span data-stu-id="b08a5-135">Response</span></span>
<span data-ttu-id="b08a5-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b08a5-136">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
