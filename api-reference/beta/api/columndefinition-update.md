---
author: swapnil1993
title: 更新 columnDefinition
description: 更新网站、列表或内容类型列
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 90f9330fd5cb934ec5cead04cfcc245d46b172df
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952230"
---
# <a name="update-columndefinition"></a><span data-ttu-id="f653f-103">更新 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f653f-103">Update columnDefinition</span></span>
<span data-ttu-id="f653f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f653f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="f653f-105">更新[网站、][][列表或][][内容类型][contentType] [column][columnDefinition] 。</span><span class="sxs-lookup"><span data-stu-id="f653f-105">Update a [site][], [list][] or [content type][contentType] [column][columnDefinition].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="f653f-106">权限</span><span class="sxs-lookup"><span data-stu-id="f653f-106">Permissions</span></span>  

<span data-ttu-id="f653f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f653f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="f653f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f653f-109">Permission type</span></span> | <span data-ttu-id="f653f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f653f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f653f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f653f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f653f-112">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f653f-112">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="f653f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f653f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f653f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f653f-114">Not supported.</span></span> |
|<span data-ttu-id="f653f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f653f-115">Application</span></span> | <span data-ttu-id="f653f-116">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f653f-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="f653f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f653f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/columns/{column-id}
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a><span data-ttu-id="f653f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f653f-118">Request headers</span></span>
|<span data-ttu-id="f653f-119">名称</span><span class="sxs-lookup"><span data-stu-id="f653f-119">Name</span></span>|<span data-ttu-id="f653f-120">说明</span><span class="sxs-lookup"><span data-stu-id="f653f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f653f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f653f-121">Authorization</span></span>|<span data-ttu-id="f653f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f653f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f653f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f653f-124">Content-Type</span></span>|<span data-ttu-id="f653f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f653f-p103">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="f653f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f653f-127">Request body</span></span>

<span data-ttu-id="f653f-128">在请求正文中，提供要更新的 [columnDefinition][] 资源的这些属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f653f-128">In the request body, supply a JSON representation of those properties of a [columnDefinition][] resource to update.</span></span> <span data-ttu-id="f653f-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f653f-129">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="f653f-130">对于 site **或** list 中的 **列**，可以更新 **columnDefinition** 的任何属性，而不是 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="f653f-130">For columns in **site** or **list**, you can update any property of **columnDefinition** other than the **id** property.</span></span>

<span data-ttu-id="f653f-131">对于 **contentType 中的列**，只能更新 **必需属性或\*\*\*\*隐藏** 属性。</span><span class="sxs-lookup"><span data-stu-id="f653f-131">For columns in **contentType**, you can update only the **required** or **hidden** property.</span></span>

## <a name="response"></a><span data-ttu-id="f653f-132">响应</span><span class="sxs-lookup"><span data-stu-id="f653f-132">Response</span></span>

<span data-ttu-id="f653f-133">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [columnDefinition][] 对象。</span><span class="sxs-lookup"><span data-stu-id="f653f-133">If successful, this method returns a `200 OK` response code and an updated [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f653f-134">示例</span><span class="sxs-lookup"><span data-stu-id="f653f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f653f-135">请求</span><span class="sxs-lookup"><span data-stu-id="f653f-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f653f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f653f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype_column"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
Content-Type: application/json

{
  "required": true,
  "hidden": false,
  "propagateChanges": false     
}
```
# <a name="c"></a>[<span data-ttu-id="f653f-137">C#</span><span class="sxs-lookup"><span data-stu-id="f653f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contenttype-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f653f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f653f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f653f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f653f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f653f-140">Java</span><span class="sxs-lookup"><span data-stu-id="f653f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contenttype-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f653f-141">响应</span><span class="sxs-lookup"><span data-stu-id="f653f-141">Response</span></span>
><span data-ttu-id="f653f-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f653f-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Custom Column",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Custom Column",
  "readOnly": false,
  "required": true,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}

```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
[list]: ../resources/list.md
[site]: ../resources/site.md

