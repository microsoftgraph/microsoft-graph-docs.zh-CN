---
author: swapnil1993
title: 列出 columnDefinitions
description: 列出内容类型的列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5d3c1c4e64323aa772639d977d0d4dfc18603932
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446121"
---
# <a name="list-columndefinitions"></a><span data-ttu-id="42e25-103">列出 columnDefinitions</span><span class="sxs-lookup"><span data-stu-id="42e25-103">List columnDefinitions</span></span>
<span data-ttu-id="42e25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42e25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="42e25-105">获取内容  [类型中的][columnDefinition] [集合][contentType]。</span><span class="sxs-lookup"><span data-stu-id="42e25-105">Get the collection of  [columns][columnDefinition] in a [content type][contentType].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="42e25-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="42e25-106">Permissions</span></span>

  

<span data-ttu-id="42e25-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="42e25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="42e25-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="42e25-109">Permission type</span></span> | <span data-ttu-id="42e25-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42e25-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42e25-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42e25-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42e25-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="42e25-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="42e25-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42e25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42e25-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="42e25-114">Not supported.</span></span> |
|<span data-ttu-id="42e25-115">Application</span><span class="sxs-lookup"><span data-stu-id="42e25-115">Application</span></span> | <span data-ttu-id="42e25-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="42e25-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="42e25-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42e25-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http

GET /sites/{site-id}/contentTypes/{contentType-id}/columns
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="42e25-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="42e25-118">Optional query parameters</span></span>
<span data-ttu-id="42e25-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="42e25-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="42e25-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="42e25-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42e25-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="42e25-121">Request headers</span></span>
|<span data-ttu-id="42e25-122">名称</span><span class="sxs-lookup"><span data-stu-id="42e25-122">Name</span></span>|<span data-ttu-id="42e25-123">说明</span><span class="sxs-lookup"><span data-stu-id="42e25-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="42e25-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="42e25-124">Authorization</span></span>|<span data-ttu-id="42e25-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42e25-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42e25-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="42e25-127">Request body</span></span>
<span data-ttu-id="42e25-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42e25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42e25-129">响应</span><span class="sxs-lookup"><span data-stu-id="42e25-129">Response</span></span>

<span data-ttu-id="42e25-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [columnDefinition][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="42e25-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="42e25-131">示例</span><span class="sxs-lookup"><span data-stu-id="42e25-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="42e25-132">请求</span><span class="sxs-lookup"><span data-stu-id="42e25-132">Request</span></span>

<!-- { "blockType": "request", "name": "get_columns_from_contenttype" } -->
 

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
```

### <a name="response"></a><span data-ttu-id="42e25-133">响应</span><span class="sxs-lookup"><span data-stu-id="42e25-133">Response</span></span>
><span data-ttu-id="42e25-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="42e25-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.columnDefinition)"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
    },
    {
      "description": "",
      "displayName": "Address",
      "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
      "indexed": false,
      "name": "Address",
      "readOnly": false,
      "required": false,
      "text": {
        "allowMultipleLines": false,
        "appendChangesToExistingText": false,
        "linesForEditing": 0,
        "maxLength": 255
      }
    }
  ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
 
