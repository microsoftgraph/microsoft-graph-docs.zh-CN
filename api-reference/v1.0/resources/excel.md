---
title: 在 Microsoft Graph 中使用 Excel
description: 你可以使用 Microsoft Graph 来让 Web 和移动应用程序读取和修改存储在 OneDrive for Business、SharePoint 网站或组驱动器中的 Excel 工作簿。
localization_priority: Priority
author: grangery
ms.prod: excel
doc_type: conceptualPageType
ms.openlocfilehash: 2fe503472021c26c2ec856e1b73cb9f432190891
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575999"
---
# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="748e4-103">在 Microsoft Graph 中使用 Excel</span><span class="sxs-lookup"><span data-stu-id="748e4-103">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="748e4-104">你可以使用 Microsoft Graph 来让 Web 和移动应用程序读取和修改存储在 OneDrive for Business、SharePoint 网站或组驱动器中的 Excel 工作簿。</span><span class="sxs-lookup"><span data-stu-id="748e4-104">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive for Business, SharePoint site or Group drive.</span></span> <span data-ttu-id="748e4-105">`Workbook`（或 Excel 文件）资源通过关系包含所有其他 Excel 资源。</span><span class="sxs-lookup"><span data-stu-id="748e4-105">The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships.</span></span> <span data-ttu-id="748e4-106">可以通过识别文件在该 URL 中的位置，借助 [驱动器 API](drive.md) 访问工作簿。</span><span class="sxs-lookup"><span data-stu-id="748e4-106">You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL.</span></span> <span data-ttu-id="748e4-107">例如：</span><span class="sxs-lookup"><span data-stu-id="748e4-107">For example:</span></span>

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="748e4-p102">可以通过使用标准 REST API 访问一组 Excel 对象（例如表、区域或图表），以便对工作簿执行创建、读取、更新和删除 (CRUD) 操作。例如，`GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets`</span><span class="sxs-lookup"><span data-stu-id="748e4-p102">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets`</span></span>  
<span data-ttu-id="748e4-110">返回属于工作簿的工作表对象的集合。</span><span class="sxs-lookup"><span data-stu-id="748e4-110">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="748e4-111">Excel REST API 仅支持 Office Open XML 文件格式的工作簿。</span><span class="sxs-lookup"><span data-stu-id="748e4-111">The Excel REST API supports only Office Open XML file formatted workbooks.</span></span> <span data-ttu-id="748e4-112">不支持扩展名为 `.xls` 的工作簿。</span><span class="sxs-lookup"><span data-stu-id="748e4-112">The `.xls` extension workbooks are not supported.</span></span> 

<span data-ttu-id="748e4-113">**注意**：仍不支持在 OneDrive 使用者平台中存储的工作簿。</span><span class="sxs-lookup"><span data-stu-id="748e4-113">**Note**: Support for workbooks stored in OneDrive Consumer platform is still not available.</span></span> <span data-ttu-id="748e4-114">目前，Excel REST API 仅支持在商业平台中存储的文件。</span><span class="sxs-lookup"><span data-stu-id="748e4-114">At this time, only the files stored in business platform is supported by Excel REST APIs.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="748e4-115">授权和范围</span><span class="sxs-lookup"><span data-stu-id="748e4-115">Authorization and scopes</span></span>

<span data-ttu-id="748e4-116">可以使用 [Azure AD v.2 终结点](../index.md)对 Excel API 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="748e4-116">You can use the [Azure AD v.2 endpoint](../index.md) to authenticate Excel APIs.</span></span> <span data-ttu-id="748e4-117">所有 API 都要求提供 `Authorization: Bearer {access-token}` HTTP 标头。</span><span class="sxs-lookup"><span data-stu-id="748e4-117">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="748e4-118">要使用 Excel 资源，需要以下[权限范围](/graph/permissions-reference)之一：</span><span class="sxs-lookup"><span data-stu-id="748e4-118">One of the following [permission scopes](/graph/permissions-reference) is required to use the Excel resource:</span></span>

* <span data-ttu-id="748e4-119">Files.Read（适用于读取操作）</span><span class="sxs-lookup"><span data-stu-id="748e4-119">Files.Read (for read actions)</span></span>
* <span data-ttu-id="748e4-120">Files.ReadWrite（适用于读写操作）</span><span class="sxs-lookup"><span data-stu-id="748e4-120">Files.ReadWrite (for read and write actions)</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="748e4-121">会话和永久性</span><span class="sxs-lookup"><span data-stu-id="748e4-121">Sessions and persistence</span></span>

<span data-ttu-id="748e4-122">可以在以下三个模式之一下调用 Excel API：</span><span class="sxs-lookup"><span data-stu-id="748e4-122">Excel APIs can be called in one of three modes:</span></span> 

1. <span data-ttu-id="748e4-123">永久会话 - 保持（保存）对工作簿所做的全部更改。</span><span class="sxs-lookup"><span data-stu-id="748e4-123">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="748e4-124">这是效率和性能最高的操作模式。</span><span class="sxs-lookup"><span data-stu-id="748e4-124">This is the most efficient and performant mode of operation.</span></span> 
2. <span data-ttu-id="748e4-p107">非永久会话 - 不会将 API 所做的更改保存到源位置。相反，Excel 后端服务器保留文件的临时副本，体现在特定 API 会话期间所做的更改。Excel 会话过期时，这些更改将丢失。此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。</span><span class="sxs-lookup"><span data-stu-id="748e4-p107">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span> 
3. <span data-ttu-id="748e4-129">无会话 - 在不使用会话信息的情况下进行 API 调用。</span><span class="sxs-lookup"><span data-stu-id="748e4-129">Sessionless - The API call is made without session information.</span></span> <span data-ttu-id="748e4-130">每次执行操作时，Excel 服务器都需要查找服务器的工作簿副本，因此这不是调用 Excel API 的高效方式。</span><span class="sxs-lookup"><span data-stu-id="748e4-130">Excel servers have to locate the server's copy of the workbook each time to perform the operation and hence this is not an efficient way for call Excel APIs.</span></span> <span data-ttu-id="748e4-131">它适用于发出一次性请求。</span><span class="sxs-lookup"><span data-stu-id="748e4-131">It is suitable for making one off requests.</span></span> 

<span data-ttu-id="748e4-132">若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。</span><span class="sxs-lookup"><span data-stu-id="748e4-132">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="748e4-p109">**注意：** Excel API 不需要会话标头也能起作用。但是，建议你使用会话标头来提高性能。如果不使用会话标头，API 调用过程中进行的更改 _仅_ 保持在该文件中。</span><span class="sxs-lookup"><span data-stu-id="748e4-p109">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="748e4-136">获取会话的 API 调用</span><span class="sxs-lookup"><span data-stu-id="748e4-136">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="748e4-137">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-137">Request</span></span> 

<span data-ttu-id="748e4-138">通过将 `persistchanges` 值设置为 `true` 或 `false` 可传递一个 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="748e4-138">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="748e4-139">当 `persistChanges` 值设置为 `false` 时，则返回非永久会话 id。</span><span class="sxs-lookup"><span data-stu-id="748e4-139">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="748e4-140">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-140">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.sessionInfo",
  "id": "{session-id}",
  "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="748e4-141">用法</span><span class="sxs-lookup"><span data-stu-id="748e4-141">Usage</span></span> 

<span data-ttu-id="748e4-142">将前一个调用中返回的会话 ID </span><span class="sxs-lookup"><span data-stu-id="748e4-142">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="748e4-143">作为 `workbook-session-id` HTTP 标头的后续 API 请求中的标头进行传递。</span><span class="sxs-lookup"><span data-stu-id="748e4-143">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="748e4-144">注意：如果会话 ID 已过期，会话上会返回 `404` HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="748e4-144">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="748e4-145">在这种情况下，可以选择新建一个会话，然后继续。</span><span class="sxs-lookup"><span data-stu-id="748e4-145">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="748e4-146">另一种方法是定期刷新会话，以使会话处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="748e4-146">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="748e4-147">通常，如果永久会话处于不活动状态的时间达到 5 分钟左右，则会话会过期。</span><span class="sxs-lookup"><span data-stu-id="748e4-147">Typically the persistent session expires after about 5 minutes of inactivity.</span></span> <span data-ttu-id="748e4-148">如果非永久会话处于不活动状态的时间达到 7 分钟左右，则会过期。</span><span class="sxs-lookup"><span data-stu-id="748e4-148">Non persistent session expires after about 7 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="748e4-149">常见的 Excel 方案</span><span class="sxs-lookup"><span data-stu-id="748e4-149">Common Excel scenarios</span></span>

<span data-ttu-id="748e4-150">本节提供可用于 Excel 对象的常见操作的示例。</span><span class="sxs-lookup"><span data-stu-id="748e4-150">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="748e4-151">工作表操作</span><span class="sxs-lookup"><span data-stu-id="748e4-151">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="748e4-152">列出工作簿的工作表部分</span><span class="sxs-lookup"><span data-stu-id="748e4-152">List worksheets part of the workbook</span></span> 
<span data-ttu-id="748e4-153">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-153">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-154">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-154">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0000-000000000000}",
      "name": "Sheet1",
      "position": 0,
      "visibility": "Visible"
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0100-000000000000}",
      "name": "Sheet57664",
      "position": 1,
      "visibility": "Visible"
    }
  ]
}
```
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="748e4-155">添加新的工作表</span><span class="sxs-lookup"><span data-stu-id="748e4-155">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/root:/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="748e4-156">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-156">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="748e4-157">获取新的工作表</span><span class="sxs-lookup"><span data-stu-id="748e4-157">Get a new worksheet</span></span> 

<span data-ttu-id="748e4-158">根据名称获取工作表。</span><span class="sxs-lookup"><span data-stu-id="748e4-158">Get a worksheet based on the name.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-159">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-159">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

<span data-ttu-id="748e4-160">\*\*注意：也可以使用 ID 检索工作表。</span><span class="sxs-lookup"><span data-stu-id="748e4-160">\*\* Note: Worksheets can also be retrieved using the ID.</span></span> <span data-ttu-id="748e4-161">但是，目前 ID 包含需要经过 URL 编码才能使 API 工作的 `{` 和“}”字符。</span><span class="sxs-lookup"><span data-stu-id="748e4-161">However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work.</span></span> <span data-ttu-id="748e4-162">示例：若要获取 ID 为 `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}` 的工作表，请将路径中的 ID 进行 URL 编码，编码为 `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`。</span><span class="sxs-lookup"><span data-stu-id="748e4-162">Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="748e4-163">删除工作表</span><span class="sxs-lookup"><span data-stu-id="748e4-163">Delete a worksheet</span></span>

<span data-ttu-id="748e4-164">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-164">Request</span></span>
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-165">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-165">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="748e4-166">更新工作表属性</span><span class="sxs-lookup"><span data-stu-id="748e4-166">Update worksheet properties</span></span>

<span data-ttu-id="748e4-167">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-167">Request</span></span> 

```
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="748e4-168">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-168">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
  "id": "{00000000-0001-0000-0100-000000000000}",
  "name": "SheetA",
  "position": 3,
  "visibility": "Visible"
}
```

### <a name="chart-operations"></a><span data-ttu-id="748e4-169">图表操作</span><span class="sxs-lookup"><span data-stu-id="748e4-169">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="748e4-170">列出属于工作表的图表</span><span class="sxs-lookup"><span data-stu-id="748e4-170">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="748e4-171">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-171">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="748e4-172">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-172">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B00000000-0008-0000-0100-000003000000%7D%27)",
      "height": 235.5,
      "id": "{00000000-0008-0000-0100-000003000000}",
      "left": 276.0,
      "name": "Chart 2",
      "top": 0.0,
      "width": 401.25
   }
  ]
}
```

<span data-ttu-id="748e4-173">\*\*注意：图表 ID 包含需要经过 URL 编码才能使 API 工作的 `{` 和 `}` 字符（例如 `{00000000-0008-0000-0100-000003000000}`）。</span><span class="sxs-lookup"><span data-stu-id="748e4-173">\*\* Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work.</span></span> <span data-ttu-id="748e4-174">示例：若要获取图表对象，请将路径中的 ID 进行 URL 编码，编码为 `/charts/%7B00000000-0008-0000-0100-000003000000%7D`。</span><span class="sxs-lookup"><span data-stu-id="748e4-174">Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="748e4-175">获取图表图像</span><span class="sxs-lookup"><span data-stu-id="748e4-175">Get chart image</span></span>

<span data-ttu-id="748e4-176">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-176">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="748e4-177">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-177">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="748e4-178">添加图表</span><span class="sxs-lookup"><span data-stu-id="748e4-178">Add a chart</span></span>  

<span data-ttu-id="748e4-179">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-179">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="748e4-180">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-180">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chart",
  "@odata.type": "#microsoft.graph.workbookChart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a><span data-ttu-id="748e4-181">更新图表</span><span class="sxs-lookup"><span data-stu-id="748e4-181">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="748e4-182">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-182">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "NewName",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-chart-source-data"></a><span data-ttu-id="748e4-183">更新图表的源数据</span><span class="sxs-lookup"><span data-stu-id="748e4-183">Update chart source data</span></span> 

<span data-ttu-id="748e4-184">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-184">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="748e4-185">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-185">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="748e4-186">表操作</span><span class="sxs-lookup"><span data-stu-id="748e4-186">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="748e4-187">获取表列表</span><span class="sxs-lookup"><span data-stu-id="748e4-187">Get list of tables</span></span> 

<span data-ttu-id="748e4-188">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-188">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-189">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-189">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="748e4-190">创建表</span><span class="sxs-lookup"><span data-stu-id="748e4-190">Create table</span></span>

<span data-ttu-id="748e4-191">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-191">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/{table-id}/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="748e4-192">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-192">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="update-table"></a><span data-ttu-id="748e4-193">更新表</span><span class="sxs-lookup"><span data-stu-id="748e4-193">Update table</span></span>

<span data-ttu-id="748e4-194">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-194">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="748e4-195">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-195">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="748e4-196">获取表行列表</span><span class="sxs-lookup"><span data-stu-id="748e4-196">Get list of table rows</span></span>
<span data-ttu-id="748e4-197">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-197">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-198">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-198">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(0)",
      "index": 0,
      "values": [
        [
          42019,
          53,
          34
       ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(1)",
      "index": 1,
      "values": [
        [
          42020,
          45,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(2)",
      "index": 2,
      "values": [
        [
          42021,
          50,
          31
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(3)",
      "index": 3,
      "values": [
        [
          42022,
          43,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(4)",
      "index": 4,
      "values": [
        [
          42023,
          45,
          41
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(5)",
      "index": 5,
      "values": [
        [
          42024,
          52,
          40
        ]
      ]
    }
  ]
}
```

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="748e4-199">获取表列列表</span><span class="sxs-lookup"><span data-stu-id="748e4-199">Get list of table columns</span></span>

<span data-ttu-id="748e4-200">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-200">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-201">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-201">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/columns",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%271%27)",
      "id": "1",
      "index": 0,
      "name": "Date",
      "values": [
        [
          "Date"
        ],
        [
          42019
       ],
        [
          42020
        ],
        [
          42021
        ],
        [
          42022
        ],
        [
          42023
        ],
        [
          42024
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%272%27)",
      "id": "2",
      "index": 1,
      "name": "High (F)",
      "values": [
        [
          "High (F)"
        ],
        [
          53
        ],
        [
          45
        ],
        [
          50
        ],
        [
          43
        ],
        [
          45
        ],
        [
          52
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%273%27)",
      "id": "3",
      "index": 2,
      "name": "Low (F)",
      "values": [
        [
          "Low (F)"
        ],
        [
          34
        ],
        [
          39
        ],
        [
          31
        ],
        [
          39
        ],
        [
          41
        ],
        [
          40
        ]
      ]
    }
  ]
}
```


#### <a name="add-a-table-row"></a><span data-ttu-id="748e4-202">添加表行</span><span class="sxs-lookup"><span data-stu-id="748e4-202">Add a table row</span></span>

<span data-ttu-id="748e4-203">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-203">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="748e4-204">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-204">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows(null)",
  "index": 6,
  "values": [
    [
      "Jan-15-2016",
      49,
      37
    ]
  ]
}
```

#### <a name="add-a-table-column"></a><span data-ttu-id="748e4-205">添加表列</span><span class="sxs-lookup"><span data-stu-id="748e4-205">Add a table column</span></span> 

<span data-ttu-id="748e4-206">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-206">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="748e4-207">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-207">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('2')/columns/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)/columns(%274%27)",
  "id": "4",
  "index": 2,
  "name": "Status",
  "values": [
    [
      "Status"
    ],
    [
      "Open"
    ],
    [
      "Closed"
    ]
  ]
}
```

#### <a name="delete-table-row"></a><span data-ttu-id="748e4-208">删除表行</span><span class="sxs-lookup"><span data-stu-id="748e4-208">Delete table row</span></span>

<span data-ttu-id="748e4-209">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-209">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http  
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows/$/itemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-210">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-210">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="748e4-211">删除表列</span><span class="sxs-lookup"><span data-stu-id="748e4-211">Delete table column</span></span> 
<span data-ttu-id="748e4-212">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-212">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-213">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-213">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="748e4-214">将表转换为区域</span><span class="sxs-lookup"><span data-stu-id="748e4-214">Convert table to range</span></span> 
<span data-ttu-id="748e4-215">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-215">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-216">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-216">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="748e4-217">表排序</span><span class="sxs-lookup"><span data-stu-id="748e4-217">Table sort</span></span>
<span data-ttu-id="748e4-218">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-218">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```


<span data-ttu-id="748e4-219">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-219">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="748e4-220">表筛选器</span><span class="sxs-lookup"><span data-stu-id="748e4-220">Table filter</span></span>
<span data-ttu-id="748e4-221">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-221">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"criteria" : 
  { "filterOn": "custom",
   "criterion1": ">15",
   "operator": "and",
   "criterion2": "<50"
   
  }
}
```

<span data-ttu-id="748e4-222">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-222">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="748e4-223">清除筛选器</span><span class="sxs-lookup"><span data-stu-id="748e4-223">Clear filter</span></span>
<span data-ttu-id="748e4-224">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-224">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-225">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-225">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="748e4-226">区域操作</span><span class="sxs-lookup"><span data-stu-id="748e4-226">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="748e4-227">获取区域</span><span class="sxs-lookup"><span data-stu-id="748e4-227">Get Range</span></span> 

<span data-ttu-id="748e4-228">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-228">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-229">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-229">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasLocal": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasR1C1": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "values": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "valueTypes": [
    [
      "Empty",
      "Empty"
    ],
    [
      "Empty",
      "Empty"
    ]
  ]
}
```

#### <a name="range-update"></a><span data-ttu-id="748e4-230">区域更新</span><span class="sxs-lookup"><span data-stu-id="748e4-230">Range update</span></span> 

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='test!A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Test", "Value" ], [ "For", "Update" ] ] }
```

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27test!A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasLocal": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasR1C1": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "values": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "valueTypes": [
    [
      "String",
      "String"
    ],
    [
      "String",
      "String"
    ]
  ]
}
```

#### <a name="range-sort"></a><span data-ttu-id="748e4-231">区域排序</span><span class="sxs-lookup"><span data-stu-id="748e4-231">Range sort</span></span>
<span data-ttu-id="748e4-232">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-232">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/usedRange/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```

<span data-ttu-id="748e4-233">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-233">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="748e4-234">已命名项目</span><span class="sxs-lookup"><span data-stu-id="748e4-234">Named items</span></span>
<span data-ttu-id="748e4-235">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-235">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="748e4-236">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-236">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27data%27)",
      "name": "data",
      "type": "Range",
      "value": "Range!$A$1:$D$3",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27myrange%27)",
      "name": "myrange",
      "type": "Range",
      "value": "Range!$E$1:$F$7",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27range1%27)",
      "name": "range1",
      "type": "Range",
      "value": "Range!$I$1:$M$11",
      "visible": true
    }
  ]
}
```

### <a name="work-with-nulls"></a><span data-ttu-id="748e4-237">使用 null</span><span class="sxs-lookup"><span data-stu-id="748e4-237">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="748e4-238">二维数组中的 null 输入</span><span class="sxs-lookup"><span data-stu-id="748e4-238">null input in 2-D array</span></span>

<span data-ttu-id="748e4-p113">区域和表资源中将忽略二维数组中的 `null` 输入（对于值、数字格式、公式）。当 `null` 输入在值、值的数字格式或值的公式网格中发送时，不会对预期目标（单元格）进行更新。</span><span class="sxs-lookup"><span data-stu-id="748e4-p113">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="748e4-241">例如，要仅更新区域的特定部分（例如某些单元格的数字格式）并保留区域其他部分的现有数字格式，请根据需要设置数字格式并对其他单元格发送 `null`。</span><span class="sxs-lookup"><span data-stu-id="748e4-241">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="748e4-242">在以下设置请求中，仅会设置区域数字格式的某些部分，同时保留其余部分的现有数字格式（通过传递 null）。</span><span class="sxs-lookup"><span data-stu-id="748e4-242">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="748e4-243">属性的 null 输入</span><span class="sxs-lookup"><span data-stu-id="748e4-243">null input for a property</span></span>

<span data-ttu-id="748e4-p114">`null` 并非整个属性的有效的单个输入。例如，以下输入无效，因为整个值不能设置为 null，也不能忽略。</span><span class="sxs-lookup"><span data-stu-id="748e4-p114">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="748e4-246">以下输入无效，因为 null 不是有效的颜色值。</span><span class="sxs-lookup"><span data-stu-id="748e4-246">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="748e4-247">Null 响应</span><span class="sxs-lookup"><span data-stu-id="748e4-247">Null-Response</span></span>

<span data-ttu-id="748e4-248">由不一致的值组成的格式属性的表示形式将导致在响应中返回 null 值。</span><span class="sxs-lookup"><span data-stu-id="748e4-248">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="748e4-p115">例如，区域可以由一个或多个单元格组成。如果指定区域中包含的单个单元格不具有一致的格式值，则不会定义区域级别表示形式。</span><span class="sxs-lookup"><span data-stu-id="748e4-p115">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```

<span data-ttu-id="748e4-251">在以下情况下，也会返回 null 值：</span><span class="sxs-lookup"><span data-stu-id="748e4-251">A null value is also returned in the response in the following cases:</span></span>
- <span data-ttu-id="748e4-252">如果在尝试获取对象的特定属性时发生错误并且此属性可设置为 null，则该属性可能会返回 null 值。</span><span class="sxs-lookup"><span data-stu-id="748e4-252">If an error occurs when trying to get a certain property of an object and this property can be set as a null, the property might return a null value in the response.</span></span>
- <span data-ttu-id="748e4-253">对于 range 对象，在获取整行或整列的区域时，某些属性可能会返回 null。</span><span class="sxs-lookup"><span data-stu-id="748e4-253">For a range object, when getting a range for entire row or entire column, some properties might return null as the response.</span></span> <span data-ttu-id="748e4-254">如果区域大小超过了上限（5M 单元格），则某些属性将返回 null 值。</span><span class="sxs-lookup"><span data-stu-id="748e4-254">If the range size exceeds the upper limitation (5M cells), some properties will return null as the value.</span></span>

### <a name="blank-input-and-output"></a><span data-ttu-id="748e4-255">空白输入和输出</span><span class="sxs-lookup"><span data-stu-id="748e4-255">Blank input and output</span></span>

<span data-ttu-id="748e4-p117">更新请求中的空白值视为清除或重置相应属性的指令。空白值表示为两个双引号，中间没有空格：`""`。</span><span class="sxs-lookup"><span data-stu-id="748e4-p117">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="748e4-258">示例：</span><span class="sxs-lookup"><span data-stu-id="748e4-258">Examples:</span></span>

* <span data-ttu-id="748e4-259">对于 `values`，将清除区域值。这与清除应用程序中的内容相同。</span><span class="sxs-lookup"><span data-stu-id="748e4-259">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="748e4-260">对于 `numberFormat`，数字格式设置为 `General`。</span><span class="sxs-lookup"><span data-stu-id="748e4-260">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="748e4-261">对于 `formula` 和 `formulaLocale`，将清除公式值。</span><span class="sxs-lookup"><span data-stu-id="748e4-261">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="748e4-p118">对于读取操作，预计单元格内容为空时会收到空白值。如果单元格不包含数据或值，该 API 将返回空白值。空白值表示为两个双引号，中间没有空格：`""`。</span><span class="sxs-lookup"><span data-stu-id="748e4-p118">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

```json
{
  "values" : [["", "some", "data", "in", "other", "cells", ""]]
}
```

```json
{
  "formula" : [["", "", "=Rand()"]]
}
```


### <a name="unbounded-range"></a><span data-ttu-id="748e4-265">无限区域</span><span class="sxs-lookup"><span data-stu-id="748e4-265">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="748e4-266">读取</span><span class="sxs-lookup"><span data-stu-id="748e4-266">Read</span></span>

<span data-ttu-id="748e4-267">无限区域地址仅包含列或行标识符和未指定的行标识符或列标识符（分别），例如：</span><span class="sxs-lookup"><span data-stu-id="748e4-267">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="748e4-268">`C:C`、`A:F`、`A:XFD`（包含未指定的行）</span><span class="sxs-lookup"><span data-stu-id="748e4-268">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="748e4-269">`2:2`、`1:4`、`1:1048546`（包含未指定的列）</span><span class="sxs-lookup"><span data-stu-id="748e4-269">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="748e4-p119">当 API 发出检索无限区域 (`getRange('C:C')`) 的请求时，返回的响应包含单元格级别属性的 `null`例如 `values`、`text`、`numberFormat` 或 `formula`。其他区域属性（例如 `address` 或 `cellCount`）将反映无限区域。</span><span class="sxs-lookup"><span data-stu-id="748e4-p119">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="748e4-272">写入</span><span class="sxs-lookup"><span data-stu-id="748e4-272">Write</span></span>

<span data-ttu-id="748e4-273">**不允许** 在无限区域上设置单元格级别属性（例如值、numberFormat 等），因为输入请求可能过大而无法处理。</span><span class="sxs-lookup"><span data-stu-id="748e4-273">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="748e4-274">例如，下面不是一个有效的更新请求，因为所请求的区域是无限的。</span><span class="sxs-lookup"><span data-stu-id="748e4-274">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/root/workbook/worksheets/{id}/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="748e4-275">当尝试对此类区域执行更新操作时，API 将返回错误。</span><span class="sxs-lookup"><span data-stu-id="748e4-275">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="748e4-276">大区域</span><span class="sxs-lookup"><span data-stu-id="748e4-276">Large Range</span></span>

<span data-ttu-id="748e4-p120">大区域意味着区域大小对于单个 API 调用来说过大。区域中包含的很多因素（例如单元格数量、值、numberFormat 和公式）都会使响应过大，而不适合于 API 交互。API 努力尝试返回或写入到请求的数据。但是，由于资源利用率较高，涉及的大尺寸可能会导致 API 错误的情况。</span><span class="sxs-lookup"><span data-stu-id="748e4-p120">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="748e4-281">为了避免出现这种情况，建议以多个较小的区域大小对大区域执行读取或写入。</span><span class="sxs-lookup"><span data-stu-id="748e4-281">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="748e4-282">单个输入副本</span><span class="sxs-lookup"><span data-stu-id="748e4-282">Single input copy</span></span>

<span data-ttu-id="748e4-p121">为了支持使用相同的值或数字格式更新区域或在整个区域应用相同的公式，在一组 API 中使用以下约定。在 Excel 中，此行为与在 CTRL+Enter 模式下将值或公式输入到区域中相似。</span><span class="sxs-lookup"><span data-stu-id="748e4-p121">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="748e4-285">API 将查找 *单个单元格值*，如果目标区域尺寸与输入区域尺寸不符，它将在 CTRL+Enter 模式下，使用请求中提供的值或公式更新整个区域。</span><span class="sxs-lookup"><span data-stu-id="748e4-285">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="748e4-286">示例</span><span class="sxs-lookup"><span data-stu-id="748e4-286">Examples</span></span>

<span data-ttu-id="748e4-p122">以下请求使用“Sample text”文本更新选定的区域。请注意，区域包含 200 个单元格，而提供的输入仅包含 1 个单元格值。</span><span class="sxs-lookup"><span data-stu-id="748e4-p122">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/root/workbook/worksheets/{id}/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="748e4-289">工作簿函数</span><span class="sxs-lookup"><span data-stu-id="748e4-289">Workbook functions</span></span> 
<span data-ttu-id="748e4-290">可以通过 /Functions 资源中包含的函数集合访问工作簿函数。</span><span class="sxs-lookup"><span data-stu-id="748e4-290">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="748e4-291">请求</span><span class="sxs-lookup"><span data-stu-id="748e4-291">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a><span data-ttu-id="748e4-292">响应</span><span class="sxs-lookup"><span data-stu-id="748e4-292">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a><span data-ttu-id="748e4-293">错误信息</span><span class="sxs-lookup"><span data-stu-id="748e4-293">Error information</span></span> 

<span data-ttu-id="748e4-p123">返回错误，其中包括 HTTP 错误代码和错误对象。错误 `code` 和 `message` 解释了导致错误的原因。</span><span class="sxs-lookup"><span data-stu-id="748e4-p123">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="748e4-296">示例如下。</span><span class="sxs-lookup"><span data-stu-id="748e4-296">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

## <a name="whats-new"></a><span data-ttu-id="748e4-297">最近更新</span><span class="sxs-lookup"><span data-stu-id="748e4-297">What's new</span></span>
<span data-ttu-id="748e4-298">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="748e4-298">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
