---
title: 创建 outlookTaskFolder
description: 在默认任务组中创建任务文件夹 (`My Tasks` 用户邮箱的) 。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0dcd011121d830af83cc894c0dc47c44fa8c3d02
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980992"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="fc760-103">创建 outlookTaskFolder (弃用) </span><span class="sxs-lookup"><span data-stu-id="fc760-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="fc760-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc760-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="fc760-105">在默认任务组中创建任务文件夹 (`My Tasks` 用户邮箱的) 。</span><span class="sxs-lookup"><span data-stu-id="fc760-105">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc760-106">权限</span><span class="sxs-lookup"><span data-stu-id="fc760-106">Permissions</span></span>
<span data-ttu-id="fc760-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc760-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc760-109">Permission type</span></span>      | <span data-ttu-id="fc760-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc760-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc760-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc760-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc760-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc760-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="fc760-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc760-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc760-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc760-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="fc760-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc760-115">Application</span></span> | <span data-ttu-id="fc760-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc760-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc760-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc760-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="fc760-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc760-118">Request headers</span></span>
| <span data-ttu-id="fc760-119">名称</span><span class="sxs-lookup"><span data-stu-id="fc760-119">Name</span></span>       | <span data-ttu-id="fc760-120">说明</span><span class="sxs-lookup"><span data-stu-id="fc760-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc760-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc760-121">Authorization</span></span>  | <span data-ttu-id="fc760-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc760-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc760-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc760-124">Request body</span></span>
<span data-ttu-id="fc760-125">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc760-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fc760-126">响应</span><span class="sxs-lookup"><span data-stu-id="fc760-126">Response</span></span>

<span data-ttu-id="fc760-127">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc760-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc760-128">示例</span><span class="sxs-lookup"><span data-stu-id="fc760-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc760-129">请求</span><span class="sxs-lookup"><span data-stu-id="fc760-129">Request</span></span>
<span data-ttu-id="fc760-130">下面的示例在用户邮箱的默认任务组 () 中创建名为 "志愿者" 的任务文件夹 `My Tasks` 。</span><span class="sxs-lookup"><span data-stu-id="fc760-130">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc760-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc760-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
# <a name="c"></a>[<span data-ttu-id="fc760-132">C#</span><span class="sxs-lookup"><span data-stu-id="fc760-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc760-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc760-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc760-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc760-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc760-135">Java</span><span class="sxs-lookup"><span data-stu-id="fc760-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fc760-136">在请求正文中，提供 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc760-136">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fc760-137">响应</span><span class="sxs-lookup"><span data-stu-id="fc760-137">Response</span></span>
<span data-ttu-id="fc760-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc760-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
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
  "suppressions": [
  ]
}
-->


