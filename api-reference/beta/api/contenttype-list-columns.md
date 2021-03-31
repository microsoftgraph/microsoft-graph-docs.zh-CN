---
author: swapnil1993
title: 列出内容类型中的 columnDefinitions
description: 列出内容类型中的列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 49a47efbeb59869dfc4f1b83946f9b6a8f178924
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468903"
---
# <a name="list-columns-in-a-content-type"></a><span data-ttu-id="77f04-103">列出内容类型中的列</span><span class="sxs-lookup"><span data-stu-id="77f04-103">List columns in a content type</span></span>
<span data-ttu-id="77f04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="77f04-105">获取在内容类型中表示为 [columnDefinition][columnDefinition] 资源的 [列的集合][contentType]。</span><span class="sxs-lookup"><span data-stu-id="77f04-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [content type][contentType].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="77f04-106">权限</span><span class="sxs-lookup"><span data-stu-id="77f04-106">Permissions</span></span>

  

<span data-ttu-id="77f04-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="77f04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="77f04-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="77f04-109">Permission type</span></span> | <span data-ttu-id="77f04-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77f04-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77f04-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77f04-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77f04-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="77f04-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="77f04-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77f04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77f04-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="77f04-114">Not supported.</span></span> |
|<span data-ttu-id="77f04-115">Application</span><span class="sxs-lookup"><span data-stu-id="77f04-115">Application</span></span> | <span data-ttu-id="77f04-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="77f04-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="77f04-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77f04-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}/columns
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="77f04-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77f04-118">Optional query parameters</span></span>
<span data-ttu-id="77f04-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="77f04-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="77f04-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="77f04-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="77f04-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="77f04-121">Request headers</span></span>
|<span data-ttu-id="77f04-122">名称</span><span class="sxs-lookup"><span data-stu-id="77f04-122">Name</span></span>|<span data-ttu-id="77f04-123">说明</span><span class="sxs-lookup"><span data-stu-id="77f04-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="77f04-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77f04-124">Authorization</span></span>|<span data-ttu-id="77f04-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77f04-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77f04-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77f04-127">Request body</span></span>
<span data-ttu-id="77f04-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77f04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77f04-129">响应</span><span class="sxs-lookup"><span data-stu-id="77f04-129">Response</span></span>

<span data-ttu-id="77f04-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [columnDefinition][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77f04-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="77f04-131">示例</span><span class="sxs-lookup"><span data-stu-id="77f04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77f04-132">请求</span><span class="sxs-lookup"><span data-stu-id="77f04-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="77f04-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="77f04-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_contenttype" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
```
# <a name="c"></a>[<span data-ttu-id="77f04-134">C#</span><span class="sxs-lookup"><span data-stu-id="77f04-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77f04-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77f04-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77f04-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77f04-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77f04-137">Java</span><span class="sxs-lookup"><span data-stu-id="77f04-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77f04-138">响应</span><span class="sxs-lookup"><span data-stu-id="77f04-138">Response</span></span>
><span data-ttu-id="77f04-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77f04-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
[contentType]: ../resources/contentType.md
 
