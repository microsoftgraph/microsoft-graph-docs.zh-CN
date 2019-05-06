---
title: 删除活动
description: 删除应用程序的现有用户活动。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: ba1c87c229fe76f20c85c164b7d788f7df9316b8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610786"
---
# <a name="delete-an-activity"></a><span data-ttu-id="f1fbd-103">删除活动</span><span class="sxs-lookup"><span data-stu-id="f1fbd-103">Delete an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1fbd-104">删除应用程序的现有用户活动。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1fbd-105">权限</span><span class="sxs-lookup"><span data-stu-id="f1fbd-105">Permissions</span></span>

<span data-ttu-id="f1fbd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f1fbd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1fbd-108">Permission type</span></span>      | <span data-ttu-id="f1fbd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1fbd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1fbd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1fbd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1fbd-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f1fbd-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f1fbd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1fbd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1fbd-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f1fbd-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f1fbd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1fbd-114">Application</span></span> | <span data-ttu-id="f1fbd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1fbd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1fbd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1fbd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1fbd-117">Request headers</span></span>

|<span data-ttu-id="f1fbd-118">名称</span><span class="sxs-lookup"><span data-stu-id="f1fbd-118">Name</span></span> | <span data-ttu-id="f1fbd-119">类型</span><span class="sxs-lookup"><span data-stu-id="f1fbd-119">Type</span></span> | <span data-ttu-id="f1fbd-120">说明</span><span class="sxs-lookup"><span data-stu-id="f1fbd-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f1fbd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1fbd-121">Authorization</span></span> | <span data-ttu-id="f1fbd-122">string</span><span class="sxs-lookup"><span data-stu-id="f1fbd-122">string</span></span> | <span data-ttu-id="f1fbd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1fbd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1fbd-125">Request body</span></span>

<span data-ttu-id="f1fbd-126">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="f1fbd-127">响应</span><span class="sxs-lookup"><span data-stu-id="f1fbd-127">Response</span></span>

<span data-ttu-id="f1fbd-128">如果成功, 此方法将返回`204 No Content`响应代码 (如果活动已删除)。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="f1fbd-129">示例</span><span class="sxs-lookup"><span data-stu-id="f1fbd-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f1fbd-130">请求</span><span class="sxs-lookup"><span data-stu-id="f1fbd-130">Request</span></span>

<span data-ttu-id="f1fbd-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="f1fbd-132">响应</span><span class="sxs-lookup"><span data-stu-id="f1fbd-132">Response</span></span>

<span data-ttu-id="f1fbd-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f1fbd-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1fbd-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f1fbd-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1fbd-135">语言</span><span class="sxs-lookup"><span data-stu-id="f1fbd-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_activity-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1fbd-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1fbd-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_activity-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
