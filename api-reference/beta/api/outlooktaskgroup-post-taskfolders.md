---
title: 创建 outlookTaskFolder
description: 在指定的 outlookTaskGroup 下创建 Outlook 任务文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 59f6b6b2d12a68ded2cd22c8f859686f7b2fef20
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337920"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="455b4-103">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="455b4-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="455b4-104">在指定的[outlookTaskGroup](../resources/outlooktaskgroup.md)下创建 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="455b4-104">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="455b4-105">权限</span><span class="sxs-lookup"><span data-stu-id="455b4-105">Permissions</span></span>
<span data-ttu-id="455b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="455b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="455b4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="455b4-108">Permission type</span></span>      | <span data-ttu-id="455b4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="455b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="455b4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="455b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="455b4-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="455b4-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="455b4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="455b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="455b4-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="455b4-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="455b4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="455b4-114">Application</span></span> | <span data-ttu-id="455b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="455b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="455b4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="455b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="455b4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="455b4-117">Request headers</span></span>
| <span data-ttu-id="455b4-118">名称</span><span class="sxs-lookup"><span data-stu-id="455b4-118">Name</span></span>       | <span data-ttu-id="455b4-119">说明</span><span class="sxs-lookup"><span data-stu-id="455b4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="455b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="455b4-120">Authorization</span></span>  | <span data-ttu-id="455b4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="455b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="455b4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="455b4-123">Request body</span></span>
<span data-ttu-id="455b4-124">在请求正文中, 提供[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="455b4-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="455b4-125">响应</span><span class="sxs-lookup"><span data-stu-id="455b4-125">Response</span></span>

<span data-ttu-id="455b4-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="455b4-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="455b4-127">示例</span><span class="sxs-lookup"><span data-stu-id="455b4-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="455b4-128">请求</span><span class="sxs-lookup"><span data-stu-id="455b4-128">Request</span></span>
<span data-ttu-id="455b4-129">下面的示例创建一个在指定任务`Cooking`组中调用的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="455b4-129">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups/AAMkADIyAAAhrbe-AAA'/taskfolders
Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
<span data-ttu-id="455b4-130">在请求正文中, 提供[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="455b4-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="455b4-131">响应</span><span class="sxs-lookup"><span data-stu-id="455b4-131">Response</span></span>
<span data-ttu-id="455b4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="455b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
