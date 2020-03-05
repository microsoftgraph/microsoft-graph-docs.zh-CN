---
title: 获取 outlookTaskFolder
description: 获取指定的 Outlook 任务文件夹的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 19ce6ee84c272da4e3e80d31b89b8ac593f19608
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456157"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="42eb5-103">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="42eb5-103">Get outlookTaskFolder</span></span>

<span data-ttu-id="42eb5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="42eb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42eb5-105">获取指定的 Outlook 任务文件夹的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42eb5-105">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="42eb5-106">权限</span><span class="sxs-lookup"><span data-stu-id="42eb5-106">Permissions</span></span>
<span data-ttu-id="42eb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42eb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42eb5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="42eb5-109">Permission type</span></span>      | <span data-ttu-id="42eb5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42eb5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42eb5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42eb5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42eb5-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="42eb5-112">Tasks.Read</span></span>    |
|<span data-ttu-id="42eb5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42eb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42eb5-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="42eb5-114">Tasks.Read</span></span>    |
|<span data-ttu-id="42eb5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="42eb5-115">Application</span></span> | <span data-ttu-id="42eb5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42eb5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42eb5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42eb5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42eb5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="42eb5-118">Optional query parameters</span></span>
<span data-ttu-id="42eb5-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="42eb5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42eb5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42eb5-120">Request headers</span></span>
| <span data-ttu-id="42eb5-121">名称</span><span class="sxs-lookup"><span data-stu-id="42eb5-121">Name</span></span>      |<span data-ttu-id="42eb5-122">说明</span><span class="sxs-lookup"><span data-stu-id="42eb5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42eb5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42eb5-123">Authorization</span></span>  | <span data-ttu-id="42eb5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42eb5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42eb5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42eb5-126">Request body</span></span>
<span data-ttu-id="42eb5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42eb5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42eb5-128">响应</span><span class="sxs-lookup"><span data-stu-id="42eb5-128">Response</span></span>

<span data-ttu-id="42eb5-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="42eb5-129">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42eb5-130">示例</span><span class="sxs-lookup"><span data-stu-id="42eb5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42eb5-131">请求</span><span class="sxs-lookup"><span data-stu-id="42eb5-131">Request</span></span>
<span data-ttu-id="42eb5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42eb5-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42eb5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="42eb5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="42eb5-134">C#</span><span class="sxs-lookup"><span data-stu-id="42eb5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42eb5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42eb5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42eb5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42eb5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42eb5-137">响应</span><span class="sxs-lookup"><span data-stu-id="42eb5-137">Response</span></span>
<span data-ttu-id="42eb5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42eb5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
