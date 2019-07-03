---
title: 获取 outlookTaskFolder
description: 获取指定的 Outlook 任务文件夹的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 687432d08b7dc9c24d59010d662c84fab6976f5a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447262"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="0e457-103">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="0e457-103">Get outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e457-104">获取指定的 Outlook 任务文件夹的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e457-104">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e457-105">权限</span><span class="sxs-lookup"><span data-stu-id="0e457-105">Permissions</span></span>
<span data-ttu-id="0e457-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e457-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e457-108">Permission type</span></span>      | <span data-ttu-id="0e457-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e457-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e457-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e457-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e457-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0e457-111">Tasks.Read</span></span>    |
|<span data-ttu-id="0e457-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e457-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e457-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0e457-113">Tasks.Read</span></span>    |
|<span data-ttu-id="0e457-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e457-114">Application</span></span> | <span data-ttu-id="0e457-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e457-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e457-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e457-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e457-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e457-117">Optional query parameters</span></span>
<span data-ttu-id="0e457-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e457-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e457-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e457-119">Request headers</span></span>
| <span data-ttu-id="0e457-120">名称</span><span class="sxs-lookup"><span data-stu-id="0e457-120">Name</span></span>      |<span data-ttu-id="0e457-121">说明</span><span class="sxs-lookup"><span data-stu-id="0e457-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e457-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e457-122">Authorization</span></span>  | <span data-ttu-id="0e457-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e457-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e457-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e457-125">Request body</span></span>
<span data-ttu-id="0e457-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e457-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e457-127">响应</span><span class="sxs-lookup"><span data-stu-id="0e457-127">Response</span></span>

<span data-ttu-id="0e457-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e457-128">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e457-129">示例</span><span class="sxs-lookup"><span data-stu-id="0e457-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e457-130">请求</span><span class="sxs-lookup"><span data-stu-id="0e457-130">Request</span></span>
<span data-ttu-id="0e457-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e457-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e457-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0e457-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e457-133">C#</span><span class="sxs-lookup"><span data-stu-id="0e457-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e457-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e457-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e457-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="0e457-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0e457-136">响应</span><span class="sxs-lookup"><span data-stu-id="0e457-136">Response</span></span>
<span data-ttu-id="0e457-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e457-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
