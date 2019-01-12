---
title: 更新 calendarGroup
description: 更新 calendargroup 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f488594778c1e80e725cb2587bf5d0c41cb570e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961300"
---
# <a name="update-calendargroup"></a><span data-ttu-id="d6b17-103">更新 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="d6b17-103">Update calendargroup</span></span>

> <span data-ttu-id="d6b17-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6b17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6b17-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6b17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6b17-106">更新 calendargroup 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6b17-106">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6b17-107">权限</span><span class="sxs-lookup"><span data-stu-id="d6b17-107">Permissions</span></span>

<span data-ttu-id="d6b17-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6b17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6b17-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6b17-110">Permission type</span></span>                        | <span data-ttu-id="d6b17-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6b17-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d6b17-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6b17-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6b17-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6b17-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="d6b17-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6b17-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6b17-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6b17-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="d6b17-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6b17-116">Application</span></span>                            | <span data-ttu-id="d6b17-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6b17-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d6b17-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6b17-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d6b17-119">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="d6b17-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d6b17-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6b17-120">Request headers</span></span>

| <span data-ttu-id="d6b17-121">标头</span><span class="sxs-lookup"><span data-stu-id="d6b17-121">Header</span></span>        | <span data-ttu-id="d6b17-122">值</span><span class="sxs-lookup"><span data-stu-id="d6b17-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="d6b17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6b17-123">Authorization</span></span> | <span data-ttu-id="d6b17-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6b17-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d6b17-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6b17-126">Content-Type</span></span>  | <span data-ttu-id="d6b17-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d6b17-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6b17-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6b17-129">Request body</span></span>

<span data-ttu-id="d6b17-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d6b17-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d6b17-133">属性</span><span class="sxs-lookup"><span data-stu-id="d6b17-133">Property</span></span> | <span data-ttu-id="d6b17-134">类型</span><span class="sxs-lookup"><span data-stu-id="d6b17-134">Type</span></span>   | <span data-ttu-id="d6b17-135">说明</span><span class="sxs-lookup"><span data-stu-id="d6b17-135">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="d6b17-136">name</span><span class="sxs-lookup"><span data-stu-id="d6b17-136">name</span></span>     | <span data-ttu-id="d6b17-137">String</span><span class="sxs-lookup"><span data-stu-id="d6b17-137">String</span></span> | <span data-ttu-id="d6b17-138">组名称。</span><span class="sxs-lookup"><span data-stu-id="d6b17-138">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="d6b17-139">响应</span><span class="sxs-lookup"><span data-stu-id="d6b17-139">Response</span></span>

<span data-ttu-id="d6b17-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6b17-140">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6b17-141">示例</span><span class="sxs-lookup"><span data-stu-id="d6b17-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6b17-142">请求</span><span class="sxs-lookup"><span data-stu-id="d6b17-142">Request</span></span>

<span data-ttu-id="d6b17-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6b17-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="d6b17-144">响应</span><span class="sxs-lookup"><span data-stu-id="d6b17-144">Response</span></span>

<span data-ttu-id="d6b17-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6b17-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
