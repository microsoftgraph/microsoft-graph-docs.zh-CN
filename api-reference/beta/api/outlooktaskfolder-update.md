---
title: 更新 outlooktaskfolder
description: 更新 Outlook 任务文件夹的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 44b95bb63eb7ed8b5da2bd97d52321cda1220524
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596284"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="1107c-103">更新 outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="1107c-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1107c-104">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="1107c-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="1107c-105">无法更改默认任务文件夹 "任务" 的 "**名称**" 属性值。</span><span class="sxs-lookup"><span data-stu-id="1107c-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="1107c-106">权限</span><span class="sxs-lookup"><span data-stu-id="1107c-106">Permissions</span></span>
<span data-ttu-id="1107c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1107c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1107c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1107c-109">Permission type</span></span>      | <span data-ttu-id="1107c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1107c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1107c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1107c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1107c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1107c-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1107c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1107c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1107c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1107c-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1107c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1107c-115">Application</span></span> | <span data-ttu-id="1107c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1107c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1107c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1107c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1107c-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="1107c-118">Optional request headers</span></span>
| <span data-ttu-id="1107c-119">名称</span><span class="sxs-lookup"><span data-stu-id="1107c-119">Name</span></span>       | <span data-ttu-id="1107c-120">说明</span><span class="sxs-lookup"><span data-stu-id="1107c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1107c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1107c-121">Authorization</span></span>  | <span data-ttu-id="1107c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1107c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1107c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1107c-124">Request body</span></span>
<span data-ttu-id="1107c-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1107c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1107c-128">属性</span><span class="sxs-lookup"><span data-stu-id="1107c-128">Property</span></span>     | <span data-ttu-id="1107c-129">类型</span><span class="sxs-lookup"><span data-stu-id="1107c-129">Type</span></span>   |<span data-ttu-id="1107c-130">说明</span><span class="sxs-lookup"><span data-stu-id="1107c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1107c-131">name</span><span class="sxs-lookup"><span data-stu-id="1107c-131">name</span></span>|<span data-ttu-id="1107c-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1107c-132">String</span></span>|<span data-ttu-id="1107c-133">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="1107c-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="1107c-134">响应</span><span class="sxs-lookup"><span data-stu-id="1107c-134">Response</span></span>

<span data-ttu-id="1107c-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1107c-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1107c-136">示例</span><span class="sxs-lookup"><span data-stu-id="1107c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1107c-137">请求</span><span class="sxs-lookup"><span data-stu-id="1107c-137">Request</span></span>
<span data-ttu-id="1107c-138">下面的示例将指定的任务文件夹的名称更改为`Charity work`。</span><span class="sxs-lookup"><span data-stu-id="1107c-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="1107c-139">响应</span><span class="sxs-lookup"><span data-stu-id="1107c-139">Response</span></span>
<span data-ttu-id="1107c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1107c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1107c-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1107c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1107c-144">语言</span><span class="sxs-lookup"><span data-stu-id="1107c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktaskfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1107c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="1107c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktaskfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
