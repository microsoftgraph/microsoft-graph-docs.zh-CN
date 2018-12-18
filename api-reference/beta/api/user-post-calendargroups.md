---
title: 创建 CalendarGroup
description: 使用此 API 创建新的 CalendarGroup。
author: dkershaw10
ms.openlocfilehash: a68be3470489b20667112b67d15f4472a3817d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319045"
---
# <a name="create-calendargroup"></a><span data-ttu-id="f348d-103">创建 CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="f348d-103">Create CalendarGroup</span></span>

> <span data-ttu-id="f348d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f348d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f348d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f348d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f348d-106">使用此 API 创建新的 CalendarGroup。</span><span class="sxs-lookup"><span data-stu-id="f348d-106">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="f348d-107">权限</span><span class="sxs-lookup"><span data-stu-id="f348d-107">Permissions</span></span>
<span data-ttu-id="f348d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f348d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f348d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f348d-110">Permission type</span></span>      | <span data-ttu-id="f348d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f348d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f348d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f348d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f348d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f348d-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f348d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f348d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f348d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f348d-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f348d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f348d-116">Application</span></span> | <span data-ttu-id="f348d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f348d-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f348d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f348d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="f348d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f348d-119">Request headers</span></span>
| <span data-ttu-id="f348d-120">标头</span><span class="sxs-lookup"><span data-stu-id="f348d-120">Header</span></span>       | <span data-ttu-id="f348d-121">值</span><span class="sxs-lookup"><span data-stu-id="f348d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f348d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f348d-122">Authorization</span></span>  | <span data-ttu-id="f348d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f348d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f348d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f348d-125">Content-Type</span></span>  | <span data-ttu-id="f348d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f348d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f348d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f348d-127">Request body</span></span>
<span data-ttu-id="f348d-128">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f348d-128">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f348d-129">响应</span><span class="sxs-lookup"><span data-stu-id="f348d-129">Response</span></span>

<span data-ttu-id="f348d-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f348d-130">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f348d-131">示例</span><span class="sxs-lookup"><span data-stu-id="f348d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f348d-132">请求</span><span class="sxs-lookup"><span data-stu-id="f348d-132">Request</span></span>
<span data-ttu-id="f348d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f348d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="f348d-134">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f348d-134">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f348d-135">响应</span><span class="sxs-lookup"><span data-stu-id="f348d-135">Response</span></span>
<span data-ttu-id="f348d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f348d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
