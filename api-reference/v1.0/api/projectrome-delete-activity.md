---
title: 删除活动
description: 删除应用程序的现有用户活动。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 6df91f6111381a9795fa9a046f30d6e45a55a4b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894011"
---
# <a name="delete-an-activity"></a><span data-ttu-id="49c0d-103">删除活动</span><span class="sxs-lookup"><span data-stu-id="49c0d-103">Delete an activity</span></span>

<span data-ttu-id="49c0d-104">删除应用程序的现有用户活动。</span><span class="sxs-lookup"><span data-stu-id="49c0d-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="49c0d-105">权限</span><span class="sxs-lookup"><span data-stu-id="49c0d-105">Permissions</span></span>

<span data-ttu-id="49c0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49c0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="49c0d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="49c0d-108">Permission type</span></span>      | <span data-ttu-id="49c0d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49c0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49c0d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49c0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49c0d-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="49c0d-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="49c0d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49c0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49c0d-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="49c0d-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="49c0d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="49c0d-114">Application</span></span> | <span data-ttu-id="49c0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="49c0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49c0d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49c0d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="49c0d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="49c0d-117">Request headers</span></span>

|<span data-ttu-id="49c0d-118">名称</span><span class="sxs-lookup"><span data-stu-id="49c0d-118">Name</span></span> | <span data-ttu-id="49c0d-119">类型</span><span class="sxs-lookup"><span data-stu-id="49c0d-119">Type</span></span> | <span data-ttu-id="49c0d-120">说明</span><span class="sxs-lookup"><span data-stu-id="49c0d-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="49c0d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="49c0d-121">Authorization</span></span> | <span data-ttu-id="49c0d-122">string</span><span class="sxs-lookup"><span data-stu-id="49c0d-122">string</span></span> | <span data-ttu-id="49c0d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49c0d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49c0d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="49c0d-125">Request body</span></span>

<span data-ttu-id="49c0d-126">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="49c0d-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="49c0d-127">响应</span><span class="sxs-lookup"><span data-stu-id="49c0d-127">Response</span></span>

<span data-ttu-id="49c0d-128">如果成功, 此方法将返回`204 No Content`响应代码 (如果活动已删除)。</span><span class="sxs-lookup"><span data-stu-id="49c0d-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="49c0d-129">示例</span><span class="sxs-lookup"><span data-stu-id="49c0d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="49c0d-130">请求</span><span class="sxs-lookup"><span data-stu-id="49c0d-130">Request</span></span>

<span data-ttu-id="49c0d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49c0d-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49c0d-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="49c0d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49c0d-133">C#</span><span class="sxs-lookup"><span data-stu-id="49c0d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49c0d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="49c0d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49c0d-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="49c0d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49c0d-136">Java</span><span class="sxs-lookup"><span data-stu-id="49c0d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49c0d-137">响应</span><span class="sxs-lookup"><span data-stu-id="49c0d-137">Response</span></span>

<span data-ttu-id="49c0d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49c0d-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
