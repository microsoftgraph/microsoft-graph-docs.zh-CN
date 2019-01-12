---
title: 创建 CalendarGroup
description: 使用此 API 创建新的 CalendarGroup。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f4b720f8d293c9803c25a32329c3d4bb8ee7bf7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990206"
---
# <a name="create-calendargroup"></a><span data-ttu-id="5f506-103">创建 CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="5f506-103">Create CalendarGroup</span></span>

> <span data-ttu-id="5f506-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5f506-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f506-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f506-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f506-106">使用此 API 创建新的 CalendarGroup。</span><span class="sxs-lookup"><span data-stu-id="5f506-106">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f506-107">权限</span><span class="sxs-lookup"><span data-stu-id="5f506-107">Permissions</span></span>
<span data-ttu-id="5f506-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f506-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f506-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f506-110">Permission type</span></span>      | <span data-ttu-id="5f506-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f506-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f506-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f506-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5f506-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f506-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f506-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f506-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f506-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f506-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f506-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f506-116">Application</span></span> | <span data-ttu-id="5f506-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f506-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f506-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f506-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="5f506-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f506-119">Request headers</span></span>
| <span data-ttu-id="5f506-120">标头</span><span class="sxs-lookup"><span data-stu-id="5f506-120">Header</span></span>       | <span data-ttu-id="5f506-121">值</span><span class="sxs-lookup"><span data-stu-id="5f506-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f506-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f506-122">Authorization</span></span>  | <span data-ttu-id="5f506-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f506-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5f506-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f506-125">Content-Type</span></span>  | <span data-ttu-id="5f506-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f506-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f506-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f506-127">Request body</span></span>
<span data-ttu-id="5f506-128">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f506-128">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5f506-129">响应</span><span class="sxs-lookup"><span data-stu-id="5f506-129">Response</span></span>

<span data-ttu-id="5f506-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f506-130">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f506-131">示例</span><span class="sxs-lookup"><span data-stu-id="5f506-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f506-132">请求</span><span class="sxs-lookup"><span data-stu-id="5f506-132">Request</span></span>
<span data-ttu-id="5f506-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f506-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="5f506-134">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f506-134">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5f506-135">响应</span><span class="sxs-lookup"><span data-stu-id="5f506-135">Response</span></span>
<span data-ttu-id="5f506-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f506-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
