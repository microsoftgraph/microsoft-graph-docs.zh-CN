---
title: 更新 outlooktaskfolder
description: 更新 Outlook 任务文件夹的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 06dd21cf9da2fab8c0472ac29f477b6a40d2df5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874352"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="d1ea7-103">更新 outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="d1ea7-103">Update outlooktaskfolder</span></span>

> <span data-ttu-id="d1ea7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1ea7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1ea7-106">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-106">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="d1ea7-107">您无法更改默认任务文件夹中，"任务"的**name**属性值。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-107">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="d1ea7-108">权限</span><span class="sxs-lookup"><span data-stu-id="d1ea7-108">Permissions</span></span>
<span data-ttu-id="d1ea7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1ea7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1ea7-111">Permission type</span></span>      | <span data-ttu-id="d1ea7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1ea7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1ea7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1ea7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d1ea7-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1ea7-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d1ea7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1ea7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1ea7-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1ea7-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d1ea7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1ea7-117">Application</span></span> | <span data-ttu-id="d1ea7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1ea7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1ea7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d1ea7-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d1ea7-120">Optional request headers</span></span>
| <span data-ttu-id="d1ea7-121">名称</span><span class="sxs-lookup"><span data-stu-id="d1ea7-121">Name</span></span>       | <span data-ttu-id="d1ea7-122">说明</span><span class="sxs-lookup"><span data-stu-id="d1ea7-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d1ea7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1ea7-123">Authorization</span></span>  | <span data-ttu-id="d1ea7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1ea7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1ea7-126">Request body</span></span>
<span data-ttu-id="d1ea7-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d1ea7-130">属性</span><span class="sxs-lookup"><span data-stu-id="d1ea7-130">Property</span></span>     | <span data-ttu-id="d1ea7-131">类型</span><span class="sxs-lookup"><span data-stu-id="d1ea7-131">Type</span></span>   |<span data-ttu-id="d1ea7-132">说明</span><span class="sxs-lookup"><span data-stu-id="d1ea7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1ea7-133">name</span><span class="sxs-lookup"><span data-stu-id="d1ea7-133">name</span></span>|<span data-ttu-id="d1ea7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d1ea7-134">String</span></span>|<span data-ttu-id="d1ea7-135">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-135">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="d1ea7-136">响应</span><span class="sxs-lookup"><span data-stu-id="d1ea7-136">Response</span></span>

<span data-ttu-id="d1ea7-137">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1ea7-138">示例</span><span class="sxs-lookup"><span data-stu-id="d1ea7-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1ea7-139">请求</span><span class="sxs-lookup"><span data-stu-id="d1ea7-139">Request</span></span>
<span data-ttu-id="d1ea7-140">以下示例更改为指定的任务文件夹的名称`Charity work`。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-140">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPWAAA=')
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="d1ea7-141">响应</span><span class="sxs-lookup"><span data-stu-id="d1ea7-141">Response</span></span>
<span data-ttu-id="d1ea7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1ea7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAKfQ==",
  "isDefaultFolder": false,
  "name": "Charity work",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
