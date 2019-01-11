---
title: 删除 calendarGroup
description: 删除默认日历组以外的日历组。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 7b67908b8ffc00a3a857c1ee163ee5290c17c7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838792"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="a624a-103">删除 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a624a-103">Delete calendarGroup</span></span>

> <span data-ttu-id="a624a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a624a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a624a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a624a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a624a-106">删除默认日历组以外的日历组。</span><span class="sxs-lookup"><span data-stu-id="a624a-106">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="a624a-107">权限</span><span class="sxs-lookup"><span data-stu-id="a624a-107">Permissions</span></span>

<span data-ttu-id="a624a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a624a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a624a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a624a-110">Permission type</span></span>                        | <span data-ttu-id="a624a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a624a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a624a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a624a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a624a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a624a-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="a624a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a624a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a624a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a624a-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="a624a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a624a-116">Application</span></span>                            | <span data-ttu-id="a624a-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a624a-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a624a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a624a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a624a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a624a-119">Request headers</span></span>

| <span data-ttu-id="a624a-120">名称</span><span class="sxs-lookup"><span data-stu-id="a624a-120">Name</span></span>          | <span data-ttu-id="a624a-121">类型</span><span class="sxs-lookup"><span data-stu-id="a624a-121">Type</span></span>   | <span data-ttu-id="a624a-122">说明</span><span class="sxs-lookup"><span data-stu-id="a624a-122">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="a624a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a624a-123">Authorization</span></span> | <span data-ttu-id="a624a-124">string</span><span class="sxs-lookup"><span data-stu-id="a624a-124">string</span></span> | <span data-ttu-id="a624a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a624a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a624a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a624a-127">Request body</span></span>

<span data-ttu-id="a624a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a624a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a624a-129">响应</span><span class="sxs-lookup"><span data-stu-id="a624a-129">Response</span></span>

<span data-ttu-id="a624a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a624a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a624a-132">示例</span><span class="sxs-lookup"><span data-stu-id="a624a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a624a-133">请求</span><span class="sxs-lookup"><span data-stu-id="a624a-133">Request</span></span>

<span data-ttu-id="a624a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a624a-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="a624a-135">响应</span><span class="sxs-lookup"><span data-stu-id="a624a-135">Response</span></span>

<span data-ttu-id="a624a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a624a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
