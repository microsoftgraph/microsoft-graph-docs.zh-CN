---
title: 更新 calendarGroup
description: 更新 calendargroup 对象的属性。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a8b8a82010a5fb7d5a1423aa3bed8ff15645a678
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039914"
---
# <a name="update-calendargroup"></a><span data-ttu-id="ee587-103">更新 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="ee587-103">Update calendargroup</span></span>

<span data-ttu-id="ee587-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee587-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee587-105">更新 calendargroup 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ee587-105">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee587-106">权限</span><span class="sxs-lookup"><span data-stu-id="ee587-106">Permissions</span></span>

<span data-ttu-id="ee587-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee587-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee587-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee587-109">Permission type</span></span>                        | <span data-ttu-id="ee587-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee587-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ee587-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee587-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee587-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee587-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="ee587-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee587-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee587-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee587-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="ee587-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee587-115">Application</span></span>                            | <span data-ttu-id="ee587-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee587-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ee587-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee587-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="ee587-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="ee587-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ee587-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee587-119">Request headers</span></span>

| <span data-ttu-id="ee587-120">标头</span><span class="sxs-lookup"><span data-stu-id="ee587-120">Header</span></span>        | <span data-ttu-id="ee587-121">值</span><span class="sxs-lookup"><span data-stu-id="ee587-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="ee587-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee587-122">Authorization</span></span> | <span data-ttu-id="ee587-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee587-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ee587-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee587-125">Content-Type</span></span>  | <span data-ttu-id="ee587-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ee587-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee587-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee587-128">Request body</span></span>

<span data-ttu-id="ee587-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ee587-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee587-132">属性</span><span class="sxs-lookup"><span data-stu-id="ee587-132">Property</span></span> | <span data-ttu-id="ee587-133">类型</span><span class="sxs-lookup"><span data-stu-id="ee587-133">Type</span></span>   | <span data-ttu-id="ee587-134">说明</span><span class="sxs-lookup"><span data-stu-id="ee587-134">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="ee587-135">name</span><span class="sxs-lookup"><span data-stu-id="ee587-135">name</span></span>     | <span data-ttu-id="ee587-136">String</span><span class="sxs-lookup"><span data-stu-id="ee587-136">String</span></span> | <span data-ttu-id="ee587-137">组名称。</span><span class="sxs-lookup"><span data-stu-id="ee587-137">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="ee587-138">响应</span><span class="sxs-lookup"><span data-stu-id="ee587-138">Response</span></span>

<span data-ttu-id="ee587-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee587-139">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee587-140">示例</span><span class="sxs-lookup"><span data-stu-id="ee587-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee587-141">请求</span><span class="sxs-lookup"><span data-stu-id="ee587-141">Request</span></span>

<span data-ttu-id="ee587-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee587-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee587-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee587-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ee587-144">C#</span><span class="sxs-lookup"><span data-stu-id="ee587-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee587-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee587-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee587-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee587-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee587-147">Java</span><span class="sxs-lookup"><span data-stu-id="ee587-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee587-148">响应</span><span class="sxs-lookup"><span data-stu-id="ee587-148">Response</span></span>

<span data-ttu-id="ee587-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee587-149">Here is an example of the response.</span></span> <span data-ttu-id="ee587-150">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee587-150">Note: The response object shown here might be shortened for readability.</span></span>

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

