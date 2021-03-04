---
author: swapnil1993
ms.date: 08/30/2020
title: 创建 columnDefinition
description: 向内容类型添加列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 071a855c79c055179022157b991b4a9f2789cad1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446117"
---
# <a name="create-columndefinition"></a><span data-ttu-id="4ca42-103">创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="4ca42-103">Create columnDefinition</span></span>
<span data-ttu-id="4ca42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ca42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="4ca42-105">将现有网站或列表 [列][columnDefinition] 添加到 [内容类型][contentType 中]。</span><span class="sxs-lookup"><span data-stu-id="4ca42-105">Adds existing site or list [column][columnDefinition] to a [content type][contentType].</span></span>

## <a name="permissions"></a><span data-ttu-id="4ca42-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ca42-106">Permissions</span></span>

<span data-ttu-id="4ca42-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4ca42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="4ca42-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ca42-109">Permission type</span></span> | <span data-ttu-id="4ca42-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ca42-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ca42-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ca42-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ca42-112">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="4ca42-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="4ca42-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ca42-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ca42-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ca42-114">Not supported.</span></span> |
|<span data-ttu-id="4ca42-115">Application</span><span class="sxs-lookup"><span data-stu-id="4ca42-115">Application</span></span> | <span data-ttu-id="4ca42-116">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="4ca42-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="4ca42-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ca42-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="4ca42-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ca42-118">Request body</span></span>

<span data-ttu-id="4ca42-119">在请求正文中，提供要添加的 [columnDefinition 资源的][] JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ca42-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="4ca42-120">响应</span><span class="sxs-lookup"><span data-stu-id="4ca42-120">Response</span></span>

<span data-ttu-id="4ca42-121">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [contentType][] 对象。</span><span class="sxs-lookup"><span data-stu-id="4ca42-121">If successful, this method returns a `200 OK` response code and [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca42-122">示例</span><span class="sxs-lookup"><span data-stu-id="4ca42-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ca42-123">请求</span><span class="sxs-lookup"><span data-stu-id="4ca42-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
```

### <a name="response"></a><span data-ttu-id="4ca42-124">响应</span><span class="sxs-lookup"><span data-stu-id="4ca42-124">Response</span></span>

<span data-ttu-id="4ca42-125">该响应返回添加到内容类型的所有列的列表。</span><span class="sxs-lookup"><span data-stu-id="4ca42-125">The response returns a list of all columns added to a content type.</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true, "scopes": "sites.readwrite.all" } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
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
  

