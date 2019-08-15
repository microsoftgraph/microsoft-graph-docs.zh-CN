---
title: '笔记本: getNotebookFromWebUrl'
description: 使用 URL 路径检索笔记本对象的属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 73e268acd5c397a2a956b73ec685ecdfa0effe30
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414789"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="76d57-103">笔记本: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="76d57-103">notebook: getNotebookFromWebUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d57-104">使用其 URL 路径检索[笔记本](../resources/notebook.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76d57-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="76d57-105">该位置可以是 office 365 上的用户笔记本、组笔记本或 Office 365 上的 SharePoint 网站托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="76d57-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="76d57-106">权限</span><span class="sxs-lookup"><span data-stu-id="76d57-106">Permissions</span></span>
<span data-ttu-id="76d57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76d57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76d57-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="76d57-109">Permission type</span></span>      | <span data-ttu-id="76d57-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76d57-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76d57-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76d57-111">Delegated (work or school account)</span></span> | <span data-ttu-id="76d57-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76d57-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="76d57-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="76d57-113">Application</span></span> | <span data-ttu-id="76d57-114">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76d57-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76d57-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76d57-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="76d57-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="76d57-116">Request headers</span></span>
| <span data-ttu-id="76d57-117">名称</span><span class="sxs-lookup"><span data-stu-id="76d57-117">Name</span></span>       | <span data-ttu-id="76d57-118">类型</span><span class="sxs-lookup"><span data-stu-id="76d57-118">Type</span></span> | <span data-ttu-id="76d57-119">说明</span><span class="sxs-lookup"><span data-stu-id="76d57-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="76d57-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76d57-120">Authorization</span></span>  | <span data-ttu-id="76d57-121">string</span><span class="sxs-lookup"><span data-stu-id="76d57-121">string</span></span>  | <span data-ttu-id="76d57-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76d57-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76d57-124">接受</span><span class="sxs-lookup"><span data-stu-id="76d57-124">Accept</span></span> | <span data-ttu-id="76d57-125">string</span><span class="sxs-lookup"><span data-stu-id="76d57-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="76d57-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="76d57-126">Request body</span></span>
<span data-ttu-id="76d57-127">在请求正文中, 提供要检索的笔记本的完整 URL 路径的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76d57-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="76d57-128">属性</span><span class="sxs-lookup"><span data-stu-id="76d57-128">Property</span></span>     | <span data-ttu-id="76d57-129">类型</span><span class="sxs-lookup"><span data-stu-id="76d57-129">Type</span></span>        | <span data-ttu-id="76d57-130">说明</span><span class="sxs-lookup"><span data-stu-id="76d57-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="76d57-131">要检索的笔记本的 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="76d57-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="76d57-132">它还可以包含 "onenote:" 前缀。</span><span class="sxs-lookup"><span data-stu-id="76d57-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="76d57-133">响应</span><span class="sxs-lookup"><span data-stu-id="76d57-133">Response</span></span>

<span data-ttu-id="76d57-134">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[笔记本](../resources/notebook.md)对象。</span><span class="sxs-lookup"><span data-stu-id="76d57-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76d57-135">示例</span><span class="sxs-lookup"><span data-stu-id="76d57-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76d57-136">请求</span><span class="sxs-lookup"><span data-stu-id="76d57-136">Request</span></span>
<span data-ttu-id="76d57-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76d57-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76d57-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="76d57-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76d57-139">C#</span><span class="sxs-lookup"><span data-stu-id="76d57-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76d57-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76d57-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76d57-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="76d57-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="76d57-142">响应</span><span class="sxs-lookup"><span data-stu-id="76d57-142">Response</span></span>
<span data-ttu-id="76d57-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="76d57-143">Here is an example of the response.</span></span> 

><span data-ttu-id="76d57-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="76d57-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
