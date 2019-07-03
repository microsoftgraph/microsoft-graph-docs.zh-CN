---
title: 列出 taskFolders
description: 获取特定 outlookTaskGroup 中的 Outlook 任务文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1753a2bfe73c92d098c9f5201f70479975445635
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447227"
---
# <a name="list-taskfolders"></a><span data-ttu-id="fb7c0-103">列出 taskFolders</span><span class="sxs-lookup"><span data-stu-id="fb7c0-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb7c0-104">获取特定[outlookTaskGroup](../resources/outlooktaskgroup.md)中的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fb7c0-105">权限</span><span class="sxs-lookup"><span data-stu-id="fb7c0-105">Permissions</span></span>
<span data-ttu-id="fb7c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb7c0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb7c0-108">Permission type</span></span>      | <span data-ttu-id="fb7c0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb7c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb7c0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb7c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb7c0-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fb7c0-111">Tasks.Read</span></span>    |
|<span data-ttu-id="fb7c0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb7c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb7c0-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fb7c0-113">Tasks.Read</span></span>    |
|<span data-ttu-id="fb7c0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb7c0-114">Application</span></span> | <span data-ttu-id="fb7c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb7c0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb7c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb7c0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb7c0-117">Optional query parameters</span></span>
<span data-ttu-id="fb7c0-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb7c0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb7c0-119">Request headers</span></span>
| <span data-ttu-id="fb7c0-120">名称</span><span class="sxs-lookup"><span data-stu-id="fb7c0-120">Name</span></span>      |<span data-ttu-id="fb7c0-121">说明</span><span class="sxs-lookup"><span data-stu-id="fb7c0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fb7c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb7c0-122">Authorization</span></span>  | <span data-ttu-id="fb7c0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb7c0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb7c0-125">Request body</span></span>
<span data-ttu-id="fb7c0-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb7c0-127">响应</span><span class="sxs-lookup"><span data-stu-id="fb7c0-127">Response</span></span>

<span data-ttu-id="fb7c0-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb7c0-129">示例</span><span class="sxs-lookup"><span data-stu-id="fb7c0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb7c0-130">请求</span><span class="sxs-lookup"><span data-stu-id="fb7c0-130">Request</span></span>
<span data-ttu-id="fb7c0-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fb7c0-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fb7c0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb7c0-133">C#</span><span class="sxs-lookup"><span data-stu-id="fb7c0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb7c0-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="fb7c0-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb7c0-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="fb7c0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fb7c0-136">响应</span><span class="sxs-lookup"><span data-stu-id="fb7c0-136">Response</span></span>
<span data-ttu-id="fb7c0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb7c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
