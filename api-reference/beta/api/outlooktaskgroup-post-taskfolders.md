---
title: 创建 outlookTaskFolder
description: 在指定的 outlookTaskGroup 下创建 Outlook 任务文件夹。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 285178adb4f0df591e1d1270d60b572f346d57e1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472893"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="698d9-103">创建 outlookTaskFolder (已弃) </span><span class="sxs-lookup"><span data-stu-id="698d9-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="698d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="698d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="698d9-105">在指定的 [outlookTaskGroup](../resources/outlooktaskgroup.md)下创建 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="698d9-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="698d9-106">权限</span><span class="sxs-lookup"><span data-stu-id="698d9-106">Permissions</span></span>
<span data-ttu-id="698d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="698d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="698d9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="698d9-109">Permission type</span></span>      | <span data-ttu-id="698d9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="698d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="698d9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="698d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="698d9-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="698d9-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="698d9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="698d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="698d9-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="698d9-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="698d9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="698d9-115">Application</span></span> | <span data-ttu-id="698d9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="698d9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="698d9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="698d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="698d9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="698d9-118">Request headers</span></span>
| <span data-ttu-id="698d9-119">名称</span><span class="sxs-lookup"><span data-stu-id="698d9-119">Name</span></span>       | <span data-ttu-id="698d9-120">说明</span><span class="sxs-lookup"><span data-stu-id="698d9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="698d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="698d9-121">Authorization</span></span>  | <span data-ttu-id="698d9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="698d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="698d9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="698d9-124">Request body</span></span>
<span data-ttu-id="698d9-125">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="698d9-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="698d9-126">响应</span><span class="sxs-lookup"><span data-stu-id="698d9-126">Response</span></span>

<span data-ttu-id="698d9-127">如果成功，此方法在响应正文中返回响应代码 `201 Created` 和 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="698d9-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="698d9-128">示例</span><span class="sxs-lookup"><span data-stu-id="698d9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="698d9-129">请求</span><span class="sxs-lookup"><span data-stu-id="698d9-129">Request</span></span>
<span data-ttu-id="698d9-130">以下示例创建一个指定任务 `Cooking` 组中调用的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="698d9-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=/taskfolders
Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```

<span data-ttu-id="698d9-131">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="698d9-131">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="698d9-132">响应</span><span class="sxs-lookup"><span data-stu-id="698d9-132">Response</span></span>
<span data-ttu-id="698d9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="698d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


