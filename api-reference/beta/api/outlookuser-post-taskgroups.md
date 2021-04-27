---
title: 创建 outlookTaskGroup
description: 在Outlook创建一个任务组。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1cef21d441ba20c1bc97f7e4bf2e4f1c922d1f9c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037996"
---
# <a name="create-outlooktaskgroup-deprecated"></a><span data-ttu-id="04947-103">创建已弃 (outlookTaskGroup) </span><span class="sxs-lookup"><span data-stu-id="04947-103">Create outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="04947-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04947-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="04947-105">在Outlook创建一个任务组。</span><span class="sxs-lookup"><span data-stu-id="04947-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="04947-106">权限</span><span class="sxs-lookup"><span data-stu-id="04947-106">Permissions</span></span>
<span data-ttu-id="04947-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04947-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="04947-109">Permission type</span></span>      | <span data-ttu-id="04947-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04947-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04947-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04947-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04947-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04947-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="04947-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04947-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04947-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04947-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="04947-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="04947-115">Application</span></span> | <span data-ttu-id="04947-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04947-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04947-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04947-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="04947-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="04947-118">Request headers</span></span>
| <span data-ttu-id="04947-119">名称</span><span class="sxs-lookup"><span data-stu-id="04947-119">Name</span></span>       | <span data-ttu-id="04947-120">说明</span><span class="sxs-lookup"><span data-stu-id="04947-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04947-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04947-121">Authorization</span></span>  | <span data-ttu-id="04947-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04947-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04947-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="04947-124">Request body</span></span>
<span data-ttu-id="04947-125">在请求正文中，提供 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04947-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04947-126">响应</span><span class="sxs-lookup"><span data-stu-id="04947-126">Response</span></span>

<span data-ttu-id="04947-127">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04947-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04947-128">示例</span><span class="sxs-lookup"><span data-stu-id="04947-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04947-129">请求</span><span class="sxs-lookup"><span data-stu-id="04947-129">Request</span></span>
<span data-ttu-id="04947-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04947-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04947-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="04947-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="04947-132">C#</span><span class="sxs-lookup"><span data-stu-id="04947-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04947-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04947-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04947-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04947-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04947-135">Java</span><span class="sxs-lookup"><span data-stu-id="04947-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskgroup-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="04947-136">在请求正文中，提供 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04947-136">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="04947-137">响应</span><span class="sxs-lookup"><span data-stu-id="04947-137">Response</span></span>
<span data-ttu-id="04947-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="04947-138">Here is an example of the response.</span></span> <span data-ttu-id="04947-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="04947-139">Note: The response object shown here might be shortened for readability.</span></span>
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


