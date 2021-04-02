---
title: 创建笔记本
description: 新建 OneNote 笔记本。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5c944fb418fad689059cdc675cac4ee71a04ece7
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507713"
---
# <a name="create-notebook"></a><span data-ttu-id="c088c-103">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="c088c-103">Create notebook</span></span>

<span data-ttu-id="c088c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c088c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c088c-105">创建新的 OneNote [笔记本](../resources/notebook.md)。</span><span class="sxs-lookup"><span data-stu-id="c088c-105">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c088c-106">权限</span><span class="sxs-lookup"><span data-stu-id="c088c-106">Permissions</span></span>
<span data-ttu-id="c088c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c088c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c088c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c088c-109">Permission type</span></span>      | <span data-ttu-id="c088c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c088c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c088c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c088c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c088c-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c088c-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c088c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c088c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c088c-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c088c-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c088c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c088c-115">Application</span></span> | <span data-ttu-id="c088c-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c088c-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c088c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c088c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="c088c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c088c-118">Request headers</span></span>
| <span data-ttu-id="c088c-119">名称</span><span class="sxs-lookup"><span data-stu-id="c088c-119">Name</span></span>       | <span data-ttu-id="c088c-120">类型</span><span class="sxs-lookup"><span data-stu-id="c088c-120">Type</span></span> | <span data-ttu-id="c088c-121">说明</span><span class="sxs-lookup"><span data-stu-id="c088c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c088c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c088c-122">Authorization</span></span>  | <span data-ttu-id="c088c-123">string</span><span class="sxs-lookup"><span data-stu-id="c088c-123">string</span></span>  | <span data-ttu-id="c088c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c088c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c088c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c088c-126">Content-Type</span></span> | <span data-ttu-id="c088c-127">string</span><span class="sxs-lookup"><span data-stu-id="c088c-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c088c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c088c-128">Request body</span></span>
<span data-ttu-id="c088c-129">在请求正文中，提供笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="c088c-129">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="c088c-130">笔记本名称必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="c088c-130">Notebook names must be unique.</span></span> <span data-ttu-id="c088c-131">该名称不能包含超过 128 个字符或包含下列字符：？\* \/ ：<>|'"</span><span class="sxs-lookup"><span data-stu-id="c088c-131">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="c088c-132">响应</span><span class="sxs-lookup"><span data-stu-id="c088c-132">Response</span></span>

<span data-ttu-id="c088c-133">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码[](../resources/notebook.md)和新笔记本对象。</span><span class="sxs-lookup"><span data-stu-id="c088c-133">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c088c-134">示例</span><span class="sxs-lookup"><span data-stu-id="c088c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="c088c-135">请求</span><span class="sxs-lookup"><span data-stu-id="c088c-135">Request</span></span>
<span data-ttu-id="c088c-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c088c-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c088c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c088c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json

{
    "displayName": "My Private notebook"
}
```
# <a name="c"></a>[<span data-ttu-id="c088c-138">C#</span><span class="sxs-lookup"><span data-stu-id="c088c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-notebook-from-onenote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c088c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c088c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notebook-from-onenote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c088c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c088c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-notebook-from-onenote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c088c-141">Java</span><span class="sxs-lookup"><span data-stu-id="c088c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-notebook-from-onenote-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c088c-142">响应</span><span class="sxs-lookup"><span data-stu-id="c088c-142">Response</span></span>
<span data-ttu-id="c088c-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c088c-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('7d54cb02-aaa3-4016-9f9c-a4b49422dd9b')/onenote/notebooks/$entity",
    "id": "1-10143016-70dc-4449-b92a-3015225f800d",
    "self": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d",
    "displayName": "My Private notebook",
    "userRole": "Owner",
    "isShared": false,
    "sectionsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sections",
    "sectionGroupsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sectionGroups",
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
        },
        "oneNoteWebUrl": {
            "href": "https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
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


