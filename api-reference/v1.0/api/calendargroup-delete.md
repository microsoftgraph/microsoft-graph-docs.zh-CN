---
title: 删除 calendarGroup
description: 删除默认日历组以外的日历组。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 80e050a6fd8520782501a9d718fba9d4d9840fa7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264720"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="bc021-103">删除 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="bc021-103">Delete calendarGroup</span></span>

<span data-ttu-id="bc021-104">删除默认日历组以外的日历组。</span><span class="sxs-lookup"><span data-stu-id="bc021-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc021-105">权限</span><span class="sxs-lookup"><span data-stu-id="bc021-105">Permissions</span></span>

<span data-ttu-id="bc021-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc021-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc021-108">Permission type</span></span>                        | <span data-ttu-id="bc021-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc021-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bc021-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc021-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc021-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc021-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bc021-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc021-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc021-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc021-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bc021-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc021-114">Application</span></span>                            | <span data-ttu-id="bc021-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc021-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bc021-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc021-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bc021-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc021-117">Request headers</span></span>

| <span data-ttu-id="bc021-118">名称</span><span class="sxs-lookup"><span data-stu-id="bc021-118">Name</span></span>          | <span data-ttu-id="bc021-119">类型</span><span class="sxs-lookup"><span data-stu-id="bc021-119">Type</span></span>   | <span data-ttu-id="bc021-120">说明</span><span class="sxs-lookup"><span data-stu-id="bc021-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="bc021-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc021-121">Authorization</span></span> | <span data-ttu-id="bc021-122">string</span><span class="sxs-lookup"><span data-stu-id="bc021-122">string</span></span> | <span data-ttu-id="bc021-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc021-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc021-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc021-125">Request body</span></span>

<span data-ttu-id="bc021-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc021-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc021-127">响应</span><span class="sxs-lookup"><span data-stu-id="bc021-127">Response</span></span>

<span data-ttu-id="bc021-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bc021-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc021-130">示例</span><span class="sxs-lookup"><span data-stu-id="bc021-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc021-131">请求</span><span class="sxs-lookup"><span data-stu-id="bc021-131">Request</span></span>

<span data-ttu-id="bc021-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc021-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="bc021-133">响应</span><span class="sxs-lookup"><span data-stu-id="bc021-133">Response</span></span>

<span data-ttu-id="bc021-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc021-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bc021-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bc021-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bc021-138">C#</span><span class="sxs-lookup"><span data-stu-id="bc021-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_calendargroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc021-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="bc021-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_calendargroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bc021-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="bc021-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_calendargroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendargroup-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendargroup-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendargroup-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
