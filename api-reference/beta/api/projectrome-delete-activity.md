---
title: 删除活动
description: 删除应用程序的现有用户活动。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 18062f99f2106eaf60a4f1bab746513e15dda9c7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455488"
---
# <a name="delete-an-activity"></a><span data-ttu-id="57175-103">删除活动</span><span class="sxs-lookup"><span data-stu-id="57175-103">Delete an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57175-104">删除应用程序的现有用户活动。</span><span class="sxs-lookup"><span data-stu-id="57175-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="57175-105">权限</span><span class="sxs-lookup"><span data-stu-id="57175-105">Permissions</span></span>

<span data-ttu-id="57175-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="57175-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="57175-108">Permission type</span></span>      | <span data-ttu-id="57175-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57175-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57175-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57175-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57175-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="57175-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="57175-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57175-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57175-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="57175-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="57175-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="57175-114">Application</span></span> | <span data-ttu-id="57175-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57175-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57175-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57175-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="57175-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="57175-117">Request headers</span></span>

|<span data-ttu-id="57175-118">名称</span><span class="sxs-lookup"><span data-stu-id="57175-118">Name</span></span> | <span data-ttu-id="57175-119">类型</span><span class="sxs-lookup"><span data-stu-id="57175-119">Type</span></span> | <span data-ttu-id="57175-120">说明</span><span class="sxs-lookup"><span data-stu-id="57175-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="57175-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="57175-121">Authorization</span></span> | <span data-ttu-id="57175-122">string</span><span class="sxs-lookup"><span data-stu-id="57175-122">string</span></span> | <span data-ttu-id="57175-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57175-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57175-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="57175-125">Request body</span></span>

<span data-ttu-id="57175-126">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="57175-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="57175-127">响应</span><span class="sxs-lookup"><span data-stu-id="57175-127">Response</span></span>

<span data-ttu-id="57175-128">如果成功, 此方法将返回`204 No Content`响应代码 (如果活动已删除)。</span><span class="sxs-lookup"><span data-stu-id="57175-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="57175-129">示例</span><span class="sxs-lookup"><span data-stu-id="57175-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57175-130">请求</span><span class="sxs-lookup"><span data-stu-id="57175-130">Request</span></span>

<span data-ttu-id="57175-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57175-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="57175-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="57175-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="57175-133">C#</span><span class="sxs-lookup"><span data-stu-id="57175-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57175-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="57175-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57175-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="57175-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="57175-136">响应</span><span class="sxs-lookup"><span data-stu-id="57175-136">Response</span></span>

<span data-ttu-id="57175-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="57175-137">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
