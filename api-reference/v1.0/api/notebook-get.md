---
title: 获取笔记本
description: 检索笔记本对象的属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 0f5c7553ef77ee114fab7fdc97ff757010192e04
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405062"
---
# <a name="get-notebook"></a><span data-ttu-id="f4036-103">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="f4036-103">Get notebook</span></span>

<span data-ttu-id="f4036-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4036-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4036-105">检索 [笔记本](../resources/notebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4036-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4036-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4036-106">Permissions</span></span>
<span data-ttu-id="f4036-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4036-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4036-109">Permission type</span></span>      | <span data-ttu-id="f4036-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4036-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4036-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4036-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4036-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4036-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4036-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4036-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4036-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4036-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f4036-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4036-115">Application</span></span> | <span data-ttu-id="f4036-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4036-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4036-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4036-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f4036-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4036-118">Optional query parameters</span></span>
<span data-ttu-id="f4036-119">此方法支持 `select` 和 `expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4036-119">This method supports the `select` and `expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="f4036-120">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="f4036-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4036-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4036-121">Request headers</span></span>
| <span data-ttu-id="f4036-122">名称</span><span class="sxs-lookup"><span data-stu-id="f4036-122">Name</span></span>       | <span data-ttu-id="f4036-123">类型</span><span class="sxs-lookup"><span data-stu-id="f4036-123">Type</span></span> | <span data-ttu-id="f4036-124">说明</span><span class="sxs-lookup"><span data-stu-id="f4036-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f4036-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4036-125">Authorization</span></span>  | <span data-ttu-id="f4036-126">string</span><span class="sxs-lookup"><span data-stu-id="f4036-126">string</span></span>  | <span data-ttu-id="f4036-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4036-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4036-129">接受</span><span class="sxs-lookup"><span data-stu-id="f4036-129">Accept</span></span> | <span data-ttu-id="f4036-130">string</span><span class="sxs-lookup"><span data-stu-id="f4036-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f4036-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4036-131">Request body</span></span>
<span data-ttu-id="f4036-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4036-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4036-133">响应</span><span class="sxs-lookup"><span data-stu-id="f4036-133">Response</span></span>

<span data-ttu-id="f4036-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [笔记本](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4036-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4036-135">示例</span><span class="sxs-lookup"><span data-stu-id="f4036-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4036-136">请求</span><span class="sxs-lookup"><span data-stu-id="f4036-136">Request</span></span>
<span data-ttu-id="f4036-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4036-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4036-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4036-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
# <a name="c"></a>[<span data-ttu-id="f4036-139">C#</span><span class="sxs-lookup"><span data-stu-id="f4036-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4036-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4036-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4036-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4036-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4036-142">Java</span><span class="sxs-lookup"><span data-stu-id="f4036-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f4036-143">响应</span><span class="sxs-lookup"><span data-stu-id="f4036-143">Response</span></span>
<span data-ttu-id="f4036-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4036-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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