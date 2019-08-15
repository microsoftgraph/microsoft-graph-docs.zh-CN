---
title: 创建 outlookTaskGroup
description: 在用户的邮箱中创建一个 Outlook 任务组。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6540f9d88693e9111015808aa92649c742a15b86
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413904"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="90d4f-103">创建 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="90d4f-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90d4f-104">在用户的邮箱中创建一个 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="90d4f-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="90d4f-105">权限</span><span class="sxs-lookup"><span data-stu-id="90d4f-105">Permissions</span></span>
<span data-ttu-id="90d4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90d4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90d4f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="90d4f-108">Permission type</span></span>      | <span data-ttu-id="90d4f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90d4f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90d4f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90d4f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90d4f-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90d4f-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="90d4f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90d4f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90d4f-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90d4f-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="90d4f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="90d4f-114">Application</span></span> | <span data-ttu-id="90d4f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90d4f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90d4f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90d4f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="90d4f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="90d4f-117">Request headers</span></span>
| <span data-ttu-id="90d4f-118">名称</span><span class="sxs-lookup"><span data-stu-id="90d4f-118">Name</span></span>       | <span data-ttu-id="90d4f-119">说明</span><span class="sxs-lookup"><span data-stu-id="90d4f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90d4f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="90d4f-120">Authorization</span></span>  | <span data-ttu-id="90d4f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90d4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90d4f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="90d4f-123">Request body</span></span>
<span data-ttu-id="90d4f-124">在请求正文中, 提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90d4f-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="90d4f-125">响应</span><span class="sxs-lookup"><span data-stu-id="90d4f-125">Response</span></span>

<span data-ttu-id="90d4f-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90d4f-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90d4f-127">示例</span><span class="sxs-lookup"><span data-stu-id="90d4f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90d4f-128">请求</span><span class="sxs-lookup"><span data-stu-id="90d4f-128">Request</span></span>
<span data-ttu-id="90d4f-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90d4f-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90d4f-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="90d4f-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="90d4f-131">C#</span><span class="sxs-lookup"><span data-stu-id="90d4f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90d4f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90d4f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90d4f-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="90d4f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="90d4f-134">在请求正文中, 提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90d4f-134">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="90d4f-135">响应</span><span class="sxs-lookup"><span data-stu-id="90d4f-135">Response</span></span>
<span data-ttu-id="90d4f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90d4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
