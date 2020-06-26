---
title: 笔记本： getNotebookFromWebUrl
description: 使用 URL 路径检索笔记本对象的属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6b42bd6425b35333f7f14021182bc4141497e1a1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44894821"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="f1848-103">笔记本： getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="f1848-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="f1848-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1848-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1848-105">使用其 URL 路径检索[笔记本](../resources/notebook.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1848-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="f1848-106">Microsoft 365 上的位置可以是 Microsoft 365、组笔记本或 SharePoint 网站托管的团队笔记本上的用户笔记本。</span><span class="sxs-lookup"><span data-stu-id="f1848-106">The location can be user notebooks on Microsoft 365, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1848-107">权限</span><span class="sxs-lookup"><span data-stu-id="f1848-107">Permissions</span></span>
<span data-ttu-id="f1848-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f1848-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f1848-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1848-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1848-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1848-110">Permission type</span></span>      | <span data-ttu-id="f1848-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1848-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1848-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1848-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1848-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1848-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1848-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1848-114">Application</span></span> | <span data-ttu-id="f1848-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1848-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1848-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1848-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="f1848-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1848-117">Request headers</span></span>
| <span data-ttu-id="f1848-118">名称</span><span class="sxs-lookup"><span data-stu-id="f1848-118">Name</span></span>       | <span data-ttu-id="f1848-119">类型</span><span class="sxs-lookup"><span data-stu-id="f1848-119">Type</span></span> | <span data-ttu-id="f1848-120">说明</span><span class="sxs-lookup"><span data-stu-id="f1848-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1848-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1848-121">Authorization</span></span>  | <span data-ttu-id="f1848-122">string</span><span class="sxs-lookup"><span data-stu-id="f1848-122">string</span></span>  | <span data-ttu-id="f1848-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f1848-123">Bearer {token}.</span></span> <span data-ttu-id="f1848-124">Required.</span><span class="sxs-lookup"><span data-stu-id="f1848-124">Required.</span></span> |
| <span data-ttu-id="f1848-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1848-125">Accept</span></span> | <span data-ttu-id="f1848-126">string</span><span class="sxs-lookup"><span data-stu-id="f1848-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f1848-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1848-127">Request body</span></span>
<span data-ttu-id="f1848-128">在请求正文中，提供要检索的笔记本的完整 URL 路径的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1848-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="f1848-129">属性</span><span class="sxs-lookup"><span data-stu-id="f1848-129">Property</span></span>     | <span data-ttu-id="f1848-130">类型</span><span class="sxs-lookup"><span data-stu-id="f1848-130">Type</span></span>        | <span data-ttu-id="f1848-131">说明</span><span class="sxs-lookup"><span data-stu-id="f1848-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="f1848-132">要检索的笔记本的 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="f1848-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="f1848-133">它还可以包含 "onenote：" 前缀。</span><span class="sxs-lookup"><span data-stu-id="f1848-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="f1848-134">响应</span><span class="sxs-lookup"><span data-stu-id="f1848-134">Response</span></span>

<span data-ttu-id="f1848-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[笔记本](../resources/notebook.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1848-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1848-136">示例</span><span class="sxs-lookup"><span data-stu-id="f1848-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1848-137">请求</span><span class="sxs-lookup"><span data-stu-id="f1848-137">Request</span></span>
<span data-ttu-id="f1848-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1848-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1848-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1848-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="c"></a>[<span data-ttu-id="f1848-140">C#</span><span class="sxs-lookup"><span data-stu-id="f1848-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1848-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1848-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1848-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1848-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1848-143">响应</span><span class="sxs-lookup"><span data-stu-id="f1848-143">Response</span></span>
<span data-ttu-id="f1848-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f1848-144">Here is an example of the response.</span></span> 

><span data-ttu-id="f1848-145">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="f1848-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1848-146">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f1848-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
