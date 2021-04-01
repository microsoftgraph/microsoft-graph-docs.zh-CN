---
title: 创建 CalendarGroup
description: 使用此 API 创建新的 CalendarGroup。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fff440ecbbdf79ac7b5e49642fb6f86330128dff
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473414"
---
# <a name="create-calendargroup"></a><span data-ttu-id="6861c-103">创建 CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="6861c-103">Create CalendarGroup</span></span>

<span data-ttu-id="6861c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6861c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6861c-105">使用此 API 创建新的 CalendarGroup。</span><span class="sxs-lookup"><span data-stu-id="6861c-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="6861c-106">权限</span><span class="sxs-lookup"><span data-stu-id="6861c-106">Permissions</span></span>
<span data-ttu-id="6861c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6861c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6861c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6861c-109">Permission type</span></span>      | <span data-ttu-id="6861c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6861c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6861c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6861c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6861c-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6861c-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6861c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6861c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6861c-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6861c-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6861c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6861c-115">Application</span></span> | <span data-ttu-id="6861c-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6861c-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6861c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6861c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="6861c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6861c-118">Request headers</span></span>
| <span data-ttu-id="6861c-119">标头</span><span class="sxs-lookup"><span data-stu-id="6861c-119">Header</span></span>       | <span data-ttu-id="6861c-120">值</span><span class="sxs-lookup"><span data-stu-id="6861c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6861c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6861c-121">Authorization</span></span>  | <span data-ttu-id="6861c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6861c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6861c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6861c-124">Content-Type</span></span>  | <span data-ttu-id="6861c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6861c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6861c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6861c-126">Request body</span></span>
<span data-ttu-id="6861c-127">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6861c-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6861c-128">响应</span><span class="sxs-lookup"><span data-stu-id="6861c-128">Response</span></span>

<span data-ttu-id="6861c-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6861c-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6861c-130">示例</span><span class="sxs-lookup"><span data-stu-id="6861c-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="6861c-131">请求</span><span class="sxs-lookup"><span data-stu-id="6861c-131">Request</span></span>
<span data-ttu-id="6861c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6861c-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json

{
  "name": "Personal events"
}
```

<span data-ttu-id="6861c-133">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6861c-133">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="6861c-134">响应</span><span class="sxs-lookup"><span data-stu-id="6861c-134">Response</span></span>
<span data-ttu-id="6861c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6861c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('7d54cb02-aaa3-4016-9f9c-a4b49422dd9b')/calendarGroups/$entity",
    "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy0YOkcEEh3vhfAAAGgdFjAAA=",
    "name": "Personal events",
    "classId": "44288f7d-7710-4293-8c8e-36f310ed2e6a",
    "changeKey": "NreqLYgxdE2DpHBBId74XwAABn6y8Q=="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


