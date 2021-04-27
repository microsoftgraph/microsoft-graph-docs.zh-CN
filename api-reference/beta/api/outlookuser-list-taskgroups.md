---
title: 列出 taskGroups
description: 获取Outlook邮箱中所有任务组。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0d79ec13b68e68ab11180db9a0826a12b79a61b3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052969"
---
# <a name="list-taskgroups-deprecated"></a><span data-ttu-id="d81db-103">列出已 (的任务组) </span><span class="sxs-lookup"><span data-stu-id="d81db-103">List taskGroups (deprecated)</span></span>

<span data-ttu-id="d81db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d81db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="d81db-105">获取Outlook邮箱中所有任务组。</span><span class="sxs-lookup"><span data-stu-id="d81db-105">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="d81db-106">该响应始终包括默认任务组 `My Tasks` ，以及已在邮箱中创建的其他任何任务组。</span><span class="sxs-lookup"><span data-stu-id="d81db-106">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="d81db-107">权限</span><span class="sxs-lookup"><span data-stu-id="d81db-107">Permissions</span></span>
<span data-ttu-id="d81db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d81db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d81db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d81db-110">Permission type</span></span>      | <span data-ttu-id="d81db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d81db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d81db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d81db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d81db-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d81db-113">Tasks.Read</span></span>    |
|<span data-ttu-id="d81db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d81db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81db-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d81db-115">Tasks.Read</span></span>    |
|<span data-ttu-id="d81db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d81db-116">Application</span></span> | <span data-ttu-id="d81db-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d81db-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d81db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d81db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d81db-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d81db-119">Optional query parameters</span></span>
<span data-ttu-id="d81db-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d81db-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d81db-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d81db-121">Request headers</span></span>
| <span data-ttu-id="d81db-122">名称</span><span class="sxs-lookup"><span data-stu-id="d81db-122">Name</span></span>      |<span data-ttu-id="d81db-123">说明</span><span class="sxs-lookup"><span data-stu-id="d81db-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d81db-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d81db-124">Authorization</span></span>  | <span data-ttu-id="d81db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d81db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d81db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d81db-127">Request body</span></span>
<span data-ttu-id="d81db-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d81db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d81db-129">响应</span><span class="sxs-lookup"><span data-stu-id="d81db-129">Response</span></span>

<span data-ttu-id="d81db-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d81db-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d81db-131">示例</span><span class="sxs-lookup"><span data-stu-id="d81db-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d81db-132">请求</span><span class="sxs-lookup"><span data-stu-id="d81db-132">Request</span></span>
<span data-ttu-id="d81db-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d81db-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d81db-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81db-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
# <a name="c"></a>[<span data-ttu-id="d81db-135">C#</span><span class="sxs-lookup"><span data-stu-id="d81db-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d81db-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81db-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d81db-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81db-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d81db-138">Java</span><span class="sxs-lookup"><span data-stu-id="d81db-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d81db-139">响应</span><span class="sxs-lookup"><span data-stu-id="d81db-139">Response</span></span>
<span data-ttu-id="d81db-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d81db-140">Here is an example of the response.</span></span> <span data-ttu-id="d81db-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d81db-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
