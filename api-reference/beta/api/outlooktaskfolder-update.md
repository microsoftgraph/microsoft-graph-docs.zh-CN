---
title: 更新 outlooktaskfolder
description: 更新 Outlook 任务文件夹的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dc8c04137ef2a8b9acafe852b411617794fbf19d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456136"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="67144-103">更新 outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="67144-103">Update outlooktaskfolder</span></span>

<span data-ttu-id="67144-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="67144-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67144-105">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="67144-105">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="67144-106">无法更改默认任务文件夹 "任务" 的 "**名称**" 属性值。</span><span class="sxs-lookup"><span data-stu-id="67144-106">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="67144-107">权限</span><span class="sxs-lookup"><span data-stu-id="67144-107">Permissions</span></span>
<span data-ttu-id="67144-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67144-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67144-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="67144-110">Permission type</span></span>      | <span data-ttu-id="67144-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67144-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67144-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67144-112">Delegated (work or school account)</span></span> | <span data-ttu-id="67144-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67144-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="67144-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67144-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67144-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67144-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="67144-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="67144-116">Application</span></span> | <span data-ttu-id="67144-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="67144-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67144-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67144-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="67144-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="67144-119">Optional request headers</span></span>
| <span data-ttu-id="67144-120">名称</span><span class="sxs-lookup"><span data-stu-id="67144-120">Name</span></span>       | <span data-ttu-id="67144-121">说明</span><span class="sxs-lookup"><span data-stu-id="67144-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="67144-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67144-122">Authorization</span></span>  | <span data-ttu-id="67144-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67144-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67144-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="67144-125">Request body</span></span>
<span data-ttu-id="67144-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="67144-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="67144-129">属性</span><span class="sxs-lookup"><span data-stu-id="67144-129">Property</span></span>     | <span data-ttu-id="67144-130">类型</span><span class="sxs-lookup"><span data-stu-id="67144-130">Type</span></span>   |<span data-ttu-id="67144-131">说明</span><span class="sxs-lookup"><span data-stu-id="67144-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67144-132">name</span><span class="sxs-lookup"><span data-stu-id="67144-132">name</span></span>|<span data-ttu-id="67144-133">String</span><span class="sxs-lookup"><span data-stu-id="67144-133">String</span></span>|<span data-ttu-id="67144-134">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="67144-134">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="67144-135">响应</span><span class="sxs-lookup"><span data-stu-id="67144-135">Response</span></span>

<span data-ttu-id="67144-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67144-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67144-137">示例</span><span class="sxs-lookup"><span data-stu-id="67144-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67144-138">请求</span><span class="sxs-lookup"><span data-stu-id="67144-138">Request</span></span>
<span data-ttu-id="67144-139">下面的示例将指定的任务文件夹的名称更改为`Charity work`。</span><span class="sxs-lookup"><span data-stu-id="67144-139">The following example changes the name of the specified task folder to `Charity work`.</span></span>

# <a name="http"></a>[<span data-ttu-id="67144-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="67144-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67144-141">C#</span><span class="sxs-lookup"><span data-stu-id="67144-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67144-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67144-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67144-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67144-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67144-144">响应</span><span class="sxs-lookup"><span data-stu-id="67144-144">Response</span></span>
<span data-ttu-id="67144-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67144-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->
