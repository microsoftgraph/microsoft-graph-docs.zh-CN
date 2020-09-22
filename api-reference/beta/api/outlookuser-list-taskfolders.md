---
title: 列出 taskFolders
description: 获取用户邮箱中的所有 Outlook 任务文件夹。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8c0de2ef734922003fb17e5e6a94ddaf9de4831a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027533"
---
# <a name="list-taskfolders-deprecated"></a><span data-ttu-id="8d05a-103">列出 taskFolders (弃用) </span><span class="sxs-lookup"><span data-stu-id="8d05a-103">List taskFolders (deprecated)</span></span>

<span data-ttu-id="8d05a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d05a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="8d05a-105">获取用户邮箱中的所有 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="8d05a-105">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d05a-106">权限</span><span class="sxs-lookup"><span data-stu-id="8d05a-106">Permissions</span></span>
<span data-ttu-id="8d05a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d05a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d05a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d05a-109">Permission type</span></span>      | <span data-ttu-id="8d05a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d05a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d05a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d05a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d05a-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8d05a-112">Tasks.Read</span></span>    |
|<span data-ttu-id="8d05a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d05a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d05a-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8d05a-114">Tasks.Read</span></span>    |
|<span data-ttu-id="8d05a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d05a-115">Application</span></span> | <span data-ttu-id="8d05a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d05a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d05a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d05a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d05a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d05a-118">Optional query parameters</span></span>
<span data-ttu-id="8d05a-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8d05a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d05a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d05a-120">Request headers</span></span>
| <span data-ttu-id="8d05a-121">名称</span><span class="sxs-lookup"><span data-stu-id="8d05a-121">Name</span></span>      |<span data-ttu-id="8d05a-122">说明</span><span class="sxs-lookup"><span data-stu-id="8d05a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d05a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d05a-123">Authorization</span></span>  | <span data-ttu-id="8d05a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d05a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d05a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d05a-126">Request body</span></span>
<span data-ttu-id="8d05a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d05a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d05a-128">响应</span><span class="sxs-lookup"><span data-stu-id="8d05a-128">Response</span></span>

<span data-ttu-id="8d05a-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [outlookTaskFolder](../resources/outlooktaskfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d05a-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d05a-130">示例</span><span class="sxs-lookup"><span data-stu-id="8d05a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d05a-131">请求</span><span class="sxs-lookup"><span data-stu-id="8d05a-131">Request</span></span>
<span data-ttu-id="8d05a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d05a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d05a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d05a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
# <a name="c"></a>[<span data-ttu-id="8d05a-134">C#</span><span class="sxs-lookup"><span data-stu-id="8d05a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d05a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d05a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d05a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d05a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8d05a-137">响应</span><span class="sxs-lookup"><span data-stu-id="8d05a-137">Response</span></span>
<span data-ttu-id="8d05a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d05a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
   {
      "id": "AAMkADIyAAAAABrJAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
      "isDefaultFolder": false,
      "name": "Monthly tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAAAAESAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAAPA==",
      "isDefaultFolder": true,
      "name": "Tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


