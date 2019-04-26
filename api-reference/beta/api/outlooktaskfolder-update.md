---
title: 更新 outlooktaskfolder
description: 更新 Outlook 任务文件夹的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9b7727ce554e5dccb24dae78e73d4692330691dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337901"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="086ae-103">更新 outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="086ae-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="086ae-104">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="086ae-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="086ae-105">无法更改默认任务文件夹 "任务" 的 "**名称**" 属性值。</span><span class="sxs-lookup"><span data-stu-id="086ae-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="086ae-106">权限</span><span class="sxs-lookup"><span data-stu-id="086ae-106">Permissions</span></span>
<span data-ttu-id="086ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="086ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="086ae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="086ae-109">Permission type</span></span>      | <span data-ttu-id="086ae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="086ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="086ae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="086ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="086ae-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="086ae-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="086ae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="086ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="086ae-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="086ae-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="086ae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="086ae-115">Application</span></span> | <span data-ttu-id="086ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="086ae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="086ae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="086ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="086ae-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="086ae-118">Optional request headers</span></span>
| <span data-ttu-id="086ae-119">名称</span><span class="sxs-lookup"><span data-stu-id="086ae-119">Name</span></span>       | <span data-ttu-id="086ae-120">说明</span><span class="sxs-lookup"><span data-stu-id="086ae-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="086ae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="086ae-121">Authorization</span></span>  | <span data-ttu-id="086ae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="086ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="086ae-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="086ae-124">Request body</span></span>
<span data-ttu-id="086ae-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="086ae-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="086ae-128">属性</span><span class="sxs-lookup"><span data-stu-id="086ae-128">Property</span></span>     | <span data-ttu-id="086ae-129">类型</span><span class="sxs-lookup"><span data-stu-id="086ae-129">Type</span></span>   |<span data-ttu-id="086ae-130">说明</span><span class="sxs-lookup"><span data-stu-id="086ae-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="086ae-131">name</span><span class="sxs-lookup"><span data-stu-id="086ae-131">name</span></span>|<span data-ttu-id="086ae-132">String</span><span class="sxs-lookup"><span data-stu-id="086ae-132">String</span></span>|<span data-ttu-id="086ae-133">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="086ae-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="086ae-134">响应</span><span class="sxs-lookup"><span data-stu-id="086ae-134">Response</span></span>

<span data-ttu-id="086ae-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="086ae-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="086ae-136">示例</span><span class="sxs-lookup"><span data-stu-id="086ae-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="086ae-137">请求</span><span class="sxs-lookup"><span data-stu-id="086ae-137">Request</span></span>
<span data-ttu-id="086ae-138">下面的示例将指定的任务文件夹的名称更改为`Charity work`。</span><span class="sxs-lookup"><span data-stu-id="086ae-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
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
##### <a name="response"></a><span data-ttu-id="086ae-139">响应</span><span class="sxs-lookup"><span data-stu-id="086ae-139">Response</span></span>
<span data-ttu-id="086ae-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="086ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
