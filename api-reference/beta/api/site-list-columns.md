---
author: swapnil1993
title: 列出网站中的列
description: 列出网站中的列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: dd7abfad63b268efb9748335ff0ef34d3b485312
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697212"
---
# <a name="list-columns-in-a-site"></a><span data-ttu-id="50a69-103">列出网站中的列</span><span class="sxs-lookup"><span data-stu-id="50a69-103">List columns in a site</span></span>
<span data-ttu-id="50a69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50a69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="50a69-105">获取网站 中的列的集合，这些列表示为 [columnDefinition][columnDefinition] [资源][site]。</span><span class="sxs-lookup"><span data-stu-id="50a69-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [site][site].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="50a69-106">权限</span><span class="sxs-lookup"><span data-stu-id="50a69-106">Permissions</span></span>

  

<span data-ttu-id="50a69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="50a69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="50a69-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="50a69-109">Permission type</span></span> | <span data-ttu-id="50a69-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50a69-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50a69-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50a69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50a69-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="50a69-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="50a69-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50a69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a69-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="50a69-114">Not supported.</span></span> |
|<span data-ttu-id="50a69-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="50a69-115">Application</span></span> | <span data-ttu-id="50a69-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="50a69-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="50a69-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50a69-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="50a69-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50a69-118">Optional query parameters</span></span>
<span data-ttu-id="50a69-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="50a69-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="50a69-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="50a69-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="50a69-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="50a69-121">Request headers</span></span>
|<span data-ttu-id="50a69-122">名称</span><span class="sxs-lookup"><span data-stu-id="50a69-122">Name</span></span>|<span data-ttu-id="50a69-123">说明</span><span class="sxs-lookup"><span data-stu-id="50a69-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="50a69-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="50a69-124">Authorization</span></span>|<span data-ttu-id="50a69-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50a69-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50a69-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50a69-127">Request body</span></span>
<span data-ttu-id="50a69-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50a69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50a69-129">响应</span><span class="sxs-lookup"><span data-stu-id="50a69-129">Response</span></span>

<span data-ttu-id="50a69-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [columnDefinition][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="50a69-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="50a69-131">示例</span><span class="sxs-lookup"><span data-stu-id="50a69-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="50a69-132">请求</span><span class="sxs-lookup"><span data-stu-id="50a69-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="50a69-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="50a69-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_site" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/columns
```
# <a name="c"></a>[<span data-ttu-id="50a69-134">C#</span><span class="sxs-lookup"><span data-stu-id="50a69-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50a69-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50a69-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50a69-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50a69-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50a69-137">Java</span><span class="sxs-lookup"><span data-stu-id="50a69-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50a69-138">响应</span><span class="sxs-lookup"><span data-stu-id="50a69-138">Response</span></span>
><span data-ttu-id="50a69-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="50a69-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "value":[
      {
         "description":"",
         "displayName":"Title",
         "hidden":false,
         "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Title",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      },
      {
         "description":"",
         "displayName":"Address",
         "id":"11dfef35-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Address",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      }
   ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
 
