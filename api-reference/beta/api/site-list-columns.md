---
author: swapnil1993
title: 列出网站中的列
description: 列出网站中的列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 30cb4348c1203d188a62f72d0545cd9d95de4112
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200772"
---
# <a name="list-columns-in-a-site"></a><span data-ttu-id="6669e-103">列出网站中的列</span><span class="sxs-lookup"><span data-stu-id="6669e-103">List columns in a site</span></span>
<span data-ttu-id="6669e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6669e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6669e-105">获取网站 中的列的集合，这些列表示为 [columnDefinition][columnDefinition] [资源][site]。</span><span class="sxs-lookup"><span data-stu-id="6669e-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [site][site].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="6669e-106">权限</span><span class="sxs-lookup"><span data-stu-id="6669e-106">Permissions</span></span>

  

<span data-ttu-id="6669e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6669e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="6669e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6669e-109">Permission type</span></span> | <span data-ttu-id="6669e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6669e-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6669e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6669e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6669e-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6669e-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="6669e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6669e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6669e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6669e-114">Not supported.</span></span> |
|<span data-ttu-id="6669e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6669e-115">Application</span></span> | <span data-ttu-id="6669e-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6669e-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="6669e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6669e-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http

GET /sites/{site-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="6669e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6669e-118">Optional query parameters</span></span>
<span data-ttu-id="6669e-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6669e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6669e-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6669e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6669e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6669e-121">Request headers</span></span>
|<span data-ttu-id="6669e-122">名称</span><span class="sxs-lookup"><span data-stu-id="6669e-122">Name</span></span>|<span data-ttu-id="6669e-123">说明</span><span class="sxs-lookup"><span data-stu-id="6669e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6669e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6669e-124">Authorization</span></span>|<span data-ttu-id="6669e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6669e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6669e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6669e-127">Request body</span></span>
<span data-ttu-id="6669e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6669e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6669e-129">响应</span><span class="sxs-lookup"><span data-stu-id="6669e-129">Response</span></span>

<span data-ttu-id="6669e-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [columnDefinition][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6669e-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="6669e-131">示例</span><span class="sxs-lookup"><span data-stu-id="6669e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6669e-132">请求</span><span class="sxs-lookup"><span data-stu-id="6669e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6669e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6669e-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_site" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/columns
```
# <a name="c"></a>[<span data-ttu-id="6669e-134">C#</span><span class="sxs-lookup"><span data-stu-id="6669e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6669e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6669e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6669e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6669e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6669e-137">Java</span><span class="sxs-lookup"><span data-stu-id="6669e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6669e-138">响应</span><span class="sxs-lookup"><span data-stu-id="6669e-138">Response</span></span>
><span data-ttu-id="6669e-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6669e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
[site]: ../resources/site.md
 
