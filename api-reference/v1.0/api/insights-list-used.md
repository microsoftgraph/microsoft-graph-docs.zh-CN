---
title: 使用的列表
description: '计算并列出用户已查看或修改的文档。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0c8d00f03d98c5dc5d18411f238ca9a507eaca30
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973195"
---
# <a name="list-used"></a><span data-ttu-id="8b530-103">使用的列表</span><span class="sxs-lookup"><span data-stu-id="8b530-103">List used</span></span>

<span data-ttu-id="8b530-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b530-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b530-105">计算并列出用户已查看或修改的文档。</span><span class="sxs-lookup"><span data-stu-id="8b530-105">Calculate and list the documents that a user has viewed or modified.</span></span> 

<span data-ttu-id="8b530-106">对于登录用户：</span><span class="sxs-lookup"><span data-stu-id="8b530-106">For the signed-in user:</span></span>
- <span data-ttu-id="8b530-107">此方法包括用户已修改的文档;请参阅 [示例 1](#example-1-return-documents-that-user-has-modified)。</span><span class="sxs-lookup"><span data-stu-id="8b530-107">This method includes documents that the user has modified; see [example 1](#example-1-return-documents-that-user-has-modified).</span></span> 
- <span data-ttu-id="8b530-108">使用 `$orderby` **lastAccessedDateTime** 属性上的查询参数返回用户可能已修改或可能尚未修改的最近查看过的文档; 请参阅 [示例 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified)。</span><span class="sxs-lookup"><span data-stu-id="8b530-108">Using an `$orderby` query parameter on the **lastAccessedDateTime** property returns the most recently viewed documents that the user might or might not not have modified; see [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>

<span data-ttu-id="8b530-109">对于其他用户，此方法仅包括用户已修改的文档。</span><span class="sxs-lookup"><span data-stu-id="8b530-109">For other users, this method includes only documents that the user has modified.</span></span>


## <a name="permissions"></a><span data-ttu-id="8b530-110">权限</span><span class="sxs-lookup"><span data-stu-id="8b530-110">Permissions</span></span>
<span data-ttu-id="8b530-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b530-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b530-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b530-113">Permission type</span></span>      | <span data-ttu-id="8b530-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b530-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b530-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b530-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8b530-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b530-116">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b530-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b530-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b530-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b530-118">Not supported.</span></span>    |
|<span data-ttu-id="8b530-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b530-119">Application</span></span> | <span data-ttu-id="8b530-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b530-120">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b530-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b530-121">HTTP request</span></span>

- <span data-ttu-id="8b530-122">获取已登录用户已修改的文档列表：</span><span class="sxs-lookup"><span data-stu-id="8b530-122">Get a list of documents that the signed-in user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used
  ```

- <span data-ttu-id="8b530-123">获取指定用户修改的文档的列表：</span><span class="sxs-lookup"><span data-stu-id="8b530-123">Get a list of documents that the specified user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  ><span data-ttu-id="8b530-124">**注意**：请求其他用户的已 **使用** 文档返回按 **lastModifiedDateTime**排序的结果。</span><span class="sxs-lookup"><span data-stu-id="8b530-124">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="8b530-125">然后，将**lastAccessedDateTime**设置为**lastModifiedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="8b530-125">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>


- <span data-ttu-id="8b530-126">扩展 **使用** 的洞察力引用的资源：</span><span class="sxs-lookup"><span data-stu-id="8b530-126">Expand the resource referenced by a **used** insight:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a><span data-ttu-id="8b530-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8b530-127">Optional query parameters</span></span>
<span data-ttu-id="8b530-128">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="8b530-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- <span data-ttu-id="8b530-129">使用 `$filter` 查询参数筛选已使用的项目。</span><span class="sxs-lookup"><span data-stu-id="8b530-129">Use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="8b530-130">例如，基于 **类型**：</span><span class="sxs-lookup"><span data-stu-id="8b530-130">For example, based on **type**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- <span data-ttu-id="8b530-131">使用 `$filter` 基于  **containerType**筛选已使用的项目：</span><span class="sxs-lookup"><span data-stu-id="8b530-131">Use `$filter` to filter used items based on  **containerType**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  <span data-ttu-id="8b530-132">请参阅可在 [resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="8b530-132">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

- <span data-ttu-id="8b530-133">使用 `$orderBy` 查询参数对 _已登录用户_上次查看或修改的文档进行排序，基于 **lastAccessedDateTime** 属性：</span><span class="sxs-lookup"><span data-stu-id="8b530-133">Use the `$orderBy` query parameter to sort documents last viewed or modified _by the signed-in user_, based on the **lastAccessedDateTime** property:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  ><span data-ttu-id="8b530-134">**注意**： _仅对已登录用户_使用此查询选项。</span><span class="sxs-lookup"><span data-stu-id="8b530-134">**Note**: Use this query option _only for the signed-in user_.</span></span> <span data-ttu-id="8b530-135">您不能使用此 API 获取其他用户查看或修改的文档。</span><span class="sxs-lookup"><span data-stu-id="8b530-135">You cannot use this API to get documents viewed or modified by another user.</span></span> <span data-ttu-id="8b530-136">请参阅 [示例 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified)。</span><span class="sxs-lookup"><span data-stu-id="8b530-136">See [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>


## <a name="request-headers"></a><span data-ttu-id="8b530-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b530-137">Request headers</span></span>
| <span data-ttu-id="8b530-138">标头</span><span class="sxs-lookup"><span data-stu-id="8b530-138">Header</span></span>       |  <span data-ttu-id="8b530-139">值</span><span class="sxs-lookup"><span data-stu-id="8b530-139">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="8b530-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b530-140">Authorization</span></span>  | <span data-ttu-id="8b530-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b530-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8b530-143">接受</span><span class="sxs-lookup"><span data-stu-id="8b530-143">Accept</span></span>  | <span data-ttu-id="8b530-144">application/json</span><span class="sxs-lookup"><span data-stu-id="8b530-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b530-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b530-145">Request body</span></span>
<span data-ttu-id="8b530-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b530-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b530-147">响应</span><span class="sxs-lookup"><span data-stu-id="8b530-147">Response</span></span>

<span data-ttu-id="8b530-148">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和已 [使用](../resources/insights-used.md) 项的列表。</span><span class="sxs-lookup"><span data-stu-id="8b530-148">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b530-149">示例</span><span class="sxs-lookup"><span data-stu-id="8b530-149">Example</span></span>

### <a name="example-1-return-documents-that-user-has-modified"></a><span data-ttu-id="8b530-150">示例1：返回用户已修改的文档</span><span class="sxs-lookup"><span data-stu-id="8b530-150">Example 1: Return documents that user has modified</span></span>

#### <a name="request"></a><span data-ttu-id="8b530-151">请求</span><span class="sxs-lookup"><span data-stu-id="8b530-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b530-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b530-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used
```
# <a name="c"></a>[<span data-ttu-id="8b530-153">C#</span><span class="sxs-lookup"><span data-stu-id="8b530-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b530-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b530-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b530-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b530-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b530-156">Java</span><span class="sxs-lookup"><span data-stu-id="8b530-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifieddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b530-157">响应</span><span class="sxs-lookup"><span data-stu-id="8b530-157">Response</span></span>

><span data-ttu-id="8b530-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8b530-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "Abk3ZeZmlghMhUVKP9mygDoPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5k5RvS1T4tPmZSWjFY1PFu5N2XmZpYITIVFSj_ZsoA6BQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:38Z",
                "lastModifiedDateTime": "2019-05-25T07:12:37Z"
            },
            "resourceVisualization": {
                "title": "Org Chart",
                "type": "Visio",
                "mediaType": "application/vnd.visio",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3/thumbnails/0/small/thumbnailContent",
                "previewText": "Page-1",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/Retail/Shared Documents/NC460 Sales",
                "containerDisplayName": "Retail",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Retail/_layouts/15/Doc.aspx?sourcedoc=%7BF4463999-4FB5-4F8B-9994-968C56353C5B%7D&file=Org%20Chart.vsdx&action=default&DefaultItemOpen=1",
                "id": "drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5T7emOJwqlCit_j9Q5CpWSlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:26Z",
                "lastModifiedDateTime": "2019-05-25T07:12:26Z"
            },
            "resourceVisualization": {
                "title": "USA Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Audio Car Audio Audio - Car Audio 4910000 4664500 245500 3928000 4320800 -736500 Audi",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B637AFB94-C289-42A9-8ADF-E3F50E42A564%7D&file=USA%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INAy6LlBcXfAJCmOiEWgBJjh-lSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:11:49Z",
                "lastModifiedDateTime": "2019-05-25T07:11:48Z"
            },
            "resourceVisualization": {
                "title": "UK Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Electronics Wearable Technology Electronics - Wearable Technology 2226000 2114700 111",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B17948B2E-7C17-4202-98E8-845A00498E1F%7D&file=UK%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a><span data-ttu-id="8b530-160">示例2：返回已登录用户可能已修改或可能尚未修改的最近查看过的文档</span><span class="sxs-lookup"><span data-stu-id="8b530-160">Example 2: Return the most recently viewed documents that the signed-in user might or might not have modified</span></span> 

#### <a name="request"></a><span data-ttu-id="8b530-161">请求</span><span class="sxs-lookup"><span data-stu-id="8b530-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b530-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b530-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->
  
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[<span data-ttu-id="8b530-163">C#</span><span class="sxs-lookup"><span data-stu-id="8b530-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b530-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b530-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b530-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b530-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b530-166">Java</span><span class="sxs-lookup"><span data-stu-id="8b530-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifiedandvieweddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b530-167">响应</span><span class="sxs-lookup"><span data-stu-id="8b530-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "AWTmrUBYzTxMsvtILkUktIaN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABk5q1AWM08TLL7SC5FJLSGBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Executive Corner",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!ZOatQFjNPEyy-0guRSS0ho36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01NTE4NPQAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Executive Corner",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Exec",
                "id": "sites/m365x887078.sharepoint.com,40ade664-cd58-4c3c-b2fb-482e4524b486,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AahdFRA14_FMrGLq9V4WmyiN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACoXRUQNePxTKxi6vVeFpsoBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Contoso Landings",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!qF0VEDXj8UysYur1XhabKI36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01UHO6LBAAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Contoso Landings",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/ContosoLandings",
                "id": "sites/m365x887078.sharepoint.com,10155da8-e335-4cf1-ac62-eaf55e169b28,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IztQAKAS6acR7HFoIKDqOPE6bjkeoHWtEu7LoUIsZkHSkzLaA_67htEozMGRwifyaqlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:54Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Media Preview Packages",
                "type": "Web",
                "mediaType": "text/html",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jO1AAoBLppxHscWggoOo48TpuOR6gda0S7suhQixmQdK/items/01RGQ6XKCMZNUA76XODNCKGMYGI4EJ7SNK/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Forms/ByAuthor.aspx",
                "containerDisplayName": "Campaigns - Events"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Media-Preview-Packages.aspx"
            }
        }
    ]
}
```

