---
title: 删除 calendarGroup
description: 删除默认日历组以外的日历组。
author: angelgolfer-ms
ms.openlocfilehash: dcb788f29b9e4b00408f4177f5785e6441084332
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342866"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="4a1ef-103">删除 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="4a1ef-103">Delete calendarGroup</span></span>

<span data-ttu-id="4a1ef-104">删除默认日历组以外的日历组。</span><span class="sxs-lookup"><span data-stu-id="4a1ef-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a1ef-105">权限</span><span class="sxs-lookup"><span data-stu-id="4a1ef-105">Permissions</span></span>

<span data-ttu-id="4a1ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a1ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a1ef-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a1ef-108">Permission type</span></span>                        | <span data-ttu-id="4a1ef-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a1ef-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4a1ef-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a1ef-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a1ef-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a1ef-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="4a1ef-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a1ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a1ef-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a1ef-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="4a1ef-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a1ef-114">Application</span></span>                            | <span data-ttu-id="4a1ef-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a1ef-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4a1ef-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a1ef-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a1ef-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a1ef-117">Request headers</span></span>

| <span data-ttu-id="4a1ef-118">Name</span><span class="sxs-lookup"><span data-stu-id="4a1ef-118">Name</span></span>          | <span data-ttu-id="4a1ef-119">类型</span><span class="sxs-lookup"><span data-stu-id="4a1ef-119">Type</span></span>   | <span data-ttu-id="4a1ef-120">说明</span><span class="sxs-lookup"><span data-stu-id="4a1ef-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="4a1ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a1ef-121">Authorization</span></span> | <span data-ttu-id="4a1ef-122">string</span><span class="sxs-lookup"><span data-stu-id="4a1ef-122">string</span></span> | <span data-ttu-id="4a1ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a1ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a1ef-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a1ef-125">Request body</span></span>

<span data-ttu-id="4a1ef-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a1ef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a1ef-127">响应</span><span class="sxs-lookup"><span data-stu-id="4a1ef-127">Response</span></span>

<span data-ttu-id="4a1ef-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4a1ef-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a1ef-130">示例</span><span class="sxs-lookup"><span data-stu-id="4a1ef-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4a1ef-131">请求</span><span class="sxs-lookup"><span data-stu-id="4a1ef-131">Request</span></span>

<span data-ttu-id="4a1ef-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a1ef-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="4a1ef-133">响应</span><span class="sxs-lookup"><span data-stu-id="4a1ef-133">Response</span></span>

<span data-ttu-id="4a1ef-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a1ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
