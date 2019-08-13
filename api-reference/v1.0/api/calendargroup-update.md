---
title: 更新 calendarGroup
description: 更新 calendargroup 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d159b57978044a2d112cfc1e56b1318acc8cee3c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369064"
---
# <a name="update-calendargroup"></a><span data-ttu-id="921fe-103">更新 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="921fe-103">Update calendargroup</span></span>

<span data-ttu-id="921fe-104">更新 calendargroup 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="921fe-104">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="921fe-105">权限</span><span class="sxs-lookup"><span data-stu-id="921fe-105">Permissions</span></span>

<span data-ttu-id="921fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="921fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="921fe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="921fe-108">Permission type</span></span>                        | <span data-ttu-id="921fe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="921fe-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="921fe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="921fe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="921fe-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="921fe-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="921fe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="921fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="921fe-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="921fe-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="921fe-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="921fe-114">Application</span></span>                            | <span data-ttu-id="921fe-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="921fe-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="921fe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="921fe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="921fe-117">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="921fe-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="921fe-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="921fe-118">Request headers</span></span>

| <span data-ttu-id="921fe-119">标头</span><span class="sxs-lookup"><span data-stu-id="921fe-119">Header</span></span>        | <span data-ttu-id="921fe-120">值</span><span class="sxs-lookup"><span data-stu-id="921fe-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="921fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="921fe-121">Authorization</span></span> | <span data-ttu-id="921fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="921fe-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="921fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="921fe-124">Content-Type</span></span>  | <span data-ttu-id="921fe-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="921fe-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="921fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="921fe-127">Request body</span></span>

<span data-ttu-id="921fe-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="921fe-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="921fe-131">属性</span><span class="sxs-lookup"><span data-stu-id="921fe-131">Property</span></span> | <span data-ttu-id="921fe-132">类型</span><span class="sxs-lookup"><span data-stu-id="921fe-132">Type</span></span>   | <span data-ttu-id="921fe-133">说明</span><span class="sxs-lookup"><span data-stu-id="921fe-133">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="921fe-134">name</span><span class="sxs-lookup"><span data-stu-id="921fe-134">name</span></span>     | <span data-ttu-id="921fe-135">String</span><span class="sxs-lookup"><span data-stu-id="921fe-135">String</span></span> | <span data-ttu-id="921fe-136">组名称。</span><span class="sxs-lookup"><span data-stu-id="921fe-136">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="921fe-137">响应</span><span class="sxs-lookup"><span data-stu-id="921fe-137">Response</span></span>

<span data-ttu-id="921fe-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="921fe-138">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="921fe-139">示例</span><span class="sxs-lookup"><span data-stu-id="921fe-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="921fe-140">请求</span><span class="sxs-lookup"><span data-stu-id="921fe-140">Request</span></span>

<span data-ttu-id="921fe-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="921fe-141">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="921fe-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="921fe-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="921fe-143">C#</span><span class="sxs-lookup"><span data-stu-id="921fe-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="921fe-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="921fe-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="921fe-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="921fe-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="921fe-146">Java</span><span class="sxs-lookup"><span data-stu-id="921fe-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="921fe-147">响应</span><span class="sxs-lookup"><span data-stu-id="921fe-147">Response</span></span>

<span data-ttu-id="921fe-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="921fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
