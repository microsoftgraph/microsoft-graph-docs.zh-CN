---
title: 创建 outlookTaskGroup
description: 在用户的邮箱中创建一个 Outlook 任务组。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a352e301468713541cb6329df6932af10779597a
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312088"
---
# <a name="create-outlooktaskgroup-deprecated"></a><span data-ttu-id="3affd-103">创建 outlookTaskGroup (弃用) </span><span class="sxs-lookup"><span data-stu-id="3affd-103">Create outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="3affd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3affd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="3affd-105">在用户的邮箱中创建一个 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="3affd-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="3affd-106">权限</span><span class="sxs-lookup"><span data-stu-id="3affd-106">Permissions</span></span>
<span data-ttu-id="3affd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3affd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3affd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3affd-109">Permission type</span></span>      | <span data-ttu-id="3affd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3affd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3affd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3affd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3affd-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3affd-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3affd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3affd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3affd-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3affd-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3affd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3affd-115">Application</span></span> | <span data-ttu-id="3affd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3affd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3affd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3affd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="3affd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3affd-118">Request headers</span></span>
| <span data-ttu-id="3affd-119">名称</span><span class="sxs-lookup"><span data-stu-id="3affd-119">Name</span></span>       | <span data-ttu-id="3affd-120">说明</span><span class="sxs-lookup"><span data-stu-id="3affd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3affd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3affd-121">Authorization</span></span>  | <span data-ttu-id="3affd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3affd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3affd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3affd-124">Request body</span></span>
<span data-ttu-id="3affd-125">在请求正文中，提供 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3affd-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3affd-126">响应</span><span class="sxs-lookup"><span data-stu-id="3affd-126">Response</span></span>

<span data-ttu-id="3affd-127">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3affd-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3affd-128">示例</span><span class="sxs-lookup"><span data-stu-id="3affd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3affd-129">请求</span><span class="sxs-lookup"><span data-stu-id="3affd-129">Request</span></span>
<span data-ttu-id="3affd-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3affd-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3affd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3affd-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3affd-132">C#</span><span class="sxs-lookup"><span data-stu-id="3affd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3affd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3affd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3affd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3affd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3affd-135">在请求正文中，提供 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3affd-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3affd-136">响应</span><span class="sxs-lookup"><span data-stu-id="3affd-136">Response</span></span>
<span data-ttu-id="3affd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3affd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
