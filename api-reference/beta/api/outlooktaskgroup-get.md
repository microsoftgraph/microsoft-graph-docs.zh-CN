---
title: 获取 outlookTaskGroup
description: 获取指定任务组Outlook关系。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6abb0d4103cf63fc0ff48a8070cc81c32469f139
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049210"
---
# <a name="get-outlooktaskgroup-deprecated"></a><span data-ttu-id="225dc-103">获取已 (outlookTaskGroup) </span><span class="sxs-lookup"><span data-stu-id="225dc-103">Get outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="225dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="225dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="225dc-105">获取指定任务组Outlook关系。</span><span class="sxs-lookup"><span data-stu-id="225dc-105">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="225dc-106">权限</span><span class="sxs-lookup"><span data-stu-id="225dc-106">Permissions</span></span>
<span data-ttu-id="225dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="225dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="225dc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="225dc-109">Permission type</span></span>      | <span data-ttu-id="225dc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="225dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="225dc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="225dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="225dc-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="225dc-112">Tasks.Read</span></span>    |
|<span data-ttu-id="225dc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="225dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="225dc-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="225dc-114">Tasks.Read</span></span>    |
|<span data-ttu-id="225dc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="225dc-115">Application</span></span> | <span data-ttu-id="225dc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="225dc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="225dc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="225dc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="225dc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="225dc-118">Optional query parameters</span></span>
<span data-ttu-id="225dc-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="225dc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="225dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="225dc-120">Request headers</span></span>
| <span data-ttu-id="225dc-121">名称</span><span class="sxs-lookup"><span data-stu-id="225dc-121">Name</span></span>      |<span data-ttu-id="225dc-122">说明</span><span class="sxs-lookup"><span data-stu-id="225dc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="225dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="225dc-123">Authorization</span></span>  | <span data-ttu-id="225dc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="225dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="225dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="225dc-126">Request body</span></span>
<span data-ttu-id="225dc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="225dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="225dc-128">响应</span><span class="sxs-lookup"><span data-stu-id="225dc-128">Response</span></span>

<span data-ttu-id="225dc-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [outlookTaskGroup](../resources/outlooktaskgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="225dc-129">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="225dc-130">示例</span><span class="sxs-lookup"><span data-stu-id="225dc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="225dc-131">请求</span><span class="sxs-lookup"><span data-stu-id="225dc-131">Request</span></span>
<span data-ttu-id="225dc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="225dc-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="225dc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="225dc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="225dc-134">C#</span><span class="sxs-lookup"><span data-stu-id="225dc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="225dc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="225dc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="225dc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="225dc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="225dc-137">Java</span><span class="sxs-lookup"><span data-stu-id="225dc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="225dc-138">响应</span><span class="sxs-lookup"><span data-stu-id="225dc-138">Response</span></span>
<span data-ttu-id="225dc-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="225dc-139">Here is an example of the response.</span></span> <span data-ttu-id="225dc-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="225dc-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
