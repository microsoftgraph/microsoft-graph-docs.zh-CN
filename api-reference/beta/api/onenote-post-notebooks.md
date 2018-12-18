---
title: 创建笔记本
description: 新建 OneNote 笔记本。
author: Jewan-microsoft
ms.openlocfilehash: e9290ed51f2ebf30cccaa8ecc82ab95767c9ed5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341599"
---
# <a name="create-notebook"></a><span data-ttu-id="0fd14-103">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="0fd14-103">Create notebook</span></span>

> <span data-ttu-id="0fd14-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0fd14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fd14-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0fd14-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fd14-106">新建 OneNote [笔记本](../resources/notebook.md)。</span><span class="sxs-lookup"><span data-stu-id="0fd14-106">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0fd14-107">权限</span><span class="sxs-lookup"><span data-stu-id="0fd14-107">Permissions</span></span>
<span data-ttu-id="0fd14-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fd14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fd14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fd14-110">Permission type</span></span>      | <span data-ttu-id="0fd14-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fd14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fd14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fd14-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0fd14-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fd14-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0fd14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fd14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fd14-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fd14-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0fd14-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fd14-116">Application</span></span> | <span data-ttu-id="0fd14-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fd14-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fd14-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fd14-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="0fd14-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fd14-119">Request headers</span></span>
| <span data-ttu-id="0fd14-120">Name</span><span class="sxs-lookup"><span data-stu-id="0fd14-120">Name</span></span>       | <span data-ttu-id="0fd14-121">类型</span><span class="sxs-lookup"><span data-stu-id="0fd14-121">Type</span></span> | <span data-ttu-id="0fd14-122">说明</span><span class="sxs-lookup"><span data-stu-id="0fd14-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0fd14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fd14-123">Authorization</span></span>  | <span data-ttu-id="0fd14-124">string</span><span class="sxs-lookup"><span data-stu-id="0fd14-124">string</span></span>  | <span data-ttu-id="0fd14-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0fd14-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0fd14-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fd14-127">Content-Type</span></span> | <span data-ttu-id="0fd14-128">string</span><span class="sxs-lookup"><span data-stu-id="0fd14-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0fd14-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fd14-129">Request body</span></span>
<span data-ttu-id="0fd14-130">在请求正文中，提供笔记本名称。</span><span class="sxs-lookup"><span data-stu-id="0fd14-130">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="0fd14-p104">笔记本名称必须是唯一的。该名称不能超过 128 个字符，也不能包含以下字符：?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="0fd14-p104">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="0fd14-133">响应</span><span class="sxs-lookup"><span data-stu-id="0fd14-133">Response</span></span>

<span data-ttu-id="0fd14-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新的 [notebook](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fd14-134">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fd14-135">示例</span><span class="sxs-lookup"><span data-stu-id="0fd14-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fd14-136">请求</span><span class="sxs-lookup"><span data-stu-id="0fd14-136">Request</span></span>
<span data-ttu-id="0fd14-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0fd14-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0fd14-138">响应</span><span class="sxs-lookup"><span data-stu-id="0fd14-138">Response</span></span>
<span data-ttu-id="0fd14-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0fd14-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->