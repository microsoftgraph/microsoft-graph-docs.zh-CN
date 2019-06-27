---
title: 更新 outlooktaskgroup
description: 更新 Outlook 任务组的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 75e41f92b28d4ca8ab2114e0fc7fd346ad49d16f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267786"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="a76d1-103">更新 outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="a76d1-103">Update outlooktaskgroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a76d1-104">更新 Outlook 任务组的可写属性。</span><span class="sxs-lookup"><span data-stu-id="a76d1-104">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="a76d1-105">请注意, 不能修改默认任务组 "我的任务" 的名称。</span><span class="sxs-lookup"><span data-stu-id="a76d1-105">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="a76d1-106">权限</span><span class="sxs-lookup"><span data-stu-id="a76d1-106">Permissions</span></span>
<span data-ttu-id="a76d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a76d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a76d1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a76d1-109">Permission type</span></span>      | <span data-ttu-id="a76d1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a76d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a76d1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a76d1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a76d1-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a76d1-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a76d1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a76d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a76d1-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a76d1-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a76d1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a76d1-115">Application</span></span> | <span data-ttu-id="a76d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a76d1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a76d1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a76d1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a76d1-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a76d1-118">Optional request headers</span></span>
| <span data-ttu-id="a76d1-119">名称</span><span class="sxs-lookup"><span data-stu-id="a76d1-119">Name</span></span>       | <span data-ttu-id="a76d1-120">说明</span><span class="sxs-lookup"><span data-stu-id="a76d1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a76d1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a76d1-121">Authorization</span></span>  | <span data-ttu-id="a76d1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a76d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a76d1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a76d1-124">Request body</span></span>
<span data-ttu-id="a76d1-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a76d1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a76d1-128">属性</span><span class="sxs-lookup"><span data-stu-id="a76d1-128">Property</span></span>     | <span data-ttu-id="a76d1-129">类型</span><span class="sxs-lookup"><span data-stu-id="a76d1-129">Type</span></span>   |<span data-ttu-id="a76d1-130">说明</span><span class="sxs-lookup"><span data-stu-id="a76d1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a76d1-131">name</span><span class="sxs-lookup"><span data-stu-id="a76d1-131">name</span></span>|<span data-ttu-id="a76d1-132">String</span><span class="sxs-lookup"><span data-stu-id="a76d1-132">String</span></span>|<span data-ttu-id="a76d1-133">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="a76d1-133">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="a76d1-134">响应</span><span class="sxs-lookup"><span data-stu-id="a76d1-134">Response</span></span>

<span data-ttu-id="a76d1-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a76d1-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a76d1-136">示例</span><span class="sxs-lookup"><span data-stu-id="a76d1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a76d1-137">请求</span><span class="sxs-lookup"><span data-stu-id="a76d1-137">Request</span></span>
<span data-ttu-id="a76d1-138">下面的示例将任务组的名称更改为 "个人任务"。</span><span class="sxs-lookup"><span data-stu-id="a76d1-138">The following example changes the name of a task group to "Personal Tasks".</span></span> 
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
##### <a name="response"></a><span data-ttu-id="a76d1-139">响应</span><span class="sxs-lookup"><span data-stu-id="a76d1-139">Response</span></span>
<span data-ttu-id="a76d1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a76d1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a76d1-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a76d1-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a76d1-144">C#</span><span class="sxs-lookup"><span data-stu-id="a76d1-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a76d1-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="a76d1-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a76d1-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="a76d1-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
