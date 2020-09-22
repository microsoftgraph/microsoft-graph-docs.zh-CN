---
title: 创建笔记本
description: 新建 OneNote 笔记本。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: d129f8c6c8a740f44dcdddd29b3406e301dd6d42
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004688"
---
# <a name="create-notebook"></a><span data-ttu-id="db54b-103">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="db54b-103">Create notebook</span></span>

<span data-ttu-id="db54b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db54b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db54b-105">创建新的 OneNote [笔记本](../resources/notebook.md)。</span><span class="sxs-lookup"><span data-stu-id="db54b-105">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="db54b-106">权限</span><span class="sxs-lookup"><span data-stu-id="db54b-106">Permissions</span></span>
<span data-ttu-id="db54b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db54b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db54b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db54b-109">Permission type</span></span>      | <span data-ttu-id="db54b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db54b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db54b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db54b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db54b-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db54b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="db54b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db54b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db54b-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db54b-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="db54b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db54b-115">Application</span></span> | <span data-ttu-id="db54b-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db54b-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db54b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db54b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="db54b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db54b-118">Request headers</span></span>
| <span data-ttu-id="db54b-119">名称</span><span class="sxs-lookup"><span data-stu-id="db54b-119">Name</span></span>       | <span data-ttu-id="db54b-120">类型</span><span class="sxs-lookup"><span data-stu-id="db54b-120">Type</span></span> | <span data-ttu-id="db54b-121">说明</span><span class="sxs-lookup"><span data-stu-id="db54b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db54b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db54b-122">Authorization</span></span>  | <span data-ttu-id="db54b-123">string</span><span class="sxs-lookup"><span data-stu-id="db54b-123">string</span></span>  | <span data-ttu-id="db54b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db54b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db54b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db54b-126">Content-Type</span></span> | <span data-ttu-id="db54b-127">string</span><span class="sxs-lookup"><span data-stu-id="db54b-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="db54b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="db54b-128">Request body</span></span>
<span data-ttu-id="db54b-129">在请求正文中，提供笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="db54b-129">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="db54b-130">笔记本名称必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="db54b-130">Notebook names must be unique.</span></span> <span data-ttu-id="db54b-131">名称不能超过128个字符，也不能包含以下字符：？ \* \/ ： <>| ' "</span><span class="sxs-lookup"><span data-stu-id="db54b-131">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="db54b-132">响应</span><span class="sxs-lookup"><span data-stu-id="db54b-132">Response</span></span>

<span data-ttu-id="db54b-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [笔记本](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db54b-133">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db54b-134">示例</span><span class="sxs-lookup"><span data-stu-id="db54b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db54b-135">请求</span><span class="sxs-lookup"><span data-stu-id="db54b-135">Request</span></span>
<span data-ttu-id="db54b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db54b-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db54b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="db54b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```
# <a name="c"></a>[<span data-ttu-id="db54b-138">C#</span><span class="sxs-lookup"><span data-stu-id="db54b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-notebook-from-onenote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db54b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db54b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notebook-from-onenote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db54b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db54b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-notebook-from-onenote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db54b-141">响应</span><span class="sxs-lookup"><span data-stu-id="db54b-141">Response</span></span>
<span data-ttu-id="db54b-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db54b-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


