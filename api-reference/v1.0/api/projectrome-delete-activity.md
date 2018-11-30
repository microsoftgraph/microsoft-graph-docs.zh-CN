---
title: 删除活动
description: 删除现有用户活动应用程序。
ms.openlocfilehash: a4b32e00719772f6dcfb715fa69350edf9a8b48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008520"
---
# <a name="delete-an-activity"></a><span data-ttu-id="d659e-103">删除活动</span><span class="sxs-lookup"><span data-stu-id="d659e-103">Delete an activity</span></span>

<span data-ttu-id="d659e-104">删除现有用户活动应用程序。</span><span class="sxs-lookup"><span data-stu-id="d659e-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="d659e-105">权限</span><span class="sxs-lookup"><span data-stu-id="d659e-105">Permissions</span></span>

<span data-ttu-id="d659e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d659e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d659e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d659e-108">Permission type</span></span>      | <span data-ttu-id="d659e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d659e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d659e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d659e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d659e-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d659e-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d659e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d659e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d659e-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d659e-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d659e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d659e-114">Application</span></span> | <span data-ttu-id="d659e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d659e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d659e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d659e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d659e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d659e-117">Request headers</span></span>

|<span data-ttu-id="d659e-118">名称</span><span class="sxs-lookup"><span data-stu-id="d659e-118">Name</span></span> | <span data-ttu-id="d659e-119">类型</span><span class="sxs-lookup"><span data-stu-id="d659e-119">Type</span></span> | <span data-ttu-id="d659e-120">说明</span><span class="sxs-lookup"><span data-stu-id="d659e-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d659e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d659e-121">Authorization</span></span> | <span data-ttu-id="d659e-122">string</span><span class="sxs-lookup"><span data-stu-id="d659e-122">string</span></span> | <span data-ttu-id="d659e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d659e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d659e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d659e-125">Request body</span></span>

<span data-ttu-id="d659e-126">没有请求正文中。</span><span class="sxs-lookup"><span data-stu-id="d659e-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="d659e-127">响应</span><span class="sxs-lookup"><span data-stu-id="d659e-127">Response</span></span>

<span data-ttu-id="d659e-128">如果成功，此方法返回`204 No Content`如果活动的已删除的响应代码。</span><span class="sxs-lookup"><span data-stu-id="d659e-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="d659e-129">示例</span><span class="sxs-lookup"><span data-stu-id="d659e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d659e-130">请求</span><span class="sxs-lookup"><span data-stu-id="d659e-130">Request</span></span>

<span data-ttu-id="d659e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d659e-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="d659e-132">响应</span><span class="sxs-lookup"><span data-stu-id="d659e-132">Response</span></span>

<span data-ttu-id="d659e-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d659e-133">Here is an example of the response.</span></span>

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
  "tocPath": ""
}-->