---
author: swapnil1993
title: 更新 columnDefinition
description: 更新内容类型列
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 89c26b5fcbe3f6509d2d763ed6e8e4d06a8530d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773345"
---
# <a name="update-columndefinition"></a><span data-ttu-id="d3ac0-103">更新 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="d3ac0-103">Update columnDefinition</span></span>
<span data-ttu-id="d3ac0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3ac0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="d3ac0-105">更新 [内容类型][contentType] [column][columnDefinition] 。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-105">Update a [content type][contentType] [column][columnDefinition].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="d3ac0-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3ac0-106">Permissions</span></span>  

<span data-ttu-id="d3ac0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="d3ac0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3ac0-109">Permission type</span></span> | <span data-ttu-id="d3ac0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3ac0-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3ac0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3ac0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3ac0-112">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d3ac0-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="d3ac0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3ac0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3ac0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-114">Not supported.</span></span> |
|<span data-ttu-id="d3ac0-115">Application</span><span class="sxs-lookup"><span data-stu-id="d3ac0-115">Application</span></span> | <span data-ttu-id="d3ac0-116">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d3ac0-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="d3ac0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3ac0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a><span data-ttu-id="d3ac0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3ac0-118">Request headers</span></span>
|<span data-ttu-id="d3ac0-119">名称</span><span class="sxs-lookup"><span data-stu-id="d3ac0-119">Name</span></span>|<span data-ttu-id="d3ac0-120">说明</span><span class="sxs-lookup"><span data-stu-id="d3ac0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3ac0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3ac0-121">Authorization</span></span>|<span data-ttu-id="d3ac0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3ac0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3ac0-124">Content-Type</span></span>|<span data-ttu-id="d3ac0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d3ac0-p103">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="d3ac0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3ac0-127">Request body</span></span>

<span data-ttu-id="d3ac0-128">在请求正文中，提供要更新的 [columnDefinition 资源的][] JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-128">In the request body, supply a JSON representation of the [columnDefinition][] resource to update.</span></span>  

><span data-ttu-id="d3ac0-129">**注意：** 只能更新必需属性和隐藏属性。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-129">**Note:** Only required and hidden properties can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="d3ac0-130">响应</span><span class="sxs-lookup"><span data-stu-id="d3ac0-130">Response</span></span>

<span data-ttu-id="d3ac0-131">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [columnDefinition][] 对象。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-131">If successful, this method returns a `200 OK` response code and an updated [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3ac0-132">示例</span><span class="sxs-lookup"><span data-stu-id="d3ac0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3ac0-133">请求</span><span class="sxs-lookup"><span data-stu-id="d3ac0-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d3ac0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3ac0-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d3ac0-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3ac0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contenttype-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3ac0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3ac0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3ac0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3ac0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3ac0-138">Java</span><span class="sxs-lookup"><span data-stu-id="d3ac0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contenttype-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3ac0-139">响应</span><span class="sxs-lookup"><span data-stu-id="d3ac0-139">Response</span></span>
><span data-ttu-id="d3ac0-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d3ac0-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
