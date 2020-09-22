---
title: 创建分区
description: 在指定的笔记本中新建分区。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f6f0f659d508616b90740d41906429858df2b68f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053480"
---
# <a name="create-section"></a><span data-ttu-id="4afc4-103">创建分区</span><span class="sxs-lookup"><span data-stu-id="4afc4-103">Create section</span></span>

<span data-ttu-id="4afc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4afc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4afc4-105">在指定的笔记本中新建[分区](../resources/onenotesection.md)。</span><span class="sxs-lookup"><span data-stu-id="4afc4-105">Create a new [section](../resources/onenotesection.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="4afc4-106">权限</span><span class="sxs-lookup"><span data-stu-id="4afc4-106">Permissions</span></span>
<span data-ttu-id="4afc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4afc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4afc4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4afc4-109">Permission type</span></span>      | <span data-ttu-id="4afc4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4afc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4afc4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4afc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4afc4-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4afc4-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4afc4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4afc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4afc4-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4afc4-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4afc4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4afc4-115">Application</span></span> | <span data-ttu-id="4afc4-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4afc4-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4afc4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4afc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="4afc4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4afc4-118">Request headers</span></span>
| <span data-ttu-id="4afc4-119">名称</span><span class="sxs-lookup"><span data-stu-id="4afc4-119">Name</span></span>       | <span data-ttu-id="4afc4-120">类型</span><span class="sxs-lookup"><span data-stu-id="4afc4-120">Type</span></span> | <span data-ttu-id="4afc4-121">说明</span><span class="sxs-lookup"><span data-stu-id="4afc4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4afc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4afc4-122">Authorization</span></span>  | <span data-ttu-id="4afc4-123">string</span><span class="sxs-lookup"><span data-stu-id="4afc4-123">string</span></span>  | <span data-ttu-id="4afc4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4afc4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4afc4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4afc4-126">Content-Type</span></span> | <span data-ttu-id="4afc4-127">string</span><span class="sxs-lookup"><span data-stu-id="4afc4-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4afc4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4afc4-128">Request body</span></span>
<span data-ttu-id="4afc4-129">在请求正文中，提供分区名称。</span><span class="sxs-lookup"><span data-stu-id="4afc4-129">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="4afc4-p103">在同一个层次结构级别中，分区名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="4afc4-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="4afc4-132">响应</span><span class="sxs-lookup"><span data-stu-id="4afc4-132">Response</span></span>

<span data-ttu-id="4afc4-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [onenoteSection](../resources/onenotesection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4afc4-133">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4afc4-134">示例</span><span class="sxs-lookup"><span data-stu-id="4afc4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4afc4-135">请求</span><span class="sxs-lookup"><span data-stu-id="4afc4-135">Request</span></span>
<span data-ttu-id="4afc4-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4afc4-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4afc4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4afc4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
# <a name="c"></a>[<span data-ttu-id="4afc4-138">C#</span><span class="sxs-lookup"><span data-stu-id="4afc4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-section-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4afc4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4afc4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-section-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4afc4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4afc4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-section-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4afc4-141">响应</span><span class="sxs-lookup"><span data-stu-id="4afc4-141">Response</span></span>
<span data-ttu-id="4afc4-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4afc4-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


