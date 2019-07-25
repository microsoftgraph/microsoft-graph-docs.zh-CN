---
title: '笔记本: getNotebookFromWebUrl'
description: 使用 URL 路径检索笔记本对象的属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 1dbc907549fb84261c157e3415e6396a22b38672
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890176"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="275ff-103">笔记本: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="275ff-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="275ff-104">使用其 URL 路径检索[笔记本](../resources/notebook.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="275ff-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="275ff-105">该位置可以是 office 365 上的用户笔记本、组笔记本或 Office 365 上的 SharePoint 网站托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="275ff-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="275ff-106">权限</span><span class="sxs-lookup"><span data-stu-id="275ff-106">Permissions</span></span>
<span data-ttu-id="275ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="275ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="275ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="275ff-109">Permission type</span></span>      | <span data-ttu-id="275ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="275ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="275ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="275ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="275ff-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="275ff-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="275ff-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="275ff-113">Application</span></span> | <span data-ttu-id="275ff-114">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="275ff-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="275ff-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="275ff-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="275ff-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="275ff-116">Request headers</span></span>
| <span data-ttu-id="275ff-117">名称</span><span class="sxs-lookup"><span data-stu-id="275ff-117">Name</span></span>       | <span data-ttu-id="275ff-118">类型</span><span class="sxs-lookup"><span data-stu-id="275ff-118">Type</span></span> | <span data-ttu-id="275ff-119">说明</span><span class="sxs-lookup"><span data-stu-id="275ff-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="275ff-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="275ff-120">Authorization</span></span>  | <span data-ttu-id="275ff-121">string</span><span class="sxs-lookup"><span data-stu-id="275ff-121">string</span></span>  | <span data-ttu-id="275ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="275ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="275ff-124">接受</span><span class="sxs-lookup"><span data-stu-id="275ff-124">Accept</span></span> | <span data-ttu-id="275ff-125">string</span><span class="sxs-lookup"><span data-stu-id="275ff-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="275ff-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="275ff-126">Request body</span></span>
<span data-ttu-id="275ff-127">在请求正文中, 提供要检索的笔记本的完整 URL 路径的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="275ff-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="275ff-128">属性</span><span class="sxs-lookup"><span data-stu-id="275ff-128">Property</span></span>     | <span data-ttu-id="275ff-129">类型</span><span class="sxs-lookup"><span data-stu-id="275ff-129">Type</span></span>        | <span data-ttu-id="275ff-130">说明</span><span class="sxs-lookup"><span data-stu-id="275ff-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="275ff-131">要检索的笔记本的 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="275ff-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="275ff-132">它还可以包含 "onenote:" 前缀。</span><span class="sxs-lookup"><span data-stu-id="275ff-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="275ff-133">响应</span><span class="sxs-lookup"><span data-stu-id="275ff-133">Response</span></span>

<span data-ttu-id="275ff-134">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[笔记本](../resources/notebook.md)对象。</span><span class="sxs-lookup"><span data-stu-id="275ff-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="275ff-135">示例</span><span class="sxs-lookup"><span data-stu-id="275ff-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="275ff-136">请求</span><span class="sxs-lookup"><span data-stu-id="275ff-136">Request</span></span>
<span data-ttu-id="275ff-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="275ff-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="275ff-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="275ff-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="275ff-139">C#</span><span class="sxs-lookup"><span data-stu-id="275ff-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="275ff-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="275ff-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="275ff-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="275ff-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="275ff-142">Java</span><span class="sxs-lookup"><span data-stu-id="275ff-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-fromweburl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="275ff-143">响应</span><span class="sxs-lookup"><span data-stu-id="275ff-143">Response</span></span>
<span data-ttu-id="275ff-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="275ff-144">Here is an example of the response.</span></span> 

><span data-ttu-id="275ff-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="275ff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
