---
title: 使用的列表
description: '计算并列出用户已查看或修改的文档。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: ba9b5953f877a6dae825aea6bede63af18c55ffd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039543"
---
# <a name="list-used"></a><span data-ttu-id="1ff7c-103">使用的列表</span><span class="sxs-lookup"><span data-stu-id="1ff7c-103">List used</span></span>

<span data-ttu-id="1ff7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ff7c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1ff7c-105">计算并列出用户已查看或修改的文档。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-105">Calculate and list the documents that a user has viewed or modified.</span></span> 

<span data-ttu-id="1ff7c-106">对于登录用户：</span><span class="sxs-lookup"><span data-stu-id="1ff7c-106">For the signed-in user:</span></span>
- <span data-ttu-id="1ff7c-107">此方法包括用户已修改的文档;请参阅[示例 1。](#example-1-return-documents-that-user-has-modified)</span><span class="sxs-lookup"><span data-stu-id="1ff7c-107">This method includes documents that the user has modified; see [example 1](#example-1-return-documents-that-user-has-modified).</span></span> 
- <span data-ttu-id="1ff7c-108">对 `$orderby` **lastAccessedDateTime** 属性使用查询参数可返回用户可能修改或可能尚未修改的最近查看的文档;请参阅示例 [2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified)。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-108">Using an `$orderby` query parameter on the **lastAccessedDateTime** property returns the most recently viewed documents that the user might or might not not have modified; see [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>

<span data-ttu-id="1ff7c-109">对于其他用户，此方法仅包括用户已修改的文档。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-109">For other users, this method includes only documents that the user has modified.</span></span>


## <a name="permissions"></a><span data-ttu-id="1ff7c-110">权限</span><span class="sxs-lookup"><span data-stu-id="1ff7c-110">Permissions</span></span>
<span data-ttu-id="1ff7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff7c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ff7c-113">Permission type</span></span>      | <span data-ttu-id="1ff7c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ff7c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ff7c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ff7c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1ff7c-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff7c-116">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ff7c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ff7c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ff7c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-118">Not supported.</span></span>    |
|<span data-ttu-id="1ff7c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ff7c-119">Application</span></span> | <span data-ttu-id="1ff7c-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff7c-120">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ff7c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ff7c-121">HTTP request</span></span>

- <span data-ttu-id="1ff7c-122">获取登录用户已修改的文档列表：</span><span class="sxs-lookup"><span data-stu-id="1ff7c-122">Get a list of documents that the signed-in user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used
  ```

- <span data-ttu-id="1ff7c-123">获取指定用户已修改的文档列表：</span><span class="sxs-lookup"><span data-stu-id="1ff7c-123">Get a list of documents that the specified user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  ><span data-ttu-id="1ff7c-124">**注意**：请求其他用户使用 **的文档** 将返回按 **lastModifiedDateTime 排序的结果**。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-124">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="1ff7c-125">**lastAccessedDateTime** 随后设置为 **lastModifiedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-125">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>


- <span data-ttu-id="1ff7c-126">展开已用见解引用 **的资源** ：</span><span class="sxs-lookup"><span data-stu-id="1ff7c-126">Expand the resource referenced by a **used** insight:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a><span data-ttu-id="1ff7c-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ff7c-127">Optional query parameters</span></span>
<span data-ttu-id="1ff7c-128">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="1ff7c-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- <span data-ttu-id="1ff7c-129">使用 `$filter` 查询参数筛选已用项目。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-129">Use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="1ff7c-130">例如，根据 **类型**：</span><span class="sxs-lookup"><span data-stu-id="1ff7c-130">For example, based on **type**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- <span data-ttu-id="1ff7c-131">用于 `$filter` 根据  **containerType** 筛选已用项：</span><span class="sxs-lookup"><span data-stu-id="1ff7c-131">Use `$filter` to filter used items based on  **containerType**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  <span data-ttu-id="1ff7c-132">请参阅 [resourceVisualization](../resources/insights-resourcevisualization.md)中可以按筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-132">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

- <span data-ttu-id="1ff7c-133">使用 `$orderBy` 查询参数根据 **lastAccessedDateTime** 属性对登录用户最后查看或修改的文档进行排序： </span><span class="sxs-lookup"><span data-stu-id="1ff7c-133">Use the `$orderBy` query parameter to sort documents last viewed or modified _by the signed-in user_, based on the **lastAccessedDateTime** property:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  ><span data-ttu-id="1ff7c-134">**注意**：仅对登录 _用户使用此查询选项_。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-134">**Note**: Use this query option _only for the signed-in user_.</span></span> <span data-ttu-id="1ff7c-135">不能使用此 API 获取其他用户查看或修改的文档。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-135">You cannot use this API to get documents viewed or modified by another user.</span></span> <span data-ttu-id="1ff7c-136">请参阅[示例 2。](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified)</span><span class="sxs-lookup"><span data-stu-id="1ff7c-136">See [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>


## <a name="request-headers"></a><span data-ttu-id="1ff7c-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ff7c-137">Request headers</span></span>
| <span data-ttu-id="1ff7c-138">标头</span><span class="sxs-lookup"><span data-stu-id="1ff7c-138">Header</span></span>       |  <span data-ttu-id="1ff7c-139">值</span><span class="sxs-lookup"><span data-stu-id="1ff7c-139">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="1ff7c-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ff7c-140">Authorization</span></span>  | <span data-ttu-id="1ff7c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1ff7c-143">接受</span><span class="sxs-lookup"><span data-stu-id="1ff7c-143">Accept</span></span>  | <span data-ttu-id="1ff7c-144">application/json</span><span class="sxs-lookup"><span data-stu-id="1ff7c-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ff7c-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ff7c-145">Request body</span></span>
<span data-ttu-id="1ff7c-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff7c-147">响应</span><span class="sxs-lookup"><span data-stu-id="1ff7c-147">Response</span></span>

<span data-ttu-id="1ff7c-148">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/insights-used.md)已用项列表。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-148">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ff7c-149">示例</span><span class="sxs-lookup"><span data-stu-id="1ff7c-149">Example</span></span>

### <a name="example-1-return-documents-that-user-has-modified"></a><span data-ttu-id="1ff7c-150">示例 1：返回用户已修改的文档</span><span class="sxs-lookup"><span data-stu-id="1ff7c-150">Example 1: Return documents that user has modified</span></span>

#### <a name="request"></a><span data-ttu-id="1ff7c-151">请求</span><span class="sxs-lookup"><span data-stu-id="1ff7c-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff7c-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff7c-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used
```
# <a name="c"></a>[<span data-ttu-id="1ff7c-153">C#</span><span class="sxs-lookup"><span data-stu-id="1ff7c-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff7c-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff7c-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff7c-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff7c-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ff7c-156">Java</span><span class="sxs-lookup"><span data-stu-id="1ff7c-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifieddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1ff7c-157">响应</span><span class="sxs-lookup"><span data-stu-id="1ff7c-157">Response</span></span>

><span data-ttu-id="1ff7c-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1ff7c-158">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3/thumbnails/0/small/thumbnailContent",
                "previewText": "Page-1",
                "containerWebUrl": "https://contoso.sharepoint.com/sites/Retail/Shared Documents/NC460 Sales",
                "containerDisplayName": "Retail",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Retail/_layouts/15/Doc.aspx?sourcedoc=%7BF4463999-4FB5-4F8B-9994-968C56353C5B%7D&file=Org%20Chart.vsdx&action=default&DefaultItemOpen=1",
                "id": "drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a><span data-ttu-id="1ff7c-159">示例 2：返回登录用户可能修改或可能未修改的最近查看的文档</span><span class="sxs-lookup"><span data-stu-id="1ff7c-159">Example 2: Return the most recently viewed documents that the signed-in user might or might not have modified</span></span> 

#### <a name="request"></a><span data-ttu-id="1ff7c-160">请求</span><span class="sxs-lookup"><span data-stu-id="1ff7c-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff7c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff7c-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->
  
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[<span data-ttu-id="1ff7c-162">C#</span><span class="sxs-lookup"><span data-stu-id="1ff7c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff7c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff7c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff7c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff7c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ff7c-165">Java</span><span class="sxs-lookup"><span data-stu-id="1ff7c-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifiedandvieweddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1ff7c-166">响应</span><span class="sxs-lookup"><span data-stu-id="1ff7c-166">Response</span></span>
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
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!ZOatQFjNPEyy-0guRSS0ho36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01NTE4NPQAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Executive Corner",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Exec",
                "id": "sites/contoso.sharepoint.com,40ade664-cd58-4c3c-b2fb-482e4524b486,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        }
    ]
}
```

