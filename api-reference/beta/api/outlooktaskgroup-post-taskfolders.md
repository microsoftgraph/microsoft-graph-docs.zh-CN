---
title: 创建 outlookTaskFolder
description: 在Outlook outlookTaskGroup 下创建一个任务文件夹。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e7fd36eae4980a533f4d3bc02223bab788f8e7a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049217"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="00b93-103">创建已弃 (outlookTaskFolder) </span><span class="sxs-lookup"><span data-stu-id="00b93-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="00b93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00b93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="00b93-105">创建Outlook [outlookTaskGroup](../resources/outlooktaskgroup.md)下的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="00b93-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="00b93-106">权限</span><span class="sxs-lookup"><span data-stu-id="00b93-106">Permissions</span></span>
<span data-ttu-id="00b93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00b93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00b93-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="00b93-109">Permission type</span></span>      | <span data-ttu-id="00b93-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00b93-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00b93-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00b93-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00b93-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00b93-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="00b93-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00b93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00b93-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00b93-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="00b93-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="00b93-115">Application</span></span> | <span data-ttu-id="00b93-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="00b93-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00b93-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00b93-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="00b93-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="00b93-118">Request headers</span></span>
| <span data-ttu-id="00b93-119">名称</span><span class="sxs-lookup"><span data-stu-id="00b93-119">Name</span></span>       | <span data-ttu-id="00b93-120">说明</span><span class="sxs-lookup"><span data-stu-id="00b93-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00b93-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="00b93-121">Authorization</span></span>  | <span data-ttu-id="00b93-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00b93-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00b93-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="00b93-124">Request body</span></span>
<span data-ttu-id="00b93-125">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00b93-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00b93-126">响应</span><span class="sxs-lookup"><span data-stu-id="00b93-126">Response</span></span>

<span data-ttu-id="00b93-127">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00b93-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00b93-128">示例</span><span class="sxs-lookup"><span data-stu-id="00b93-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00b93-129">请求</span><span class="sxs-lookup"><span data-stu-id="00b93-129">Request</span></span>
<span data-ttu-id="00b93-130">下面的示例创建一个在指定的任务 `Cooking` 组中调用的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="00b93-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>


# <a name="http"></a>[<span data-ttu-id="00b93-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="00b93-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="00b93-132">C#</span><span class="sxs-lookup"><span data-stu-id="00b93-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00b93-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00b93-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00b93-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00b93-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00b93-135">Java</span><span class="sxs-lookup"><span data-stu-id="00b93-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="00b93-136">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00b93-136">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="00b93-137">响应</span><span class="sxs-lookup"><span data-stu-id="00b93-137">Response</span></span>
<span data-ttu-id="00b93-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="00b93-138">Here is an example of the response.</span></span> <span data-ttu-id="00b93-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="00b93-139">Note: The response object shown here might be shortened for readability.</span></span>
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


