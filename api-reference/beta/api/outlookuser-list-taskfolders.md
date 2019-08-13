---
title: 列出 taskFolders
description: 获取用户邮箱中的所有 Outlook 任务文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0c20da6fa5cb0a2e88cd5c233a43fca6a431deb6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346450"
---
# <a name="list-taskfolders"></a><span data-ttu-id="92842-103">列出 taskFolders</span><span class="sxs-lookup"><span data-stu-id="92842-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92842-104">获取用户邮箱中的所有 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="92842-104">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="92842-105">权限</span><span class="sxs-lookup"><span data-stu-id="92842-105">Permissions</span></span>
<span data-ttu-id="92842-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92842-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92842-108">Permission type</span></span>      | <span data-ttu-id="92842-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92842-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92842-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92842-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92842-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="92842-111">Tasks.Read</span></span>    |
|<span data-ttu-id="92842-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92842-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92842-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="92842-113">Tasks.Read</span></span>    |
|<span data-ttu-id="92842-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92842-114">Application</span></span> | <span data-ttu-id="92842-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92842-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92842-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92842-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92842-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92842-117">Optional query parameters</span></span>
<span data-ttu-id="92842-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92842-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92842-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="92842-119">Request headers</span></span>
| <span data-ttu-id="92842-120">名称</span><span class="sxs-lookup"><span data-stu-id="92842-120">Name</span></span>      |<span data-ttu-id="92842-121">说明</span><span class="sxs-lookup"><span data-stu-id="92842-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92842-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92842-122">Authorization</span></span>  | <span data-ttu-id="92842-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92842-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92842-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="92842-125">Request body</span></span>
<span data-ttu-id="92842-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92842-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92842-127">响应</span><span class="sxs-lookup"><span data-stu-id="92842-127">Response</span></span>

<span data-ttu-id="92842-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="92842-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92842-129">示例</span><span class="sxs-lookup"><span data-stu-id="92842-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92842-130">请求</span><span class="sxs-lookup"><span data-stu-id="92842-130">Request</span></span>
<span data-ttu-id="92842-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92842-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92842-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="92842-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92842-133">C#</span><span class="sxs-lookup"><span data-stu-id="92842-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92842-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92842-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92842-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="92842-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92842-136">Java</span><span class="sxs-lookup"><span data-stu-id="92842-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92842-137">响应</span><span class="sxs-lookup"><span data-stu-id="92842-137">Response</span></span>
<span data-ttu-id="92842-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92842-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
