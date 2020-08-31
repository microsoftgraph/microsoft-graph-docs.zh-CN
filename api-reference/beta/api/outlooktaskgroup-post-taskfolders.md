---
title: 创建 outlookTaskFolder
description: 在指定的 outlookTaskGroup 下创建 Outlook 任务文件夹。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 95c657c69b059e9049378d67382237b4080bc717
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311947"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="69633-103">创建 outlookTaskFolder (弃用) </span><span class="sxs-lookup"><span data-stu-id="69633-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="69633-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69633-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="69633-105">在指定的 [outlookTaskGroup](../resources/outlooktaskgroup.md)下创建 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="69633-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="69633-106">权限</span><span class="sxs-lookup"><span data-stu-id="69633-106">Permissions</span></span>
<span data-ttu-id="69633-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69633-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="69633-109">Permission type</span></span>      | <span data-ttu-id="69633-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69633-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69633-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69633-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69633-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69633-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="69633-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69633-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69633-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69633-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="69633-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="69633-115">Application</span></span> | <span data-ttu-id="69633-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69633-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69633-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69633-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="69633-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="69633-118">Request headers</span></span>
| <span data-ttu-id="69633-119">名称</span><span class="sxs-lookup"><span data-stu-id="69633-119">Name</span></span>       | <span data-ttu-id="69633-120">说明</span><span class="sxs-lookup"><span data-stu-id="69633-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69633-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69633-121">Authorization</span></span>  | <span data-ttu-id="69633-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69633-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69633-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="69633-124">Request body</span></span>
<span data-ttu-id="69633-125">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69633-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="69633-126">响应</span><span class="sxs-lookup"><span data-stu-id="69633-126">Response</span></span>

<span data-ttu-id="69633-127">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69633-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69633-128">示例</span><span class="sxs-lookup"><span data-stu-id="69633-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69633-129">请求</span><span class="sxs-lookup"><span data-stu-id="69633-129">Request</span></span>
<span data-ttu-id="69633-130">下面的示例创建一个 `Cooking` 在指定任务组中调用的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="69633-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>

# <a name="http"></a>[<span data-ttu-id="69633-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="69633-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="69633-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69633-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="69633-133">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69633-133">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="69633-134">响应</span><span class="sxs-lookup"><span data-stu-id="69633-134">Response</span></span>
<span data-ttu-id="69633-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69633-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
