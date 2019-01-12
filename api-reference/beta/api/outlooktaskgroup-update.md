---
title: 更新 outlooktaskgroup
description: 更新 Outlook 任务组的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ecea8487e0fedfdf3658d5f04c0ae8d96dcd5d93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940412"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="1d4b0-103">更新 outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="1d4b0-103">Update outlooktaskgroup</span></span>

> <span data-ttu-id="1d4b0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d4b0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d4b0-106">更新 Outlook 任务组的可写属性。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-106">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="1d4b0-107">请注意，不能修改的默认任务组中，"我的任务"的名称。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-107">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="1d4b0-108">权限</span><span class="sxs-lookup"><span data-stu-id="1d4b0-108">Permissions</span></span>
<span data-ttu-id="1d4b0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d4b0-111">Permission type</span></span>      | <span data-ttu-id="1d4b0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d4b0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d4b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d4b0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1d4b0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d4b0-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1d4b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d4b0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d4b0-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d4b0-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1d4b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d4b0-117">Application</span></span> | <span data-ttu-id="1d4b0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d4b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d4b0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1d4b0-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="1d4b0-120">Optional request headers</span></span>
| <span data-ttu-id="1d4b0-121">名称</span><span class="sxs-lookup"><span data-stu-id="1d4b0-121">Name</span></span>       | <span data-ttu-id="1d4b0-122">说明</span><span class="sxs-lookup"><span data-stu-id="1d4b0-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1d4b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d4b0-123">Authorization</span></span>  | <span data-ttu-id="1d4b0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d4b0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d4b0-126">Request body</span></span>
<span data-ttu-id="1d4b0-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d4b0-130">属性</span><span class="sxs-lookup"><span data-stu-id="1d4b0-130">Property</span></span>     | <span data-ttu-id="1d4b0-131">类型</span><span class="sxs-lookup"><span data-stu-id="1d4b0-131">Type</span></span>   |<span data-ttu-id="1d4b0-132">说明</span><span class="sxs-lookup"><span data-stu-id="1d4b0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d4b0-133">name</span><span class="sxs-lookup"><span data-stu-id="1d4b0-133">name</span></span>|<span data-ttu-id="1d4b0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1d4b0-134">String</span></span>|<span data-ttu-id="1d4b0-135">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-135">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="1d4b0-136">响应</span><span class="sxs-lookup"><span data-stu-id="1d4b0-136">Response</span></span>

<span data-ttu-id="1d4b0-137">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d4b0-138">示例</span><span class="sxs-lookup"><span data-stu-id="1d4b0-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d4b0-139">请求</span><span class="sxs-lookup"><span data-stu-id="1d4b0-139">Request</span></span>
<span data-ttu-id="1d4b0-140">下面的示例任务组的名称更改为"个人任务"。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-140">The following example changes the name of a task group to "Personal Tasks".</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')

Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
##### <a name="response"></a><span data-ttu-id="1d4b0-141">响应</span><span class="sxs-lookup"><span data-stu-id="1d4b0-141">Response</span></span>
<span data-ttu-id="1d4b0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d4b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
