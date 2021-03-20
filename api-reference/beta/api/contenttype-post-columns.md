---
author: swapnil1993
ms.date: 08/30/2020
title: 在内容类型创建 columnDefinition
description: 向内容类型添加列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 7071322064d55c21123fabd5ddc80d63fa5575ac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946962"
---
# <a name="create-columndefinition-for-a-content-type"></a><span data-ttu-id="db679-103">为内容类型创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="db679-103">Create columnDefinition for a content type</span></span>
<span data-ttu-id="db679-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db679-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="db679-105">向内容类型添加 [列][contentType] in a site or list by specifying a [columnDefinition][columnDefinition] 。</span><span class="sxs-lookup"><span data-stu-id="db679-105">Add a column to a [content type][contentType] in a site or list by specifying a [columnDefinition][columnDefinition].</span></span>

## <a name="permissions"></a><span data-ttu-id="db679-106">权限</span><span class="sxs-lookup"><span data-stu-id="db679-106">Permissions</span></span>

<span data-ttu-id="db679-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="db679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="db679-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db679-109">Permission type</span></span> | <span data-ttu-id="db679-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db679-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db679-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db679-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db679-112">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="db679-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="db679-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db679-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db679-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db679-114">Not supported.</span></span> |
|<span data-ttu-id="db679-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db679-115">Application</span></span> | <span data-ttu-id="db679-116">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="db679-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="db679-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db679-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="db679-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="db679-118">Request body</span></span>

<span data-ttu-id="db679-119">在请求正文中，提供要添加的 [columnDefinition 资源的][] JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db679-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="db679-120">响应</span><span class="sxs-lookup"><span data-stu-id="db679-120">Response</span></span>

<span data-ttu-id="db679-121">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [columnDefinition][] 对象。</span><span class="sxs-lookup"><span data-stu-id="db679-121">If successful, this method returns a `200 OK` response code and [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db679-122">示例</span><span class="sxs-lookup"><span data-stu-id="db679-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="db679-123">请求</span><span class="sxs-lookup"><span data-stu-id="db679-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
```

### <a name="response"></a><span data-ttu-id="db679-124">响应</span><span class="sxs-lookup"><span data-stu-id="db679-124">Response</span></span>

<span data-ttu-id="db679-125">响应返回添加到内容类型的列。</span><span class="sxs-lookup"><span data-stu-id="db679-125">The response returns the column added to a content type.</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true} -->

  

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
  

