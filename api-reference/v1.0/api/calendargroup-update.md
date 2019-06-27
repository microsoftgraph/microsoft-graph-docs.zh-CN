---
title: 更新 calendarGroup
description: 更新 calendargroup 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2f017c20c3cf982dd09fb84dfead90b56a7fe184
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264692"
---
# <a name="update-calendargroup"></a><span data-ttu-id="3a3cb-103">更新 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="3a3cb-103">Update calendargroup</span></span>

<span data-ttu-id="3a3cb-104">更新 calendargroup 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-104">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a3cb-105">权限</span><span class="sxs-lookup"><span data-stu-id="3a3cb-105">Permissions</span></span>

<span data-ttu-id="3a3cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a3cb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a3cb-108">Permission type</span></span>                        | <span data-ttu-id="3a3cb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a3cb-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3a3cb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a3cb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a3cb-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a3cb-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="3a3cb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a3cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a3cb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a3cb-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="3a3cb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a3cb-114">Application</span></span>                            | <span data-ttu-id="3a3cb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a3cb-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3a3cb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a3cb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3a3cb-117">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3a3cb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a3cb-118">Request headers</span></span>

| <span data-ttu-id="3a3cb-119">标头</span><span class="sxs-lookup"><span data-stu-id="3a3cb-119">Header</span></span>        | <span data-ttu-id="3a3cb-120">值</span><span class="sxs-lookup"><span data-stu-id="3a3cb-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="3a3cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a3cb-121">Authorization</span></span> | <span data-ttu-id="3a3cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3a3cb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a3cb-124">Content-Type</span></span>  | <span data-ttu-id="3a3cb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3a3cb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a3cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a3cb-127">Request body</span></span>

<span data-ttu-id="3a3cb-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3a3cb-131">属性</span><span class="sxs-lookup"><span data-stu-id="3a3cb-131">Property</span></span> | <span data-ttu-id="3a3cb-132">类型</span><span class="sxs-lookup"><span data-stu-id="3a3cb-132">Type</span></span>   | <span data-ttu-id="3a3cb-133">说明</span><span class="sxs-lookup"><span data-stu-id="3a3cb-133">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="3a3cb-134">name</span><span class="sxs-lookup"><span data-stu-id="3a3cb-134">name</span></span>     | <span data-ttu-id="3a3cb-135">String</span><span class="sxs-lookup"><span data-stu-id="3a3cb-135">String</span></span> | <span data-ttu-id="3a3cb-136">组名称。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-136">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="3a3cb-137">响应</span><span class="sxs-lookup"><span data-stu-id="3a3cb-137">Response</span></span>

<span data-ttu-id="3a3cb-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-138">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a3cb-139">示例</span><span class="sxs-lookup"><span data-stu-id="3a3cb-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3a3cb-140">请求</span><span class="sxs-lookup"><span data-stu-id="3a3cb-140">Request</span></span>

<span data-ttu-id="3a3cb-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="3a3cb-142">响应</span><span class="sxs-lookup"><span data-stu-id="3a3cb-142">Response</span></span>

<span data-ttu-id="3a3cb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a3cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3a3cb-146">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3a3cb-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3a3cb-147">C#</span><span class="sxs-lookup"><span data-stu-id="3a3cb-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_calendargroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a3cb-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a3cb-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_calendargroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3a3cb-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="3a3cb-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_calendargroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendargroup-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendargroup-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendargroup-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
