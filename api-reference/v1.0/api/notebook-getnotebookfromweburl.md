---
title: notebook： getNotebookFromWebUrl
description: 使用笔记本对象 URL 路径检索其属性和关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e03c0d685d4f050b6f8401a6cdb46b5bacb387d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055881"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="865a5-103">notebook： getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="865a5-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="865a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="865a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="865a5-105">使用笔记本对象 URL [路径检索](../resources/notebook.md) 其属性和关系。</span><span class="sxs-lookup"><span data-stu-id="865a5-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="865a5-106">该位置可以是用户笔记本Microsoft 365、组笔记本或SharePoint托管的工作组笔记本上Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="865a5-106">The location can be user notebooks on Microsoft 365, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="865a5-107">权限</span><span class="sxs-lookup"><span data-stu-id="865a5-107">Permissions</span></span>
<span data-ttu-id="865a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="865a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="865a5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="865a5-110">Permission type</span></span>      | <span data-ttu-id="865a5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="865a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="865a5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="865a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="865a5-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="865a5-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="865a5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="865a5-114">Application</span></span> | <span data-ttu-id="865a5-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="865a5-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="865a5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="865a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="865a5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="865a5-117">Request headers</span></span>
| <span data-ttu-id="865a5-118">名称</span><span class="sxs-lookup"><span data-stu-id="865a5-118">Name</span></span>       | <span data-ttu-id="865a5-119">类型</span><span class="sxs-lookup"><span data-stu-id="865a5-119">Type</span></span> | <span data-ttu-id="865a5-120">说明</span><span class="sxs-lookup"><span data-stu-id="865a5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="865a5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="865a5-121">Authorization</span></span>  | <span data-ttu-id="865a5-122">string</span><span class="sxs-lookup"><span data-stu-id="865a5-122">string</span></span>  | <span data-ttu-id="865a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="865a5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="865a5-125">接受</span><span class="sxs-lookup"><span data-stu-id="865a5-125">Accept</span></span> | <span data-ttu-id="865a5-126">string</span><span class="sxs-lookup"><span data-stu-id="865a5-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="865a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="865a5-127">Request body</span></span>
<span data-ttu-id="865a5-128">在请求正文中，提供要检索的笔记本的完整 URL 路径的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="865a5-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="865a5-129">属性</span><span class="sxs-lookup"><span data-stu-id="865a5-129">Property</span></span>     | <span data-ttu-id="865a5-130">类型</span><span class="sxs-lookup"><span data-stu-id="865a5-130">Type</span></span>        | <span data-ttu-id="865a5-131">说明</span><span class="sxs-lookup"><span data-stu-id="865a5-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="865a5-132">要检索的笔记本的 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="865a5-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="865a5-133">它还可以包含"onenote："前缀。</span><span class="sxs-lookup"><span data-stu-id="865a5-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="865a5-134">响应</span><span class="sxs-lookup"><span data-stu-id="865a5-134">Response</span></span>

<span data-ttu-id="865a5-135">如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/notebook.md)代码和笔记本对象。</span><span class="sxs-lookup"><span data-stu-id="865a5-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="865a5-136">示例</span><span class="sxs-lookup"><span data-stu-id="865a5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="865a5-137">请求</span><span class="sxs-lookup"><span data-stu-id="865a5-137">Request</span></span>
<span data-ttu-id="865a5-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="865a5-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="865a5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="865a5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="c"></a>[<span data-ttu-id="865a5-140">C#</span><span class="sxs-lookup"><span data-stu-id="865a5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="865a5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="865a5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="865a5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="865a5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="865a5-143">Java</span><span class="sxs-lookup"><span data-stu-id="865a5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-fromweburl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="865a5-144">响应</span><span class="sxs-lookup"><span data-stu-id="865a5-144">Response</span></span>
<span data-ttu-id="865a5-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="865a5-145">Here is an example of the response.</span></span> 

><span data-ttu-id="865a5-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="865a5-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

