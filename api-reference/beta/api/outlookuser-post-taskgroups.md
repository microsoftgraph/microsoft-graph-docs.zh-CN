---
title: 创建 outlookTaskGroup
description: 在用户的邮箱中创建一个 Outlook 任务组。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7fadfbb0ff448b74d02460d6437a92d5cee327d3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265658"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="a85fa-103">创建 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a85fa-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a85fa-104">在用户的邮箱中创建一个 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="a85fa-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="a85fa-105">权限</span><span class="sxs-lookup"><span data-stu-id="a85fa-105">Permissions</span></span>
<span data-ttu-id="a85fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a85fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a85fa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a85fa-108">Permission type</span></span>      | <span data-ttu-id="a85fa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a85fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a85fa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a85fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a85fa-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a85fa-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a85fa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a85fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a85fa-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a85fa-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a85fa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a85fa-114">Application</span></span> | <span data-ttu-id="a85fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a85fa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a85fa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a85fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="a85fa-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a85fa-117">Request headers</span></span>
| <span data-ttu-id="a85fa-118">名称</span><span class="sxs-lookup"><span data-stu-id="a85fa-118">Name</span></span>       | <span data-ttu-id="a85fa-119">说明</span><span class="sxs-lookup"><span data-stu-id="a85fa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a85fa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a85fa-120">Authorization</span></span>  | <span data-ttu-id="a85fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a85fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a85fa-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a85fa-123">Request body</span></span>
<span data-ttu-id="a85fa-124">在请求正文中, 提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a85fa-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a85fa-125">响应</span><span class="sxs-lookup"><span data-stu-id="a85fa-125">Response</span></span>

<span data-ttu-id="a85fa-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a85fa-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a85fa-127">示例</span><span class="sxs-lookup"><span data-stu-id="a85fa-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a85fa-128">请求</span><span class="sxs-lookup"><span data-stu-id="a85fa-128">Request</span></span>
<span data-ttu-id="a85fa-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a85fa-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
<span data-ttu-id="a85fa-130">在请求正文中, 提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a85fa-130">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a85fa-131">响应</span><span class="sxs-lookup"><span data-stu-id="a85fa-131">Response</span></span>
<span data-ttu-id="a85fa-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a85fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a85fa-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a85fa-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a85fa-136">C#</span><span class="sxs-lookup"><span data-stu-id="a85fa-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktaskgroup_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a85fa-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a85fa-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktaskgroup_from_outlookuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a85fa-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="a85fa-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_outlooktaskgroup_from_outlookuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
