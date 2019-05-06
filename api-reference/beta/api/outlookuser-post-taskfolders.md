---
title: 创建 outlookTaskFolder
description: 在用户邮箱的默认任务组 (`My Tasks`) 中创建一个任务文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c3eb5f82c0dd68a2f4db8d35ba1f4d6ba0a02e99
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596235"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="983bb-103">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="983bb-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="983bb-104">在用户邮箱的默认任务组 (`My Tasks`) 中创建一个任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="983bb-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="983bb-105">权限</span><span class="sxs-lookup"><span data-stu-id="983bb-105">Permissions</span></span>
<span data-ttu-id="983bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="983bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="983bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="983bb-108">Permission type</span></span>      | <span data-ttu-id="983bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="983bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="983bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="983bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="983bb-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="983bb-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="983bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="983bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="983bb-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="983bb-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="983bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="983bb-114">Application</span></span> | <span data-ttu-id="983bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="983bb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="983bb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="983bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="983bb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="983bb-117">Request headers</span></span>
| <span data-ttu-id="983bb-118">名称</span><span class="sxs-lookup"><span data-stu-id="983bb-118">Name</span></span>       | <span data-ttu-id="983bb-119">说明</span><span class="sxs-lookup"><span data-stu-id="983bb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="983bb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="983bb-120">Authorization</span></span>  | <span data-ttu-id="983bb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="983bb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="983bb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="983bb-123">Request body</span></span>
<span data-ttu-id="983bb-124">在请求正文中, 提供[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="983bb-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="983bb-125">响应</span><span class="sxs-lookup"><span data-stu-id="983bb-125">Response</span></span>

<span data-ttu-id="983bb-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="983bb-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="983bb-127">示例</span><span class="sxs-lookup"><span data-stu-id="983bb-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="983bb-128">请求</span><span class="sxs-lookup"><span data-stu-id="983bb-128">Request</span></span>
<span data-ttu-id="983bb-129">下面的示例在用户邮箱的默认任务组 (`My Tasks`) 中创建名为 "志愿者" 的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="983bb-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
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
<span data-ttu-id="983bb-130">在请求正文中, 提供[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="983bb-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="983bb-131">响应</span><span class="sxs-lookup"><span data-stu-id="983bb-131">Response</span></span>
<span data-ttu-id="983bb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="983bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="983bb-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="983bb-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="983bb-136">语言</span><span class="sxs-lookup"><span data-stu-id="983bb-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktaskfolder_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="983bb-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="983bb-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktaskfolder_from_outlookuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
