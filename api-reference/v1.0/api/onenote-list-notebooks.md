---
title: 列出笔记本
description: 检索 notebook 对象列表。
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9bf025494554c0fbf6e1c169479f76d9377489e6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461263"
---
# <a name="list-notebooks"></a><span data-ttu-id="6bb29-103">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="6bb29-103">List notebooks</span></span>

<span data-ttu-id="6bb29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bb29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6bb29-105">检索 [notebook](../resources/notebook.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="6bb29-105">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6bb29-106">权限</span><span class="sxs-lookup"><span data-stu-id="6bb29-106">Permissions</span></span>
<span data-ttu-id="6bb29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6bb29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bb29-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6bb29-109">Permission type</span></span>      | <span data-ttu-id="6bb29-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6bb29-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bb29-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6bb29-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6bb29-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb29-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6bb29-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6bb29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bb29-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bb29-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6bb29-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6bb29-115">Application</span></span> | <span data-ttu-id="6bb29-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb29-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bb29-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bb29-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6bb29-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6bb29-118">Optional query parameters</span></span>
<span data-ttu-id="6bb29-119">此方法支持 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6bb29-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="6bb29-120">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="6bb29-120">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="6bb29-121">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="6bb29-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bb29-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bb29-122">Request headers</span></span>
| <span data-ttu-id="6bb29-123">名称</span><span class="sxs-lookup"><span data-stu-id="6bb29-123">Name</span></span>       | <span data-ttu-id="6bb29-124">类型</span><span class="sxs-lookup"><span data-stu-id="6bb29-124">Type</span></span> | <span data-ttu-id="6bb29-125">说明</span><span class="sxs-lookup"><span data-stu-id="6bb29-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6bb29-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bb29-126">Authorization</span></span>  | <span data-ttu-id="6bb29-127">string</span><span class="sxs-lookup"><span data-stu-id="6bb29-127">string</span></span>  | <span data-ttu-id="6bb29-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6bb29-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6bb29-130">接受</span><span class="sxs-lookup"><span data-stu-id="6bb29-130">Accept</span></span> | <span data-ttu-id="6bb29-131">string</span><span class="sxs-lookup"><span data-stu-id="6bb29-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6bb29-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bb29-132">Request body</span></span>
<span data-ttu-id="6bb29-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6bb29-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bb29-134">响应</span><span class="sxs-lookup"><span data-stu-id="6bb29-134">Response</span></span>

<span data-ttu-id="6bb29-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6bb29-135">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6bb29-136">示例</span><span class="sxs-lookup"><span data-stu-id="6bb29-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6bb29-137">请求</span><span class="sxs-lookup"><span data-stu-id="6bb29-137">Request</span></span>
<span data-ttu-id="6bb29-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6bb29-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6bb29-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb29-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
# <a name="c"></a>[<span data-ttu-id="6bb29-140">C#</span><span class="sxs-lookup"><span data-stu-id="6bb29-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bb29-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bb29-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bb29-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bb29-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bb29-143">Java</span><span class="sxs-lookup"><span data-stu-id="6bb29-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6bb29-144">响应</span><span class="sxs-lookup"><span data-stu-id="6bb29-144">Response</span></span>
<span data-ttu-id="6bb29-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6bb29-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
