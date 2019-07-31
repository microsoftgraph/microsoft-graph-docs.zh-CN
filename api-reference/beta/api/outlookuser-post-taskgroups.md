---
title: 创建 outlookTaskGroup
description: 在用户的邮箱中创建一个 Outlook 任务组。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e99444cdfeb6638734674e2afcec7fc256cf9277
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992414"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="69359-103">创建 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="69359-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69359-104">在用户的邮箱中创建一个 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="69359-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="69359-105">权限</span><span class="sxs-lookup"><span data-stu-id="69359-105">Permissions</span></span>
<span data-ttu-id="69359-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69359-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="69359-108">Permission type</span></span>      | <span data-ttu-id="69359-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69359-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69359-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69359-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69359-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69359-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="69359-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69359-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69359-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69359-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="69359-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="69359-114">Application</span></span> | <span data-ttu-id="69359-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69359-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69359-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69359-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="69359-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="69359-117">Request headers</span></span>
| <span data-ttu-id="69359-118">名称</span><span class="sxs-lookup"><span data-stu-id="69359-118">Name</span></span>       | <span data-ttu-id="69359-119">说明</span><span class="sxs-lookup"><span data-stu-id="69359-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69359-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="69359-120">Authorization</span></span>  | <span data-ttu-id="69359-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69359-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69359-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="69359-123">Request body</span></span>
<span data-ttu-id="69359-124">在请求正文中, 提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69359-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="69359-125">响应</span><span class="sxs-lookup"><span data-stu-id="69359-125">Response</span></span>

<span data-ttu-id="69359-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69359-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69359-127">示例</span><span class="sxs-lookup"><span data-stu-id="69359-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69359-128">请求</span><span class="sxs-lookup"><span data-stu-id="69359-128">Request</span></span>
<span data-ttu-id="69359-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69359-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="69359-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="69359-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="69359-131">C#</span><span class="sxs-lookup"><span data-stu-id="69359-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69359-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="69359-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69359-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="69359-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="69359-134">Java</span><span class="sxs-lookup"><span data-stu-id="69359-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskgroup-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="69359-135">在请求正文中, 提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69359-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="69359-136">响应</span><span class="sxs-lookup"><span data-stu-id="69359-136">Response</span></span>
<span data-ttu-id="69359-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69359-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
