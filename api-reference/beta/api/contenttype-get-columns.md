---
author: swapnil1993
title: 获取 columnDefinition
description: " 获取内容类型列。"
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8fa2da27e03ad5d174d1c6bcc19b7b82201fb581
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446126"
---
# <a name="get-columndefinition"></a><span data-ttu-id="b36b0-103">获取 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="b36b0-103">Get columnDefinition</span></span>
<span data-ttu-id="b36b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b36b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="b36b0-105">检索[contentType 列的][][元数据][columnDefinition]。</span><span class="sxs-lookup"><span data-stu-id="b36b0-105">Retrieve the metadata for a [contentType][] [column][columnDefinition].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="b36b0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b36b0-106">Permissions</span></span>

  

<span data-ttu-id="b36b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b36b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="b36b0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b36b0-109">Permission type</span></span> | <span data-ttu-id="b36b0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b36b0-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b36b0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b36b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b36b0-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b36b0-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="b36b0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b36b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b36b0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b36b0-114">Not supported.</span></span> |
|<span data-ttu-id="b36b0-115">Application</span><span class="sxs-lookup"><span data-stu-id="b36b0-115">Application</span></span> | <span data-ttu-id="b36b0-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b36b0-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="b36b0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b36b0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http

GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns/{column-id}
```

## <a name="request-headers"></a><span data-ttu-id="b36b0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b36b0-118">Request headers</span></span>
|<span data-ttu-id="b36b0-119">名称</span><span class="sxs-lookup"><span data-stu-id="b36b0-119">Name</span></span>|<span data-ttu-id="b36b0-120">说明</span><span class="sxs-lookup"><span data-stu-id="b36b0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b36b0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b36b0-121">Authorization</span></span>|<span data-ttu-id="b36b0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b36b0-p102">Bearer {token}. Required.</span></span>|  

## <a name="request-body"></a><span data-ttu-id="b36b0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b36b0-124">Request body</span></span>

  

<span data-ttu-id="b36b0-125">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="b36b0-125">Do not supply a request body with this method.</span></span>

  

## <a name="example"></a><span data-ttu-id="b36b0-126">示例</span><span class="sxs-lookup"><span data-stu-id="b36b0-126">Example</span></span>

  

### <a name="request"></a><span data-ttu-id="b36b0-127">请求</span><span class="sxs-lookup"><span data-stu-id="b36b0-127">Request</span></span>

  

<!-- { "blockType": "request", "name": "get_column_from_contenttype" } -->

  

```http
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```

  

#### <a name="response"></a><span data-ttu-id="b36b0-128">响应</span><span class="sxs-lookup"><span data-stu-id="b36b0-128">Response</span></span>

  

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "readOnly": false,
  "required": false,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md

[list]: ../resources/list.md

[site]: ../resources/site.md

[contentType]: ../resources/contentType.md
  
