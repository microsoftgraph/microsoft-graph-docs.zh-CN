---
title: 更新 outlooktaskgroup
description: 更新任务组的可写Outlook属性。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 37bf87e8d52ac320d29fd7be1f6cdd3dae7165ea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049203"
---
# <a name="update-outlooktaskgroup-deprecated"></a><span data-ttu-id="e22e9-103">更新 outlooktaskgroup (已弃) </span><span class="sxs-lookup"><span data-stu-id="e22e9-103">Update outlooktaskgroup (deprecated)</span></span>

<span data-ttu-id="e22e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e22e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="e22e9-105">更新任务组的可写Outlook属性。</span><span class="sxs-lookup"><span data-stu-id="e22e9-105">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="e22e9-106">请注意，您无法修改默认任务组"My Tasks"的名称。</span><span class="sxs-lookup"><span data-stu-id="e22e9-106">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="e22e9-107">权限</span><span class="sxs-lookup"><span data-stu-id="e22e9-107">Permissions</span></span>
<span data-ttu-id="e22e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e22e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e22e9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e22e9-110">Permission type</span></span>      | <span data-ttu-id="e22e9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e22e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e22e9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e22e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e22e9-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e22e9-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e22e9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e22e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e22e9-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e22e9-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e22e9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e22e9-116">Application</span></span> | <span data-ttu-id="e22e9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e22e9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e22e9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e22e9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e22e9-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="e22e9-119">Optional request headers</span></span>
| <span data-ttu-id="e22e9-120">名称</span><span class="sxs-lookup"><span data-stu-id="e22e9-120">Name</span></span>       | <span data-ttu-id="e22e9-121">说明</span><span class="sxs-lookup"><span data-stu-id="e22e9-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e22e9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e22e9-122">Authorization</span></span>  | <span data-ttu-id="e22e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e22e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e22e9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e22e9-125">Request body</span></span>
<span data-ttu-id="e22e9-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e22e9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e22e9-129">属性</span><span class="sxs-lookup"><span data-stu-id="e22e9-129">Property</span></span>     | <span data-ttu-id="e22e9-130">类型</span><span class="sxs-lookup"><span data-stu-id="e22e9-130">Type</span></span>   |<span data-ttu-id="e22e9-131">说明</span><span class="sxs-lookup"><span data-stu-id="e22e9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e22e9-132">name</span><span class="sxs-lookup"><span data-stu-id="e22e9-132">name</span></span>|<span data-ttu-id="e22e9-133">String</span><span class="sxs-lookup"><span data-stu-id="e22e9-133">String</span></span>|<span data-ttu-id="e22e9-134">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="e22e9-134">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="e22e9-135">响应</span><span class="sxs-lookup"><span data-stu-id="e22e9-135">Response</span></span>

<span data-ttu-id="e22e9-136">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e22e9-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e22e9-137">示例</span><span class="sxs-lookup"><span data-stu-id="e22e9-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e22e9-138">请求</span><span class="sxs-lookup"><span data-stu-id="e22e9-138">Request</span></span>
<span data-ttu-id="e22e9-139">下面的示例将任务组的名称更改为"个人任务"。</span><span class="sxs-lookup"><span data-stu-id="e22e9-139">The following example changes the name of a task group to "Personal Tasks".</span></span> 

# <a name="http"></a>[<span data-ttu-id="e22e9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e22e9-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
# <a name="c"></a>[<span data-ttu-id="e22e9-141">C#</span><span class="sxs-lookup"><span data-stu-id="e22e9-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e22e9-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e22e9-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e22e9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e22e9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e22e9-144">Java</span><span class="sxs-lookup"><span data-stu-id="e22e9-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e22e9-145">响应</span><span class="sxs-lookup"><span data-stu-id="e22e9-145">Response</span></span>
<span data-ttu-id="e22e9-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e22e9-146">Here is an example of the response.</span></span> <span data-ttu-id="e22e9-147">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e22e9-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjw==",
  "isDefaultGroup": false,
  "name": "Personal Tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


