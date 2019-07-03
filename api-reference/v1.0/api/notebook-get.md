---
title: 获取笔记本
description: 检索笔记本对象的属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 253667910517dfac5ebb783b0071ef014de747a1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445189"
---
# <a name="get-notebook"></a><span data-ttu-id="e29c7-103">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="e29c7-103">Get notebook</span></span>

<span data-ttu-id="e29c7-104">检索[笔记本](../resources/notebook.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e29c7-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e29c7-105">权限</span><span class="sxs-lookup"><span data-stu-id="e29c7-105">Permissions</span></span>
<span data-ttu-id="e29c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e29c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e29c7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e29c7-108">Permission type</span></span>      | <span data-ttu-id="e29c7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e29c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e29c7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e29c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e29c7-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e29c7-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e29c7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e29c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e29c7-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e29c7-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e29c7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e29c7-114">Application</span></span> | <span data-ttu-id="e29c7-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e29c7-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e29c7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e29c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e29c7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e29c7-117">Optional query parameters</span></span>
<span data-ttu-id="e29c7-118">此方法支持`select`和`expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e29c7-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e29c7-119">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="e29c7-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e29c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e29c7-120">Request headers</span></span>
| <span data-ttu-id="e29c7-121">名称</span><span class="sxs-lookup"><span data-stu-id="e29c7-121">Name</span></span>       | <span data-ttu-id="e29c7-122">类型</span><span class="sxs-lookup"><span data-stu-id="e29c7-122">Type</span></span> | <span data-ttu-id="e29c7-123">说明</span><span class="sxs-lookup"><span data-stu-id="e29c7-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e29c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e29c7-124">Authorization</span></span>  | <span data-ttu-id="e29c7-125">string</span><span class="sxs-lookup"><span data-stu-id="e29c7-125">string</span></span>  | <span data-ttu-id="e29c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e29c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e29c7-128">接受</span><span class="sxs-lookup"><span data-stu-id="e29c7-128">Accept</span></span> | <span data-ttu-id="e29c7-129">string</span><span class="sxs-lookup"><span data-stu-id="e29c7-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e29c7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e29c7-130">Request body</span></span>
<span data-ttu-id="e29c7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e29c7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e29c7-132">响应</span><span class="sxs-lookup"><span data-stu-id="e29c7-132">Response</span></span>

<span data-ttu-id="e29c7-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[笔记本](../resources/notebook.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e29c7-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e29c7-134">示例</span><span class="sxs-lookup"><span data-stu-id="e29c7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e29c7-135">请求</span><span class="sxs-lookup"><span data-stu-id="e29c7-135">Request</span></span>
<span data-ttu-id="e29c7-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e29c7-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e29c7-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e29c7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e29c7-138">C#</span><span class="sxs-lookup"><span data-stu-id="e29c7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e29c7-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="e29c7-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e29c7-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="e29c7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e29c7-141">响应</span><span class="sxs-lookup"><span data-stu-id="e29c7-141">Response</span></span>
<span data-ttu-id="e29c7-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e29c7-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
